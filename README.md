# ujjwal.github.io
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
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        .skill-icon {
            transition: all 0.3s ease;
        }
        .skill-icon:hover {
            transform: translateY(-5px);
        }
    </style>
</head>
<body class="min-h-screen">
    <!-- Navigation -->
    <nav class="bg-white/80 backdrop-blur-md shadow-sm fixed w-full z-50">
        <div class="max-w-6xl mx-auto px-4">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <span class="font-bold text-xl bg-gradient-to-r from-blue-600 to-indigo-600 bg-clip-text text-transparent">Portfolio</span>
                </div>
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#home" class="text-gray-700 hover:text-blue-600 transition-colors duration-300">Home</a>
                    <a href="#about" class="text-gray-700 hover:text-blue-600 transition-colors duration-300">About</a>
                    <a href="#skills" class="text-gray-700 hover:text-blue-600 transition-colors duration-300">Skills</a>
                    <a href="#projects" class="text-gray-700 hover:text-blue-600 transition-colors duration-300">Projects</a>
                    <a href="#contact" class="text-gray-700 hover:text-blue-600 transition-colors duration-300">Contact</a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="pt-32 pb-20 px-4" data-aos="fade-in">
        <div class="max-w-4xl mx-auto text-center">
            <h1 class="text-5xl md:text-6xl font-bold mb-6 bg-gradient-to-r from-blue-600 to-indigo-600 bg-clip-text text-transparent">Hi, I'm Ujjwal</h1>
            <p class="text-xl md:text-2xl text-gray-600 mb-8">BTech Professional | Data Visualization Expert</p>
            <div class="flex justify-center space-x-4">
                <a href="#projects" class="px-8 py-3 bg-blue-600 text-white rounded-full font-medium hover:bg-blue-700 transition-all duration-300 transform hover:-translate-y-1 shadow-lg hover:shadow-xl">View My Work</a>
                <a href="#contact" class="px-8 py-3 border border-blue-600 text-blue-600 rounded-full font-medium hover:bg-blue-50 transition-all duration-300 transform hover:-translate-y-1">Contact Me</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 px-4 bg-white/50 backdrop-blur-sm" data-aos="fade-up">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">About Me</h2>
            <div class="flex flex-col md:flex-row items-center gap-12">
                <div class="md:w-1/2" data-aos="fade-right">
                    <div class="glass-card rounded-2xl p-1 shadow-xl">
                        <img src="https://via.placeholder.com/500" alt="Profile" class="rounded-2xl w-full">
                    </div>
                </div>
                <div class="md:w-1/2" data-aos="fade-left">
                    <h3 class="text-2xl font-semibold mb-4 text-gray-800">Data Specialist & Problem Solver</h3>
                    <p class="text-gray-600 mb-4 leading-relaxed">With extensive experience in Excel, Power BI, and Python, I transform complex data into actionable insights that drive business decisions.</p>
                    <p class="text-gray-600 mb-6 leading-relaxed">My technical expertise combined with strong analytical skills allows me to create efficient, scalable solutions for data processing and visualization.</p>
                    <div class="flex space-x-4">
                        <a href="#" class="px-6 py-2 bg-blue-600 text-white rounded-full hover:bg-blue-700 transition-all duration-300 flex items-center">
                            <i class="fas fa-download mr-2"></i> Download CV
                        </a>
                        <a href="#contact" class="px-6 py-2 border border-blue-600 text-blue-600 rounded-full hover:bg-blue-50 transition-all duration-300 flex items-center">
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
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">My Expertise</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Excel -->
                <div class="glass-card p-8 rounded-2xl text-center hover:shadow-xl transition-all duration-500" data-aos="zoom-in">
                    <div class="text-blue-600 mb-4 skill-icon">
                        <i class="fas fa-file-excel text-6xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-gray-800">Advanced Excel</h3>
                    <p class="text-gray-600">Complex formulas, VBA automation, pivot tables, and dynamic dashboards for data analysis and reporting.</p>
                </div>
                
                <!-- Power BI -->
                <div class="glass-card p-8 rounded-2xl text-center hover:shadow-xl transition-all duration-500" data-aos="zoom-in" data-aos-delay="150">
                    <div class="text-purple-600 mb-4 skill-icon">
                        <i class="fas fa-chart-line text-6xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-gray-800">Power BI</h3>
                    <p class="text-gray-600">Interactive dashboards, DAX formulas, data modeling, and business intelligence solutions.</p>
                </div>
                
                <!-- Python -->
                <div class="glass-card p-8 rounded-2xl text-center hover:shadow-xl transition-all duration-500" data-aos="zoom-in" data-aos-delay="300">
                    <div class="text-green-600 mb-4 skill-icon">
                        <i class="fab fa-python text-6xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-gray-800">Python</h3>
                    <p class="text-gray-600">Data analysis with Pandas, automation scripts, and visualization with Matplotlib/Seaborn.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-20 px-4 bg-white/50 backdrop-blur-sm">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800" data-aos="fade-in">Featured Projects</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="glass-card rounded-2xl overflow-hidden hover:shadow-xl transition-all duration-500" data-aos="fade-up">
                    <div class="h-48 overflow-hidden">
                        <img src="https://via.placeholder.com/600x400" alt="Project 1" class="w-full h-full object-cover hover:scale-105 transition-transform duration-500">
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2 text-gray-800">Sales Analytics Dashboard</h3>
                        <p class="text-gray-600 mb-4">Interactive Power BI dashboard with real-time sales metrics and predictive analytics.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-blue-100 text-blue-800 px-3 py-1 rounded-full text-sm">Power BI</span>
                            <span class="bg-purple-100 text-purple-800 px-3 py-1 rounded-full text-sm">DAX</span>
                        </div>
                        <a href="#" class="text-blue-600 font-medium hover:underline flex items-center">
                            View Details <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="glass-card rounded-2xl overflow-hidden hover:shadow-xl transition-all duration-500" data-aos="fade-up" data-aos-delay="150">
                    <div class="h-48 overflow-hidden">
                        <img src="https://via.placeholder.com/600x400" alt="Project 2" class="w-full h-full object-cover hover:scale-105 transition-transform duration-500">
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2 text-gray-800">Inventory Management System</h3>
                        <p class="text-gray-600 mb-4">Python application with automated reporting and stock level predictions.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-green-100 text-green-800 px-3 py-1 rounded-full text-sm">Python</span>
                            <span class="bg-red-100 text-red-800 px-3 py-1 rounded-full text-sm">Pandas</span>
                        </div>
                        <a href="#" class="text-blue-600 font-medium hover:underline flex items-center">
                            View Details <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="glass-card rounded-2xl overflow-hidden hover:shadow-xl transition-all duration-500" data-aos="fade-up" data-aos-delay="300">
                    <div class="h-48 overflow-hidden">
                        <img src="https://via.placeholder.com/600x400" alt="Project 3" class="w-full h-full object-cover hover:scale-105 transition-transform duration-500">
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2 text-gray-800">Financial Reporting Tool</h3>
                        <p class="text-gray-600 mb-4">Excel-based solution with automated data processing and visualization.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-blue-100 text-blue-800 px-3 py-1 rounded-full text-sm">Excel</span>
                            <span class="bg-gray-100 text-gray-800 px-3 py-1 rounded-full text-sm">VBA</span>
                        </div>
                        <a href="#" class="text-blue-600 font-medium hover:underline flex items-center">
                            View Details <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 px-4">
        <div class="max-w-2xl mx-auto" data-aos="fade-in">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Get In Touch</h2>
            <form class="glass-card p-8 rounded-2xl shadow-lg hover:shadow-xl transition-all duration-500" action="https://formspree.io/f/ujjwalshukla291@gmail.com" method="POST" data-aos="fade-up">
                <div class="mb-6">
                    <label for="name" class="block text-gray-700 font-medium mb-2">Name</label>
                    <input type="text" id="name" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-all duration-300">
                </div>
                <div class="mb-6">
                    <label for="email" class="block text-gray-700 font-medium mb-2">Email</label>
                    <input type="email" id="email" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-all duration-300">
                </div>
                <div class="mb-6">
                    <label for="message" class="block text-gray-700 font-medium mb-2">Message</label>
                    <textarea id="message" rows="4" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-all duration-300"></textarea>
                </div>
                <input type="hidden" name="_replyto" value="ujjwalshukla291@gmail.com">
                <button type="submit" class="w-full bg-blue-600 text-white py-3 rounded-lg font-medium hover:bg-blue-700 transition-all duration-300 flex items-center justify-center transform hover:scale-105 hover:shadow-lg active:scale-95" data-aos="zoom-in" data-aos-delay="300">
                    <i class="fas fa-paper-plane mr-2"></i> Send Message
                </button>
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
                <p>&copy; 2023 All Rights Reserved</p>
            </div>
        </div>
    </footer>

    <script>
        AOS.init({
            duration: 800,
            easing: 'ease-in-out',
            once: true
        });
    </script>
</body>
