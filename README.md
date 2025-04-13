<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated Portfolio | BTech Expert</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #a8e0ff, #ffffff);
            color: #333;
        }
        
        /* Dark mode styles */
        .dark body {
            background: linear-gradient(135deg, #1a1a2e, #16213e);
            color: #f8f9fa;
        }
        .dark .glass-card {
            background: rgba(30, 30, 30, 0.8);
            border-color: rgba(255, 255, 255, 0.1);
        }
        .dark a {
            color: #58a6ff;
        }
        .dark a:hover {
            color: #79ff97;
        }
        .dark h1, .dark h2, .dark h3 {
            color: #ffffff;
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(5px);
            border: 1px solid rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }
        .glass-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
        }
        .skill-icon {
            transition: all 0.3s ease;
        }
        .skill-icon:hover {
            transform: translateY(-5px) scale(1.1);
        }
        a {
            color: #007bff;
        }
        a:hover {
            color: #0056b3;
        }
    </style>
</head>
<body class="min-h-screen">
    <!-- Navigation -->
    <nav class="bg-white/80 backdrop-blur-md shadow-sm fixed w-full z-50 dark:bg-gray-800/80">
        <div class="max-w-6xl mx-auto px-4">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <span class="font-bold text-xl bg-gradient-to-r from-blue-600 to-indigo-600 bg-clip-text text-transparent">Portfolio</span>
                </div>
                <div class="flex items-center space-x-8">
                    <a href="#home" class="text-gray-700 hover:text-blue-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400">Home</a>
                    <a href="#about" class="text-gray-700 hover:text-blue-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400">About</a>
                    <a href="#skills" class="text-gray-700 hover:text-blue-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400">Skills</a>
                    <a href="#projects" class="text-gray-700 hover:text-blue-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400">Projects</a>
                    <a href="#contact" class="text-gray-700 hover:text-blue-600 transition-colors duration-300 dark:text-gray-300 dark:hover:text-blue-400">Contact</a>
                    <button id="theme-toggle" class="p-2 rounded-full bg-gray-200 dark:bg-gray-700 text-gray-700 dark:text-gray-200 hover:bg-gray-300 dark:hover:bg-gray-600 transition-all duration-300 transform hover:rotate-180">
                        <i class="fas fa-moon dark:hidden"></i>
                        <i class="fas fa-sun hidden dark:block"></i>
                    </button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="pt-32 pb-20 px-4" data-aos="fade-in">
        <div class="max-w-4xl mx-auto text-center">
            <h1 class="text-5xl md:text-6xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-indigo-600 bg-clip-text text-transparent">Hi, I'm Ujjwal</h1>
            <p class="text-xl md:text-2xl text-gray-600 mb-8 dark:text-gray-300">BTech Professional | Data Visualization Expert</p>
            <div class="flex justify-center space-x-4">
                <a href="#projects" class="px-8 py-3 bg-blue-600 text-white rounded-full font-medium hover:bg-blue-700 transition-all duration-300 transform hover:-translate-y-1 shadow-lg hover:shadow-xl">View My Work</a>
                <a href="#contact" class="px-8 py-3 border border-blue-600 text-blue-600 rounded-full font-medium hover:bg-blue-50 transition-all duration-300 transform hover:-translate-y-1 dark:text-blue-400 dark:border-blue-400 dark:hover:bg-gray-700">Contact Me</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 px-4 bg-white/50 backdrop-blur-sm dark:bg-gray-800/50" data-aos="fade-up">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800 dark:text-white">About Me</h2>
            <div class="flex flex-col md:flex-row items-center gap-12">
                <div class="md:w-1/2" data-aos="fade-right">
                    <div class="glass-card rounded-2xl p-1 shadow-xl">
                        <img src="https://via.placeholder.com/500" alt="Profile" class="rounded-2xl w-full">
                    </div>
                </div>
                <div class="md:w-1/2" data-aos="fade-left">
                    <h3 class="text-2xl font-semibold mb-4 text-gray-800 dark:text-white">Data Specialist & Problem Solver</h3>
                    <p class="text-gray-600 mb-4 leading-relaxed dark:text-gray-300">With extensive experience in Excel, Power BI, and Python, I transform complex data into actionable insights that drive business decisions.</p>
                    <p class="text-gray-600 mb-6 leading-relaxed dark:text-gray-300">My technical expertise combined with strong analytical skills allows me to create efficient, scalable solutions for data processing and visualization.</p>
                    <div class="flex space-x-4">
                        <a href="#" class="px-6 py-2 bg-blue-600 text-white rounded-full hover:bg-blue-700 transition-all duration-300 flex items-center">
                            <i class="fas fa-download mr-2"></i> Download CV
                        </a>
                        <a href="#contact" class="px-6 py-2 border border-blue-600 text-blue-600 rounded-full hover:bg-blue-50 transition-all duration-300 flex items-center dark:text-blue-400 dark:border-blue-400 dark:hover:bg-gray-700">
                            <i class="fas fa-paper-plane mr-2"></i> Contact Me
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-20 px-4" data-aos="fade-in">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800 dark:text-white">My Expertise</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Excel -->
                <div class="glass-card p-8 rounded-2xl text-center hover:shadow-xl transition-all duration-500" data-aos="zoom-in">
                    <div class="text-blue-600 mb-4 skill-icon">
                        <i class="fas fa-file-excel text-6xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-gray-800 dark:text-white">Advanced Excel</h3>
                    <p class="text-gray-600 dark:text-gray-300">Complex formulas, VBA automation, pivot tables, and dynamic dashboards for data analysis and reporting.</p>
                </div>
                
                <!-- Power BI -->
                <div class="glass-card p-8 rounded-2xl text-center hover:shadow-xl transition-all duration-500" data-aos="zoom-in" data-aos-delay="150">
                    <div class="text-purple-600 mb-4 skill-icon">
                        <i class="fas fa-chart-line text-6xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-gray-800 dark:text-white">Power BI</h3>
                    <p class="text-gray-600 dark:text-gray-300">Interactive dashboards, DAX formulas, data modeling, and business intelligence solutions.</p>
                </div>
                
                <!-- Python -->
                <div class="glass-card p-8 rounded-2xl text-center hover:shadow-xl transition-all duration-500" data-aos="zoom-in" data-aos-delay="300">
                    <div class="text-green-600 mb-4 skill-icon">
                        <i class="fab fa-python text-6xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-gray-800 dark:text-white">Python</h3>
                    <p class="text-gray-600 dark:text-gray-300">Data analysis with Pandas, automation scripts, and visualization with Matplotlib/Seaborn.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-20 px-4 bg-white/50 backdrop-blur-sm dark:bg-gray-800/50">
        <div class="max-w-6xl mx-auto text-center">
            <h2 class="text-3xl font-bold mb-12 text-gray-800 dark:text-white" data-aos="fade-in">My Projects</h2>
            <div class="glass-card p-12 rounded-2xl" data-aos="fade-up">
                <i class="fas fa-code-branch text-6xl text-blue-600 mb-6"></i>
                <h3 class="text-2xl font-bold mb-4 text-gray-800 dark:text-white">Projects Coming Soon</h3>
                <p class="text-gray-600 mb-6 dark:text-gray-300">I'm currently working on some exciting projects that showcase my skills in data analysis and visualization.</p>
                <p class="text-gray-600 dark:text-gray-300">Check back soon to see my work!</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 px-4">
        <div class="max-w-2xl mx-auto" data-aos="fade-in">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800 dark:text-white">Get In Touch</h2>
            <form class="glass-card p-8 rounded-2xl shadow-lg hover:shadow-xl transition-all duration-500" 
                  action="https://formspree.io/f/mqapnjao" 
                  method="POST" 
                  data-aos="fade-up" 
                  id="contact-form">
                <div class="mb-6">
                    <label for="name" class="block text-gray-700 font-medium mb-2 dark:text-gray-300">Name</label>
                    <input type="text" id="name" name="name" required
                           class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-all duration-300 dark:bg-gray-700 dark:border-gray-600 dark:text-white">
                </div>
                <div class="mb-6">
                    <label for="email" class="block text-gray-700 font-medium mb-2 dark:text-gray-300">Email</label>
                    <input type="email" id="email" name="email" required
                           class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-all duration-300 dark:bg-gray-700 dark:border-gray-600 dark:text-white">
                </div>
                <div class="mb-6">
                    <label for="message" class="block text-gray-700 font-medium mb-2 dark:text-gray-300">Message</label>
                    <textarea id="message" name="message" rows="4" required
                              class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-all duration-300 dark:bg-gray-700 dark:border-gray-600 dark:text-white"></textarea>
                </div>
                <button type="submit" class="w-full bg-blue-600 text-white py-3 rounded-lg font-medium hover:bg-blue-700 transition-all duration-300 flex items-center justify-center transform hover:scale-105 hover:shadow-lg active:scale-95" 
                        data-aos="zoom-in" data-aos-delay="300">
                    <i class="fas fa-paper-plane mr-2"></i> Send Message
                </button>
                <div id="form-message" class="mt-4 text-center hidden"></div>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12 px-4">
        <div class="max-w-6xl mx-auto">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-6 md:mb-0">
                    <h3 class="text-xl font-bold">Ujjwal</h3>
                    <p class="text-gray-400 mt-2">Data Specialist & Problem Solver</p>
                </div>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-400 hover:text-white transition-colors duration-300 text-xl">
                        <i class="fab fa-linkedin"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition-colors duration-300 text-xl">
                        <i class="fab fa-github"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition-colors duration-300 text-xl">
                        <i class="fab fa-twitter"></i>
                    </a>
                </div>
            </div>
            <div class="border-t border-gray-800 mt-8 pt-8 text-center text-gray-400">
                <p>&copy; 2025 All Rights Reserved</p>
            </div>
        </div>
    </footer>

    <script>
        // Initialize AOS animations
        AOS.init({
            duration: 800,
            easing: 'ease-in-out',
            once: true
        });

        // Dark mode functionality
        document.addEventListener('DOMContentLoaded', function() {
            const themeToggle = document.getElementById('theme-toggle');
            const html = document.documentElement;
            
            // Check for saved theme preference or use system preference
            const savedTheme = localStorage.getItem('theme') || 
                             (window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light');
            
            // Apply the saved theme
            if (savedTheme === 'dark') {
                html.classList.add('dark');
            } else {
                html.classList.remove('dark');
            }
            
            // Theme toggle button click handler
            themeToggle.addEventListener('click', () => {
                html.classList.toggle('dark');
                const isDark = html.classList.contains('dark');
                localStorage.setItem('theme', isDark ? 'dark' : 'light');
            });

            // Form submission handler
            const form = document.getElementById('contact-form');
            const formMessage = document.getElementById('form-message');
            
            if (form) {
                form.addEventListener('submit', async (e) => {
                    e.preventDefault();
                    const submitBtn = form.querySelector('button[type="submit"]');
                    const originalText = submitBtn.innerHTML;
                    
                    submitBtn.disabled = true;
                    submitBtn.innerHTML = '<i class="fas fa-spinner fa-spin mr-2"></i> Sending...';
                    
                    try {
                        const formData = new FormData(form);
                        
                        // Add honeypot field (optional spam prevention)
                        formData.append('_gotcha', '');
                        
                        const response = await fetch(form.action, {
                            method: 'POST',
                            body: formData,
                            headers: {
                                'Accept': 'application/json'
                            }
                        });
                        
                        if (response.ok) {
                            formMessage.textContent = 'Message sent successfully! I\'ll get back to you soon.';
                            formMessage.classList.remove('hidden', 'text-red-600');
                            formMessage.classList.add('text-green-600');
                            form.reset();
                        } else {
                            const errorData = await response.json();
                            throw new Error(errorData.error || 'Form submission failed');
                        }
                    } catch (error) {
                        formMessage.textContent = `Error: ${error.message}`;
                        formMessage.classList.remove('hidden', 'text-green-600');
                        formMessage.classList.add('text-red-600');
                    } finally {
                        submitBtn.disabled = false;
                        submitBtn.innerHTML = originalText;
                        formMessage.classList.remove('hidden');
                        
                        // Hide message after 5 seconds
                        setTimeout(() => {
                            formMessage.classList.add('hidden');
                        }, 5000);
                    }
                });
            }
        });
    </script>
</body>
</html>
