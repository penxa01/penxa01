<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Juan Peña | GitHub Profile</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #0f172a;
            color: #e2e8f0;
        }
        
        .profile-img {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
        
        .skill-card {
            transition: all 0.3s ease;
            background: rgba(15, 23, 42, 0.7);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .skill-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
            border-color: #3b82f6;
        }
        
        .social-icon {
            transition: all 0.3s ease;
        }
        
        .social-icon:hover {
            transform: scale(1.1);
        }
        
        .section-title {
            position: relative;
            display: inline-block;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 100%;
            height: 3px;
            background: linear-gradient(90deg, #3b82f6, #8b5cf6);
            border-radius: 3px;
        }
        
        .neon-text {
            text-shadow: 0 0 5px #3b82f6, 0 0 10px #3b82f6;
        }
        
        @media (max-width: 768px) {
            .skill-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }
    </style>
</head>
<body class="min-h-screen">
    <div class="container mx-auto px-4 py-8 max-w-6xl">
        <!-- Header Section -->
        <header class="flex flex-col items-center justify-center text-center mb-12">
            <div class="profile-img w-32 h-32 rounded-full overflow-hidden border-4 border-blue-500 mb-4">
                <img src="https://cdn.dribbble.com/users/1787323/screenshots/10091971/media/d43c019bfeff34be8816481e843ea8c1.png" alt="Profile Image" class="w-full h-full object-cover">
            </div>
            <h1 class="text-4xl md:text-5xl font-bold mb-2 neon-text">Juan Peña <span class="wave text-3xl">👋</span></h1>
            <h2 class="text-xl md:text-2xl text-blue-400 mb-4">Student at Universidad Nacional de San Juan</h2>
            
            <div class="max-w-2xl mx-auto text-gray-300">
                <p class="mb-4">🌱 Currently learning <span class="font-semibold text-blue-300">to be a better programmer</span></p>
                <p class="mb-4">⚡ Fun fact: <span class="font-semibold text-purple-300">Coding and gaming are my passion</span></p>
                <p class="text-lg">🧔 Learning to be a web developer</p>
            </div>
        </header>

        <!-- Knowledge Base Section -->
        <section class="mb-16">
            <h2 class="section-title text-3xl font-bold mb-8 text-center">Knowledge Base</h2>
            
            <div class="flex justify-center mb-12">
                <img src="https://raw.githubusercontent.com/Elanza-48/Elanza-48/41a4790484e268102dfdab2b7c59d440d3ffafab/resources/img/coders-prog.gif" alt="Coding Animation" class="rounded-lg max-w-full md:max-w-2xl">
            </div>
            
            <!-- Languages Section -->
            <div class="mb-12">
                <h3 class="text-2xl font-semibold mb-6 text-center text-blue-300">Languages</h3>
                <div class="skill-grid grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
                    <a href="https://www.python.org/" target="_blank" class="skill-card rounded-lg p-4 flex flex-col items-center">
                        <i class="fab fa-python text-4xl text-blue-400 mb-2"></i>
                        <span class="font-medium">Python</span>
                    </a>
                    
                    <a href="https://en.cppreference.com/w/" target="_blank" class="skill-card rounded-lg p-4 flex flex-col items-center">
                        <i class="fas fa-code text-4xl text-purple-400 mb-2"></i>
                        <span class="font-medium">C++</span>
                    </a>
                    
                    <a href="https://www.java.com/" target="_blank" class="skill-card rounded-lg p-4 flex flex-col items-center">
                        <i class="fab fa-java text-4xl text-red-400 mb-2"></i>
                        <span class="font-medium">Java</span>
                    </a>
                    
                    <a href="https://www.swi-prolog.org/" target="_blank" class="skill-card rounded-lg p-4 flex flex-col items-center">
                        <i class="fas fa-brain text-4xl text-yellow-400 mb-2"></i>
                        <span class="font-medium">Prolog</span>
                    </a>
                    
                    <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" class="skill-card rounded-lg p-4 flex flex-col items-center">
                        <i class="fab fa-js text-4xl text-yellow-300 mb-2"></i>
                        <span class="font-medium">JavaScript</span>
                    </a>
                </div>
            </div>
            
            <!-- Frontend Section -->
            <div class="mb-12">
                <h3 class="text-2xl font-semibold mb-6 text-center text-blue-300">Frontend</h3>
                <div class="skill-grid grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
                    <a href="https://developer.mozilla.org/en-US/docs/Web/HTML" target="_blank" class="skill-card rounded-lg p-4 flex flex-col items-center">
                        <i class="fab fa-html5 text-4xl text-orange-500 mb-2"></i>
                        <span class="font-medium">HTML</span>
                    </a>
                </div>
            </div>
            
            <!-- Database Section -->
            <div class="mb-12">
                <h3 class="text-2xl font-semibold mb-6 text-center text-blue-300">Database</h3>
                <div class="skill-grid grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
                    <a href="https://www.w3schools.com/sql/" target="_blank" class="skill-card rounded-lg p-4 flex flex-col items-center">
                        <i class="fas fa-database text-4xl text-blue-300 mb-2"></i>
                        <span class="font-medium">SQL</span>
                    </a>
                    
                    <a href="https://www.postgresql.org/" target="_blank" class="skill-card rounded-lg p-4 flex flex-col items-center">
                        <i class="fas fa-server text-4xl text-blue-400 mb-2"></i>
                        <span class="font-medium">PostgreSQL</span>
                    </a>
                </div>
            </div>
            
            <!-- IDE Section -->
            <div>
                <h3 class="text-2xl font-semibold mb-6 text-center text-blue-300">Preferred IDEs</h3>
                <div class="skill-grid grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
                    <a href="https://code.visualstudio.com/" target="_blank" class="skill-card rounded-lg p-4 flex flex-col items-center">
                        <i class="fas fa-code text-4xl text-blue-500 mb-2"></i>
                        <span class="font-medium">VS Code</span>
                    </a>
                </div>
            </div>
        </section>

        <!-- Connect Section -->
        <section class="mb-16">
            <h2 class="section-title text-3xl font-bold mb-8 text-center">Connect With Me</h2>
            
            <div class="flex flex-wrap justify-center gap-6 mb-8">
                <a href="https://www.instagram.com/_penxa01/" target="_blank" class="social-icon w-16 h-16 rounded-full bg-gradient-to-br from-pink-500 to-purple-600 flex items-center justify-center text-white hover:shadow-lg hover:shadow-pink-500/30">
                    <i class="fab fa-instagram text-2xl"></i>
                </a>
                
                <a href="https://x.com/Penxa01" target="_blank" class="social-icon w-16 h-16 rounded-full bg-gradient-to-br from-blue-400 to-blue-600 flex items-center justify-center text-white hover:shadow-lg hover:shadow-blue-500/30">
                    <i class="fab fa-twitter text-2xl"></i>
                </a>
                
                <a href="https://www.linkedin.com/in/juan-pe%C3%B1a-b543771ba/" target="_blank" class="social-icon w-16 h-16 rounded-full bg-gradient-to-br from-blue-600 to-blue-800 flex items-center justify-center text-white hover:shadow-lg hover:shadow-blue-500/30">
                    <i class="fab fa-linkedin-in text-2xl"></i>
                </a>
                
                <a href="mailto:pepino199582@gmail.com" class="social-icon w-16 h-16 rounded-full bg-gradient-to-br from-red-500 to-red-600 flex items-center justify-center text-white hover:shadow-lg hover:shadow-red-500/30">
                    <i class="fas fa-envelope text-2xl"></i>
                </a>
            </div>
        </section>

        <!-- GitHub Stats Section -->
        <section class="mb-16">
            <h2 class="section-title text-3xl font-bold mb-8 text-center">GitHub Stats</h2>
            
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <div class="bg-gray-800 rounded-lg p-4">
                    <img src="https://github-readme-stats.vercel.app/api?username=penxa01&show_icons=true&theme=tokyonight&hide_border=true&locale=en" alt="GitHub Stats" class="w-full">
                </div>
                
                <div class="bg-gray-800 rounded-lg p-4">
                    <img src="https://github-readme-streak-stats.herokuapp.com/?user=penxa01&theme=material-palenight" alt="GitHub Streak" class="w-full">
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer class="text-center text-gray-400 py-6 border-t border-gray-800">
            <div class="mb-4">
                <img src="https://raw.githubusercontent.com/Elanza-48/Elanza-48/main/resources/img/github-contribution-grid-snake.svg" alt="GitHub Snake" class="w-full max-w-2xl mx-auto">
            </div>
            <p>© 2023 Juan Peña | <a href="https://github.com/penxa01" target="_blank" class="text-blue-400 hover:underline">GitHub Profile</a></p>
        </footer>
    </div>

    <script>
        // Simple animation for the wave emoji
        const wave = document.querySelector('.wave');
        let rotation = 0;
        
        setInterval(() => {
            rotation = (rotation + 2) % 360;
            wave.style.transform = `rotate(${rotation}deg)`;
        }, 100);
    </script>
</body>
</html>
