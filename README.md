<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Simple Calculator</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f4f4;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    .calculator {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      width: 260px;
    }
    .display {
      width: 100%;
      height: 50px;
      font-size: 24px;
      text-align: right;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
      margin-bottom: 15px;
      box-sizing: border-box;
      background: #e9e9e9;
      user-select: none;
    }
    .buttons {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 10px;
    }
    button {
      padding: 15px;
      font-size: 18px;
      border: none;
      border-radius: 5px;
      background: #007bff;
      color: white;
      cursor: pointer;
      transition: background 0.3s ease;
      user-select: none;
    }
    button.operator {
      background: #28a745;
    }
    button.equal {
      background: #dc3545;
      grid-column: span 2;
    }
    button.clear {
      background: #6c757d;
      grid-column: span 2;
    }
    button:hover {
      background: #0056b3;
    }
    button.operator:hover {
      background: #1e7e34;
    }
    button.equal:hover {
      background: #bd2130;
    }
    button.clear:hover {
      background: #5a6268;
    }
  </style>
</head>
<body>
  <div class="calculator">
    <div id="display" class="display">0</div>
    <div class="buttons">
      <button class="clear" id="clear">C</button>
      <button class="operator" data-op="/">÷</button>
      <button class="operator" data-op="*">×</button>
      <button class="operator" data-op="-">−</button>

      <button data-num="7">7</button>
      <button data-num="8">8</button>
      <button data-num="9">9</button>
      <button class="operator" data-op="+">+</button>

      <button data-num="4">4</button>
      <button data-num="5">5</button>
      <button data-num="6">6</button>
      <button data-num="1">1</button>

      <button data-num="1">1</button>
      <button data-num="2">2</button>
      <button data-num="3">3</button>
      <button class="equal" id="equals">=</button>

      <button data-num="0" style="grid-column: span 2;">0</button>
      <button data-num=".">.</button>
    </div>
  </div>

  <script>
    (function() {
      const display = document.getElementById('display');
      const buttons = document.querySelectorAll('button');
      let currentInput = '';
      let lastInput = '';
      let resetNext = false;

      function updateDisplay(value) {
        display.textContent = value;
      }

      function isOperator(char) {
        return ['+', '-', '*', '/'].includes(char);
      }

      buttons.forEach(button => {
        button.addEventListener('click', () => {
          const num = button.getAttribute('data-num');
          const op = button.getAttribute('data-op');
          const id = button.id;

          if (id === 'clear') {
            currentInput = '';
            updateDisplay('0');
            resetNext = false;
            return;
          }

          if (id === 'equals') {
            try {
              // Evaluate expression safely
              let result = eval(currentInput);
              if (result === Infinity || result === -Infinity) {
                updateDisplay('Error');
              } else {
                updateDisplay(result);
                currentInput = result.toString();
              }
            } catch (e) {
              updateDisplay('Error');
              currentInput = '';
            }
            resetNext = true;
            return;
          }

          if (num !== null) {
            if (resetNext) {
              currentInput = '';
              resetNext = false;
            }
            // Prevent multiple dots in one number
            if (num === '.') {
              const parts = currentInput.split(/[\+\-\*\/]/);
              const lastPart = parts[parts.length - 1];
              if (lastPart.includes('.')) return;
              if (lastPart === '') currentInput += '0'; // add leading 0 if dot is first char
            }
            currentInput += num;
            updateDisplay(currentInput);
            return;
          }

          if (op !== null) {
            if (currentInput === '') return; // Do not start with operator
            if (resetNext) resetNext = false;
            // Prevent two operators in a row
            if (isOperator(currentInput.slice(-1))) {
              currentInput = currentInput.slice(0, -1);
            }
            currentInput += op;
            updateDisplay(currentInput);
            return;
          }
        });
      });
    })();
  </script>
</body>
</html>
