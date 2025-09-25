<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chauhan Harit - Computer Engineering Student</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }
        
        .hero-pattern {
            background-image: radial-gradient(circle at 1px 1px, rgba(255,255,255,0.1) 1px, transparent 0);
            background-size: 20px 20px;
        }
        
        .card-hover {
            transition: all 0.3s ease;
            transform: translateY(0);
        }
        
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        
        .typewriter {
            overflow: hidden;
            border-right: .15em solid #764ba2;
            white-space: nowrap;
            margin: 0 auto;
            letter-spacing: .15em;
            animation: typing 3.5s steps(40, end), blink-caret .75s step-end infinite;
        }
        
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        
        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #764ba2 }
        }
        
        .floating {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }
    </style>
</head>
<body class="min-h-screen text-white">
    <!-- Navigation -->
    <nav class="fixed w-full bg-white bg-opacity-10 backdrop-blur-md z-50 py-4 px-6 shadow-lg">
        <div class="container mx-auto flex justify-between items-center">
            <div class="text-2xl font-bold text-white">
                <span class="bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent">CH</span>
            </div>
            <div class="hidden md:flex space-x-8">
                <a href="#home" class="hover:text-purple-300 transition-colors">Home</a>
                <a href="#about" class="hover:text-purple-300 transition-colors">About</a>
                <a href="#education" class="hover:text-purple-300 transition-colors">Education</a>
                <a href="#contact" class="hover:text-purple-300 transition-colors">Contact</a>
            </div>
            <div class="md:hidden">
                <button id="menu-btn" class="text-white">
                    <i class="fas fa-bars text-2xl"></i>
                </button>
            </div>
        </div>
    </nav>

    <!-- Mobile Menu -->
    <div id="mobile-menu" class="fixed top-0 right-0 h-full w-64 bg-gray-900 bg-opacity-95 backdrop-blur-md transform translate-x-full transition-transform duration-300 z-50 md:hidden">
        <div class="p-6">
            <button id="close-menu" class="absolute top-4 right-4 text-white text-2xl">
                <i class="fas fa-times"></i>
            </button>
            <div class="mt-16 space-y-6">
                <a href="#home" class="block text-xl hover:text-purple-300 transition-colors">Home</a>
                <a href="#about" class="block text-xl hover:text-purple-300 transition-colors">About</a>
                <a href="#education" class="block text-xl hover:text-purple-300 transition-colors">Education</a>
                <a href="#contact" class="block text-xl hover:text-purple-300 transition-colors">Contact</a>
            </div>
        </div>
    </div>

    <!-- Hero Section -->
    <section id="home" class="min-h-screen flex items-center justify-center pt-20 px-4 hero-pattern">
        <div class="container mx-auto text-center">
            <div class="floating mb-8">
                <img src="6c379be2-2142-45bd-b4d4-732ea3c054b5.jpg" alt="" class="w-48 h-48 rounded-full mx-auto border-4 border-white border-opacity-30 shadow-2xl">
            </div>
            <h1 class="text-4xl md:text-6xl font-bold mb-4">
                Chauhan <span class="bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent">Harit</span>
            </h1>
            <div class="typewriter text-xl md:text-2xl mb-6">
                Computer Engineering Student
            </div>
            <p class="text-lg md:text-xl mb-8 max-w-2xl mx-auto opacity-90">
                Passionate about technology, programming, and building innovative solutions for the digital world.
            </p>
            <div class="flex justify-center space-x-4">
                <a href="#about" class="bg-white text-purple-600 px-8 py-3 rounded-full font-semibold hover:bg-purple-100 transition-colors">
                    Know More
                </a>
                <a href="#contact" class="border-2 border-white border-opacity-30 text-white px-8 py-3 rounded-full font-semibold hover:bg-white hover:bg-opacity-10 transition-colors">
                    Get in Touch
                </a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 px-4 bg-white bg-opacity-5">
        <div class="container mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-16">
                About <span class="bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent">Me</span>
            </h2>
            
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div class="card-hover bg-white bg-opacity-10 backdrop-blur-md rounded-2xl p-8 shadow-xl">
                    <h3 class="text-2xl font-semibold mb-6">Personal Details</h3>
                    <div class="space-y-4">
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-purple-500 bg-opacity-20 rounded-full flex items-center justify-center mr-4">
                                <i class="fas fa-user text-purple-400"></i>
                            </div>
                            <div>
                                <p class="font-semibold">Name</p>
                                <p>Chauhan Harit</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-purple-500 bg-opacity-20 rounded-full flex items-center justify-center mr-4">
                                <i class="fas fa-birthday-cake text-purple-400"></i>
                            </div>
                            <div>
                                <p class="font-semibold">Age</p>
                                <p>17 Years</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-purple-500 bg-opacity-20 rounded-full flex items-center justify-center mr-4">
                                <i class="fas fa-map-marker-alt text-purple-400"></i>
                            </div>
                            <div>
                                <p class="font-semibold">Location</p>
                                <p>Vadali, Sabarkantha, Gujarat, India</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-purple-500 bg-opacity-20 rounded-full flex items-center justify-center mr-4">
                                <i class="fas fa-graduation-cap text-purple-400"></i>
                            </div>
                            <div>
                                <p class="font-semibold">Education</p>
                                <p>Diploma in Computer Engineering</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="card-hover bg-white bg-opacity-10 backdrop-blur-md rounded-2xl p-8 shadow-xl">
                    <h3 class="text-2xl font-semibold mb-6">My Journey</h3>
                    <p class="mb-4">
                        I am a passionate computer engineering student with a strong interest in technology and innovation. 
                        Currently pursuing my diploma, I'm constantly exploring new technologies and expanding my skills 
                        in programming and software development.
                    </p>
                    <p class="mb-4">
                        Hailing from the beautiful region of Sabarkantha in Gujarat, I bring the values of hard work and 
                        dedication to everything I do. My goal is to become a skilled software engineer and contribute 
                        to the ever-evolving tech industry.
                    </p>
                    <p>
                        When I'm not coding, I enjoy learning about new technologies, participating in tech communities, 
                        and working on personal projects that challenge my skills and creativity.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Education Section -->
    <section id="education" class="py-20 px-4">
        <div class="container mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-16">
                Education & <span class="bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent">Skills</span>
            </h2>
            
            <div class="grid md:grid-cols-2 gap-8">
                <div class="card-hover bg-white bg-opacity-10 backdrop-blur-md rounded-2xl p-8 shadow-xl">
                    <h3 class="text-2xl font-semibold mb-6">Education</h3>
                    <div class="space-y-6">
                        <div class="flex items-start">
                            <div class="w-16 h-16 bg-purple-500 bg-opacity-20 rounded-full flex items-center justify-center mr-4 mt-1">
                                <i class="fas fa-graduation-cap text-2xl text-purple-400"></i>
                            </div>
                            <div>
                                <h4 class="text-xl font-semibold">Diploma in Computer Engineering</h4>
                                <p class="text-purple-300">Currently Pursuing</p>
                                <p class="mt-2">Focusing on software development, hardware systems, and computer networking</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="card-hover bg-white bg-opacity-10 backdrop-blur-md rounded-2xl p-8 shadow-xl">
                    <h3 class="text-2xl font-semibold mb-6">Technical Skills</h3>
                    <div class="space-y-4">
                        <div>
                            <p class="font-semibold">Programming Languages</p>
                            <div class="flex flex-wrap gap-2 mt-2">
                                <span class="bg-purple-500 bg-opacity-20 px-3 py-1 rounded-full">Java</span>
                                <span class="bg-purple-500 bg-opacity-20 px-3 py-1 rounded-full">Python</span>
                                <span class="bg-purple-500 bg-opacity-20 px-3 py-1 rounded-full">C++</span>
                                <span class="bg-purple-500 bg-opacity-20 px-3 py-1 rounded-full">JavaScript</span>
                            </div>
                        </div>
                        <div>
                            <p class="font-semibold">Web Development</p>
                            <div class="flex flex-wrap gap-2 mt-2">
                                <span class="bg-purple-500 bg-opacity-20 px-3 py-1 rounded-full">HTML/CSS</span>
                                <span class="bg-purple-500 bg-opacity-20 px-3 py-1 rounded-full">React</span>
                                <span class="bg-purple-500 bg-opacity-20 px-3 py-1 rounded-full">Node.js</span>
                            </div>
                        </div>
                        <div>
                            <p class="font-semibold">Tools & Technologies</p>
                            <div class="flex flex-wrap gap-2 mt-2">
                                <span class="bg-purple-500 bg-opacity-20 px-3 py-1 rounded-full">Git</span>
                                <span class="bg-purple-500 bg-opacity-20 px-3 py-1 rounded-full">VS Code</span>
                                <span class="bg-purple-500 bg-opacity-20 px-3 py-1 rounded-full">MySQL</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Location Section -->
    <section class="py-20 px-4 bg-white bg-opacity-5">
        <div class="container mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-16">
                My <span class="bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent">Location</span>
            </h2>
            
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div class="card-hover bg-white bg-opacity-10 backdrop-blur-md rounded-2xl p-8 shadow-xl">
                    <h3 class="text-2xl font-semibold mb-6">Vadali, Sabarkantha</h3>
                    <p class="mb-4">
                        I reside in the beautiful town of Vadali, located in the Sabarkantha district of Gujarat, India. 
                        This region is known for its rich cultural heritage and natural beauty.
                    </p>
                    <p class="mb-4">
                        Sabarkantha is situated in the northeastern part of Gujarat, bordering Rajasthan. 
                        The area is famous for its agricultural produce and is gradually developing into 
                        an emerging hub for education and technology.
                    </p>
                    <p>
                        Being from this region has instilled in me the values of community, hard work, and 
                        the importance of staying connected to one's roots while embracing technological progress.
                    </p>
                </div>
                
                <div class="card-hover overflow-hidden rounded-2xl shadow-xl">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/5b0faad6-2227-42a3-b0bc-27a236ab10ee.png" alt="Scenic view of Vadali town in Sabarkantha district showing traditional architecture and natural landscapes of Gujarat" class="w-full h-64 object-cover">
                    <div class="p-6 bg-white bg-opacity-10 backdrop-blur-md">
                        <h4 class="text-xl font-semibold mb-2">Gujarat, India</h4>
                        <p class="text-sm">Known for its vibrant culture, technological advancement, and entrepreneurial spirit</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 px-4">
        <div class="container mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-16">
                Get In <span class="bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent">Touch</span>
            </h2>
            
            <div class="max-w-2xl mx-auto">
                <div class="card-hover bg-white bg-opacity-10 backdrop-blur-md rounded-2xl p-8 shadow-xl">
                    <h3 class="text-2xl font-semibold mb-6 text-center">Let's Connect!</h3>
                    <p class="text-center mb-8">
                        I'm always interested in new opportunities, collaborations, and conversations about technology.
                    </p>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8">
                        <div class="flex items-center justify-center p-4 bg-white bg-opacity-10 rounded-xl">
                            <i class="fas fa-envelope text-2xl text-purple-400 mr-3"></i>
                            <span>harit.chauhan@email.com</span>
                        </div>
                        <div class="flex items-center justify-center p-4 bg-white bg-opacity-10 rounded-xl">
                            <i class="fas fa-phone text-2xl text-purple-400 mr-3"></i>
                            <span>+91 XXXXX XXXXX</span>
                        </div>
                    </div>
                    
                    <div class="flex justify-center space-x-6">
                        <a href="#" class="w-12 h-12 bg-white bg-opacity-10 rounded-full flex items-center justify-center hover:bg-purple-500 transition-colors">
                            <i class="fab fa-linkedin-in text-xl"></i>
                        </a>
                        <a href="#" class="w-12 h-12 bg-white bg-opacity-10 rounded-full flex items-center justify-center hover:bg-purple-500 transition-colors">
                            <i class="fab fa-github text-xl"></i>
                        </a>
                        <a href="#" class="w-12 h-12 bg-white bg-opacity-10 rounded-full flex items-center justify-center hover:bg-purple-500 transition-colors">
                            <i class="fab fa-twitter text-xl"></i>
                        </a>
                        <a href="#" class="w-12 h-12 bg-white bg-opacity-10 rounded-full flex items-center justify-center hover:bg-purple-500 transition-colors">
                            <i class="fab fa-instagram text-xl"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 bg-opacity-50 py-8 px-4">
        <div class="container mx-auto text-center">
            <p>© 2024 Chauhan Harit. All rights reserved.</p>
            <p class="mt-2 text-sm opacity-70">Computer Engineering Student | Vadali, Sabarkantha, Gujarat</p>
        </div>
    </footer>

    <script>
        // Mobile menu functionality
        const menuBtn = document.getElementById('menu-btn');
        const closeMenu = document.getElementById('close-menu');
        const mobileMenu = document.getElementById('mobile-menu');
        const menuLinks = document.querySelectorAll('#mobile-menu a');

        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.remove('translate-x-full');
        });

        closeMenu.addEventListener('click', () => {
            mobileMenu.classList.add('translate-x-full');
        });

        menuLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('translate-x-full');
            });
        });

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
                }
            });
        });

        // Add scroll animation
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('animate-fade-in');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.card-hover').forEach(card => {
            observer.observe(card);
        });
    </script>
</body>
</html>

