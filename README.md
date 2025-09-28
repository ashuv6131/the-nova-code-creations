 THE NOVA CODE CREATIONS
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nova Creations Codes - Building Ideas into Reality</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            box-sizing: border-box;
        }
        
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');
        
        * {
            font-family: 'Inter', sans-serif;
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .card-hover {
            transition: all 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 0.8s ease forwards;
        }
        
        @keyframes fadeInUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .stagger-1 { animation-delay: 0.1s; }
        .stagger-2 { animation-delay: 0.2s; }
        .stagger-3 { animation-delay: 0.3s; }
        .stagger-4 { animation-delay: 0.4s; }
        
        .pulse-glow {
            animation: pulseGlow 2s infinite;
        }
        
        @keyframes pulseGlow {
            0%, 100% { box-shadow: 0 0 20px rgba(102, 126, 234, 0.4); }
            50% { box-shadow: 0 0 30px rgba(102, 126, 234, 0.8); }
        }
        
        .floating {
            animation: floating 3s ease-in-out infinite;
        }
        
        @keyframes floating {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }
        
        .text-gradient {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .nav-link {
            position: relative;
            transition: color 0.3s ease;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -5px;
            left: 0;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            transition: width 0.3s ease;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        .service-icon {
            transition: all 0.3s ease;
        }
        
        .service-card:hover .service-icon {
            transform: scale(1.1) rotate(5deg);
        }
        
        .review-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .contact-btn {
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .contact-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            transition: left 0.5s;
        }
        
        .contact-btn:hover::before {
            left: 100%;
        }
        
        .scroll-smooth {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-gray-50 scroll-smooth">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full bg-white/90 backdrop-blur-md z-50 shadow-sm">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center py-4">
                <div class="flex items-center space-x-3">
                    <div class="w-10 h-10 gradient-bg rounded-lg flex items-center justify-center">
                        <span class="text-white font-bold text-xl">N</span>
                    </div>
                    <span class="text-xl font-bold text-gray-800">Nova Creations</span>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="nav-link text-gray-700 hover:text-purple-600">Home</a>
                    <a href="#services" class="nav-link text-gray-700 hover:text-purple-600">Services</a>
                    <a href="#reviews" class="nav-link text-gray-700 hover:text-purple-600">Reviews</a>
                    <a href="#about" class="nav-link text-gray-700 hover:text-purple-600">About</a>
                    <a href="#terms" class="nav-link text-gray-700 hover:text-purple-600">Terms</a>
                    <a href="#contact" class="nav-link text-gray-700 hover:text-purple-600">Contact</a>
                </div>
                <button class="md:hidden text-gray-700" onclick="toggleMobileMenu()">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
        </div>
        <!-- Mobile Menu -->
        <div id="mobileMenu" class="hidden md:hidden bg-white border-t">
            <div class="px-4 py-2 space-y-2">
                <a href="#home" class="block py-2 text-gray-700 hover:text-purple-600">Home</a>
                <a href="#services" class="block py-2 text-gray-700 hover:text-purple-600">Services</a>
                <a href="#reviews" class="block py-2 text-gray-700 hover:text-purple-600">Reviews</a>
                <a href="#about" class="block py-2 text-gray-700 hover:text-purple-600">About</a>
                <a href="#terms" class="block py-2 text-gray-700 hover:text-purple-600">Terms</a>
                <a href="#contact" class="block py-2 text-gray-700 hover:text-purple-600">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="min-h-screen gradient-bg flex items-center justify-center relative overflow-hidden">
        <div class="absolute inset-0 bg-black/20"></div>
        <div class="relative z-10 text-center text-white px-4 max-w-4xl mx-auto">
            <div class="fade-in stagger-1">
                <h1 class="text-5xl md:text-7xl font-bold mb-6 floating">
                    Nova Creations <span class="text-yellow-300">Codes</span>
                </h1>
            </div>
            <div class="fade-in stagger-2">
                <p class="text-xl md:text-2xl mb-8 text-gray-200">
                    Building Ideas into Reality
                </p>
            </div>
            <div class="fade-in stagger-3">
                <p class="text-lg mb-10 text-gray-300 max-w-2xl mx-auto">
                    Professional web development, stunning designs, and custom solutions that bring your vision to life
                </p>
            </div>
            <div class="fade-in stagger-4">
                <a href="#services" class="inline-block bg-white text-purple-600 px-8 py-4 rounded-full font-semibold text-lg hover:bg-gray-100 transition-all duration-300 pulse-glow">
                    Explore Our Services
                </a>
            </div>
        </div>
        
        <!-- Floating Elements -->
        <div class="absolute top-20 left-10 w-20 h-20 bg-white/10 rounded-full floating" style="animation-delay: 0.5s;"></div>
        <div class="absolute bottom-20 right-10 w-16 h-16 bg-yellow-300/20 rounded-full floating" style="animation-delay: 1s;"></div>
        <div class="absolute top-1/2 left-20 w-12 h-12 bg-purple-300/20 rounded-full floating" style="animation-delay: 1.5s;"></div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-4">
                    Our <span class="text-gradient">Services</span>
                </h2>
                <p class="text-xl text-gray-600 max-w-2xl mx-auto">
                    We offer comprehensive digital solutions to transform your ideas into powerful online experiences
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Web Development -->
                <div class="service-card card-hover bg-gradient-to-br from-blue-50 to-indigo-100 p-8 rounded-2xl">
                    <div class="service-icon w-16 h-16 bg-blue-500 rounded-xl flex items-center justify-center mb-6">
                        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"></path>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">Web Development</h3>
                    <p class="text-gray-600 mb-6">Custom websites built with modern technologies, responsive design, and optimized performance for all devices.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Responsive Design</li>
                        <li>• Modern Frameworks</li>
                        <li>• SEO Optimized</li>
                        <li>• Fast Loading</li>
                    </ul>
                </div>

                <!-- Web Design -->
                <div class="service-card card-hover bg-gradient-to-br from-purple-50 to-pink-100 p-8 rounded-2xl">
                    <div class="service-icon w-16 h-16 bg-purple-500 rounded-xl flex items-center justify-center mb-6">
                        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 21a4 4 0 01-4-4V5a2 2 0 012-2h4a2 2 0 012 2v12a4 4 0 01-4 4zM21 5a2 2 0 00-2-2h-4a2 2 0 00-2 2v12a4 4 0 004 4h4a2 2 0 002-2V5z"></path>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">Web Design</h3>
                    <p class="text-gray-600 mb-6">Beautiful, user-friendly designs that capture your brand essence and provide exceptional user experiences.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• UI/UX Design</li>
                        <li>• Brand Identity</li>
                        <li>• Prototyping</li>
                        <li>• User Research</li>
                    </ul>
                </div>

                <!-- Application Building -->
                <div class="service-card card-hover bg-gradient-to-br from-green-50 to-emerald-100 p-8 rounded-2xl">
                    <div class="service-icon w-16 h-16 bg-green-500 rounded-xl flex items-center justify-center mb-6">
                        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z"></path>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">Application Building</h3>
                    <p class="text-gray-600 mb-6">Custom web applications tailored to your business needs with robust functionality and scalable architecture.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Custom Solutions</li>
                        <li>• Database Integration</li>
                        <li>• API Development</li>
                        <li>• Cloud Deployment</li>
                    </ul>
                </div>

                <!-- E-commerce Solutions -->
                <div class="service-card card-hover bg-gradient-to-br from-orange-50 to-red-100 p-8 rounded-2xl">
                    <div class="service-icon w-16 h-16 bg-orange-500 rounded-xl flex items-center justify-center mb-6">
                        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 11V7a4 4 0 00-8 0v4M5 9h14l1 12H4L5 9z"></path>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">E-commerce Solutions</h3>
                    <p class="text-gray-600 mb-6">Complete online stores with secure payment integration, inventory management, and customer analytics.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Payment Integration</li>
                        <li>• Inventory Management</li>
                        <li>• Order Tracking</li>
                        <li>• Analytics Dashboard</li>
                    </ul>
                </div>

                <!-- Maintenance & Support -->
                <div class="service-card card-hover bg-gradient-to-br from-teal-50 to-cyan-100 p-8 rounded-2xl">
                    <div class="service-icon w-16 h-16 bg-teal-500 rounded-xl flex items-center justify-center mb-6">
                        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z"></path>
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"></path>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">Maintenance & Support</h3>
                    <p class="text-gray-600 mb-6">Ongoing support, updates, and maintenance to keep your digital assets running smoothly and securely.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Regular Updates</li>
                        <li>• Security Monitoring</li>
                        <li>• Performance Optimization</li>
                        <li>• 24/7 Support</li>
                    </ul>
                </div>

                <!-- Custom Solutions -->
                <div class="service-card card-hover bg-gradient-to-br from-yellow-50 to-amber-100 p-8 rounded-2xl">
                    <div class="service-icon w-16 h-16 bg-yellow-500 rounded-xl flex items-center justify-center mb-6">
                        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path>
                        </svg>
                    </div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">Custom Solutions</h3>
                    <p class="text-gray-600 mb-6">Unique digital solutions crafted specifically for your business requirements and industry challenges.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li>• Tailored Development</li>
                        <li>• Industry Specific</li>
                        <li>• Scalable Architecture</li>
                        <li>• Integration Ready</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Reviews Section -->
    <section id="reviews" class="py-20 gradient-bg relative overflow-hidden">
        <div class="absolute inset-0 bg-black/10"></div>
        <div class="relative z-10 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-bold text-white mb-4">
                    Client <span class="text-yellow-300">Reviews</span>
                </h2>
                <p class="text-xl text-gray-200 max-w-2xl mx-auto">
                    See what our satisfied clients have to say about our work
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Review 1 -->
                <div class="review-card p-8 rounded-2xl card-hover">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 bg-gradient-to-r from-blue-400 to-purple-500 rounded-full flex items-center justify-center text-white font-bold text-lg">
                            P
                        </div>
                        <div class="ml-4">
                            <h4 class="text-white font-semibold">Priya Sharma</h4>
                            <p class="text-gray-300 text-sm">CEO, TechStart India</p>
                        </div>
                    </div>
                    <div class="flex mb-4">
                        <span class="text-yellow-400">★★★★★</span>
                    </div>
                    <p class="text-gray-200">
                        "Nova Creations delivered an exceptional website that exceeded our expectations. The design is modern, responsive, and perfectly captures our brand identity. Highly recommended!"
                    </p>
                </div>

                <!-- Review 2 -->
                <div class="review-card p-8 rounded-2xl card-hover">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 bg-gradient-to-r from-green-400 to-blue-500 rounded-full flex items-center justify-center text-white font-bold text-lg">
                            A
                        </div>
                        <div class="ml-4">
                            <h4 class="text-white font-semibold">Arjun Patel</h4>
                            <p class="text-gray-300 text-sm">Founder, Digital Solutions</p>
                        </div>
                    </div>
                    <div class="flex mb-4">
                        <span class="text-yellow-400">★★★★★</span>
                    </div>
                    <p class="text-gray-200">
                        "Outstanding work! The custom application they built for us has streamlined our operations significantly. Professional, timely, and excellent communication throughout."
                    </p>
                </div>

                <!-- Review 3 -->
                <div class="review-card p-8 rounded-2xl card-hover">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 bg-gradient-to-r from-purple-400 to-pink-500 rounded-full flex items-center justify-center text-white font-bold text-lg">
                            K
                        </div>
                        <div class="ml-4">
                            <h4 class="text-white font-semibold">Kavya Singh</h4>
                            <p class="text-gray-300 text-sm">Marketing Director, Creative Agency</p>
                        </div>
                    </div>
                    <div class="flex mb-4">
                        <span class="text-yellow-400">★★★★★</span>
                    </div>
                    <p class="text-gray-200">
                        "The e-commerce platform they developed has boosted our online sales by 300%. The user experience is seamless, and the admin panel is incredibly user-friendly."
                    </p>
                </div>

                <!-- Review 4 -->
                <div class="review-card p-8 rounded-2xl card-hover">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 bg-gradient-to-r from-orange-400 to-red-500 rounded-full flex items-center justify-center text-white font-bold text-lg">
                            R
                        </div>
                        <div class="ml-4">
                            <h4 class="text-white font-semibold">Rajesh Kumar</h4>
                            <p class="text-gray-300 text-sm">Restaurant Owner</p>
                        </div>
                    </div>
                    <div class="flex mb-4">
                        <span class="text-yellow-400">★★★★★</span>
                    </div>
                    <p class="text-gray-200">
                        "They created a beautiful website for our restaurant with online ordering functionality. Our customers love it, and we've seen a significant increase in orders!"
                    </p>
                </div>

                <!-- Review 5 -->
                <div class="review-card p-8 rounded-2xl card-hover">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 bg-gradient-to-r from-teal-400 to-green-500 rounded-full flex items-center justify-center text-white font-bold text-lg">
                            S
                        </div>
                        <div class="ml-4">
                            <h4 class="text-white font-semibold">Sneha Gupta</h4>
                            <p class="text-gray-300 text-sm">Fitness Coach</p>
                        </div>
                    </div>
                    <div class="flex mb-4">
                        <span class="text-yellow-400">★★★★★</span>
                    </div>
                    <p class="text-gray-200">
                        "Amazing work on my fitness coaching website! The booking system works flawlessly, and the design perfectly represents my brand. Thank you for bringing my vision to life!"
                    </p>
                </div>

                <!-- Review 6 -->
                <div class="review-card p-8 rounded-2xl card-hover">
                    <div class="flex items-center mb-6">
                        <div class="w-12 h-12 bg-gradient-to-r from-indigo-400 to-purple-500 rounded-full flex items-center justify-center text-white font-bold text-lg">
                            V
                        </div>
                        <div class="ml-4">
                            <h4 class="text-white font-semibold">Vikram Mehta</h4>
                            <p class="text-gray-300 text-sm">Real Estate Agent</p>
                        </div>
                    </div>
                    <div class="flex mb-4">
                        <span class="text-yellow-400">★★★★★</span>
                    </div>
                    <p class="text-gray-200">
                        "The property listing website they built has transformed my business. The search functionality is excellent, and the mobile experience is top-notch. Highly professional team!"
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid lg:grid-cols-2 gap-16 items-center">
                <div>
                    <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-8">
                        About the <span class="text-gradient">Founder</span>
                    </h2>
                    <div class="space-y-6 text-lg text-gray-600 leading-relaxed">
                        <p>
                            <strong class="text-gray-800">Astik Sharma</strong>, the founder of Nova Creations Codes, is a passionate web developer and visionary entrepreneur dedicated to creating impactful digital experiences.
                        </p>
                        <p>
                            With a focus on innovation, creativity, and precision, Astik believes in delivering technology that not only works but inspires. His mission is to empower businesses and individuals by providing elegant, functional, and affordable digital solutions.
                        </p>
                        <p>
                            Every project is approached with meticulous attention to detail, ensuring that each client receives a unique solution tailored to their specific needs and goals.
                        </p>
                    </div>
                    <div class="mt-8 flex flex-wrap gap-4">
                        <div class="bg-blue-50 px-4 py-2 rounded-full">
                            <span class="text-blue-600 font-medium">Web Development</span>
                        </div>
                        <div class="bg-purple-50 px-4 py-2 rounded-full">
                            <span class="text-purple-600 font-medium">UI/UX Design</span>
                        </div>
                        <div class="bg-green-50 px-4 py-2 rounded-full">
                            <span class="text-green-600 font-medium">Custom Solutions</span>
                        </div>
                        <div class="bg-orange-50 px-4 py-2 rounded-full">
                            <span class="text-orange-600 font-medium">Innovation</span>
                        </div>
                    </div>
                </div>
                <div class="relative">
                    <div class="w-full h-96 bg-gradient-to-br from-purple-100 to-blue-100 rounded-3xl flex items-center justify-center relative overflow-hidden">
                        <div class="text-center">
                            <div class="w-32 h-32 bg-gradient-to-br from-purple-500 to-blue-600 rounded-full flex items-center justify-center mb-6 mx-auto">
                                <span class="text-4xl font-bold text-white">AS</span>
                            </div>
                            <h3 class="text-2xl font-bold text-gray-800 mb-2">Astik Sharma</h3>
                            <p class="text-purple-600 font-medium">Founder & Lead Developer</p>
                        </div>
                        <!-- Decorative elements -->
                        <div class="absolute top-4 right-4 w-16 h-16 bg-yellow-300/20 rounded-full floating"></div>
                        <div class="absolute bottom-4 left-4 w-12 h-12 bg-purple-300/20 rounded-full floating" style="animation-delay: 0.5s;"></div>
                        <div class="absolute top-1/2 right-8 w-8 h-8 bg-blue-300/20 rounded-full floating" style="animation-delay: 1s;"></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Terms and Conditions Section -->
    <section id="terms" class="py-20 bg-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-4">
                    Terms & <span class="text-gradient">Conditions</span>
                </h2>
                <p class="text-xl text-gray-600">
                    Please read these terms carefully before engaging our services
                </p>
            </div>
            
            <div class="bg-gray-50 rounded-2xl p-8 space-y-8">
                <div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">1. Service Agreement</h3>
                    <p class="text-gray-600 leading-relaxed">
                        By engaging Nova Creations Codes for web development, design, or custom solutions, you agree to these terms and conditions. All projects require a signed agreement and advance payment as specified in the project proposal.
                    </p>
                </div>
                
                <div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">2. Payment Terms</h3>
                    <ul class="text-gray-600 space-y-2 leading-relaxed">
                        <li>• 50% advance payment required to start any project</li>
                        <li>• Remaining 50% due upon project completion and delivery</li>
                        <li>• Additional features or scope changes will be billed separately</li>
                        <li>• All payments are non-refundable once work has commenced</li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">3. Project Timeline</h3>
                    <p class="text-gray-600 leading-relaxed">
                        Project timelines are estimates based on project scope and complexity. Delays may occur due to client feedback cycles, content provision delays, or scope changes. We commit to transparent communication throughout the development process.
                    </p>
                </div>
                
                <div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">4. Intellectual Property</h3>
                    <p class="text-gray-600 leading-relaxed">
                        Upon full payment, clients receive full ownership of the final delivered product. However, Nova Creations Codes retains the right to showcase completed work in our portfolio and marketing materials unless otherwise specified in writing.
                    </p>
                </div>
                
                <div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">5. Support & Maintenance</h3>
                    <p class="text-gray-600 leading-relaxed">
                        We provide 30 days of free support for bug fixes after project delivery. Ongoing maintenance, updates, and new feature requests are available under separate maintenance agreements with competitive pricing.
                    </p>
                </div>
                
                <div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">6. Limitation of Liability</h3>
                    <p class="text-gray-600 leading-relaxed">
                        Nova Creations Codes' liability is limited to the total amount paid for the specific project. We are not responsible for any indirect, incidental, or consequential damages arising from the use of our services or delivered products.
                    </p>
                </div>
                
                <div class="bg-white p-6 rounded-xl border-l-4 border-purple-500">
                    <p class="text-gray-700 font-medium">
                        <strong>Contact for Clarifications:</strong> If you have any questions about these terms, please contact us before starting your project. We're here to ensure a smooth and transparent working relationship.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-4">
                    Get in <span class="text-gradient">Touch</span>
                </h2>
                <p class="text-xl text-gray-600 max-w-2xl mx-auto">
                    Ready to bring your ideas to life? Let's discuss your project and create something amazing together.
                </p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8 max-w-4xl mx-auto">
                <!-- WhatsApp -->
                <div class="text-center">
                    <div class="contact-btn bg-green-500 hover:bg-green-600 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-6 cursor-pointer" onclick="openWhatsApp()">
                        <svg class="w-10 h-10 text-white" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893A11.821 11.821 0 0020.885 3.488"/>
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-800 mb-2">WhatsApp</h3>
                    <p class="text-gray-600 mb-4">Quick chat and instant support</p>
                    <p class="text-lg font-semibold text-green-600">+91 6260943446</p>
                </div>

                <!-- Instagram -->
                <div class="text-center">
                    <div class="contact-btn bg-gradient-to-r from-purple-500 to-pink-500 hover:from-purple-600 hover:to-pink-600 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-6 cursor-pointer" onclick="openInstagram()">
                        <svg class="w-10 h-10 text-white" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/>
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-800 mb-2">Instagram</h3>
                    <p class="text-gray-600 mb-4">Follow our latest work</p>
                    <p class="text-lg font-semibold text-purple-600">@the_nova_creations_</p>
                </div>

                <!-- Email -->
                <div class="text-center">
                    <div class="contact-btn bg-blue-500 hover:bg-blue-600 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-6 cursor-pointer" onclick="openEmail()">
                        <svg class="w-10 h-10 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-800 mb-2">Email</h3>
                    <p class="text-gray-600 mb-4">Professional inquiries</p>
                    <p class="text-lg font-semibold text-blue-600">ashuv6131@gmail.com</p>
                </div>
            </div>

            <!-- Call to Action -->
            <div class="text-center mt-16">
                <div class="bg-white p-8 rounded-2xl shadow-lg max-w-2xl mx-auto">
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">Ready to Start Your Project?</h3>
                    <p class="text-gray-600 mb-6">Let's discuss your ideas and create something extraordinary together. Get in touch today!</p>
                    <button onclick="openWhatsApp()" class="bg-gradient-to-r from-purple-600 to-blue-600 hover:from-purple-700 hover:to-blue-700 text-white px-8 py-4 rounded-full font-semibold text-lg transition-all duration-300 pulse-glow">
                        Start Your Project Now
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-4 gap-8">
                <div class="md:col-span-2">
                    <div class="flex items-center space-x-3 mb-4">
                        <div class="w-10 h-10 gradient-bg rounded-lg flex items-center justify-center">
                            <span class="text-white font-bold text-xl">N</span>
                        </div>
                        <span class="text-xl font-bold">Nova Creations Codes</span>
                    </div>
                    <p class="text-gray-400 mb-6 max-w-md">
                        Building Ideas into Reality. Professional web development, stunning designs, and custom solutions that bring your vision to life.
                    </p>
                    <div class="flex space-x-4">
                        <button onclick="openWhatsApp()" class="w-10 h-10 bg-green-500 hover:bg-green-600 rounded-full flex items-center justify-center transition-colors">
                            <svg class="w-5 h-5 text-white" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893A11.821 11.821 0 0020.885 3.488"/>
                            </svg>
                        </button>
                        <button onclick="openInstagram()" class="w-10 h-10 bg-gradient-to-r from-purple-500 to-pink-500 hover:from-purple-600 hover:to-pink-600 rounded-full flex items-center justify-center transition-all">
                            <svg class="w-5 h-5 text-white" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/>
                            </svg>
                        </button>
                        <button onclick="openEmail()" class="w-10 h-10 bg-blue-500 hover:bg-blue-600 rounded-full flex items-center justify-center transition-colors">
                            <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
                            </svg>
                        </button>
                    </div>
                </div>
                
                <div>
                    <h4 class="text-lg font-semibold mb-4">Services</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li><a href="#services" class="hover:text-white transition-colors">Web Development</a></li>
                        <li><a href="#services" class="hover:text-white transition-colors">Web Design</a></li>
                        <li><a href="#services" class="hover:text-white transition-colors">Applications</a></li>
                        <li><a href="#services" class="hover:text-white transition-colors">Custom Solutions</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-semibold mb-4">Quick Links</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li><a href="#home" class="hover:text-white transition-colors">Home</a></li>
                        <li><a href="#about" class="hover:text-white transition-colors">About</a></li>
                        <li><a href="#reviews" class="hover:text-white transition-colors">Reviews</a></li>
                        <li><a href="#terms" class="hover:text-white transition-colors">Terms</a></li>
                        <li><a href="#contact" class="hover:text-white transition-colors">Contact</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 text-center">
                <p class="text-gray-400">© 2025 Nova Creations Codes. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Floating WhatsApp Button -->
    <div class="fixed bottom-6 right-6 z-50">
        <button onclick="openWhatsApp()" class="bg-green-500 hover:bg-green-600 w-16 h-16 rounded-full flex items-center justify-center shadow-lg hover:shadow-xl transition-all duration-300 pulse-glow group">
            <svg class="w-8 h-8 text-white group-hover:scale-110 transition-transform" fill="currentColor" viewBox="0 0 24 24">
                <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893A11.821 11.821 0 0020.885 3.488"/>
            </svg>
        </button>
        <div class="absolute -top-12 right-0 bg-gray-800 text-white px-3 py-1 rounded-lg text-sm opacity-0 group-hover:opacity-100 transition-opacity whitespace-nowrap">
            Chat with us!
        </div>
    </div>

    <script>
        // Mobile menu toggle
        function toggleMobileMenu() {
            const mobileMenu = document.getElementById('mobileMenu');
            mobileMenu.classList.toggle('hidden');
        }

        // Contact functions
        function openWhatsApp() {
            window.open('https://wa.me/916260943446', '_blank', 'noopener,noreferrer');
        }

        function openInstagram() {
            window.open('https://instagram.com/the_nova_creations_', '_blank', 'noopener,noreferrer');
        }

        function openEmail() {
            window.open('mailto:ashuv6131@gmail.com', '_blank', 'noopener,noreferrer');
        }

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                    // Close mobile menu if open
                    document.getElementById('mobileMenu').classList.add('hidden');
                }
            });
        });

        // Add scroll effect to navigation
        window.addEventListener('scroll', function() {
            const nav = document.querySelector('nav');
            if (window.scrollY > 100) {
                nav.classList.add('bg-white/95');
                nav.classList.remove('bg-white/90');
            } else {
                nav.classList.add('bg-white/90');
                nav.classList.remove('bg-white/95');
            }
        });

        // Intersection Observer for animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('fade-in');
                }
            });
        }, observerOptions);

        // Observe elements for animation
        document.addEventListener('DOMContentLoaded', function() {
            const animateElements = document.querySelectorAll('.card-hover, .service-card, .review-card');
            animateElements.forEach(el => {
                observer.observe(el);
            });
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9864705b90374844',t:'MTc1OTA3NTA3Ni4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
