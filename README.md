<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ayanle Aideed - Full Stack/Backend Developer</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.9.1/gsap.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.9.1/ScrollTrigger.min.js"></script>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        h1, h2, h3 {
            color: #4CAF50;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
        }
        .hero {
            text-align: center;
            padding: 100px 0;
            background: url('/api/placeholder/1200/400') center/cover no-repeat;
            color: white;
            position: relative;
            overflow: hidden;
        }
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.5);
            z-index: 1;
        }
        .hero-content {
            position: relative;
            z-index: 2;
        }
        .animated-text {
            font-size: 2.5em;
            margin-bottom: 20px;
        }
        .skills {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin-top: 40px;
        }
        .skill-icon {
            width: 60px;
            height: 60px;
            transition: transform 0.3s ease;
        }
        .skill-icon:hover {
            transform: scale(1.2);
        }
        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin-top: 40px;
        }
        .project-card {
            background: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: transform 0.3s ease;
        }
        .project-card:hover {
            transform: translateY(-5px);
        }
        .project-image {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .project-info {
            padding: 20px;
        }
        .stats {
            display: flex;
            justify-content: space-around;
            margin-top: 40px;
        }
        .stat-item {
            text-align: center;
        }
        .stat-value {
            font-size: 2em;
            font-weight: bold;
            color: #4CAF50;
        }
        .connect {
            text-align: center;
            margin-top: 40px;
        }
        .social-icons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        .social-icon {
            font-size: 24px;
            color: #4CAF50;
            transition: color 0.3s ease;
        }
        .social-icon:hover {
            color: #45a049;
        }
        #codePlayers {
            margin-top: 40px;
        }
        .code-player {
            background: #f4f4f4;
            border-radius: 8px;
            padding: 20px;
            margin-bottom: 20px;
            position: relative;
            overflow: hidden;
        }
        .code-player pre {
            margin: 0;
            white-space: pre-wrap;
        }
        .play-button {
            position: absolute;
            top: 10px;
            right: 10px;
            background: #4CAF50;
            color: white;
            border: none;
            border-radius: 50%;
            width: 30px;
            height: 30px;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }
        .floating {
            animation: float 3s ease-in-out infinite;
        }
    </style>
</head>
<body>
    <div class="container">
        <section class="hero">
            <div class="hero-content">
                <h1 class="animated-text">Ayanle Aideed</h1>
                <p class="animated-text">Full Stack/Backend Developer</p>
            </div>
        </section>

        <section class="about">
            <h2>About Me</h2>
            <p>Passionate developer with expertise in full-stack and backend technologies. I love creating efficient, scalable solutions and continuously learning new technologies.</p>
        </section>

        <section class="skills">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" class="skill-icon floating">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript" class="skill-icon floating">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="Java" class="skill-icon floating">
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg" alt="C#" class="skill-icon floating">
            <img src="https://cdn.worldvectorlogo.com/logos/django.svg" alt="Django" class="skill-icon floating">
            <img src="https://www.vectorlogo.zone/logos/pocoo_flask/pocoo_flask-icon.svg" alt="Flask" class="skill-icon floating">
        </section>

        <section class="projects">
            <div class="project-card">
                <img src="/api/placeholder/300/200" alt="Project 1" class="project-image">
                <div class="project-info">
                    <h3>Project 1</h3>
                    <p>Description of Project 1</p>
                </div>
            </div>
            <div class="project-card">
                <img src="/api/placeholder/300/200" alt="Project 2" class="project-image">
                <div class="project-info">
                    <h3>Project 2</h3>
                    <p>Description of Project 2</p>
                </div>
            </div>
            <div class="project-card">
                <img src="/api/placeholder/300/200" alt="Project 3" class="project-image">
                <div class="project-info">
                    <h3>Project 3</h3>
                    <p>Description of Project 3</p>
                </div>
            </div>
        </section>

        <section class="stats">
            <div class="stat-item">
                <div class="stat-value" id="repoCount">0</div>
                <div>Repositories</div>
            </div>
            <div class="stat-item">
                <div class="stat-value" id="starsCount">0</div>
                <div>GitHub Stars</div>
            </div>
            <div class="stat-item">
                <div class="stat-value" id="contributionsCount">0</div>
                <div>Contributions</div>
            </div>
        </section>

        <section id="codePlayers">
            <h2>Code Snippets</h2>
            <div class="code-player">
                <pre><code class="language-python">
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)

print(fibonacci(10))
                </code></pre>
                <button class="play-button">▶</button>
            </div>
            <div class="code-player">
                <pre><code class="language-javascript">
const quickSort = (arr) => {
    if (arr.length <= 1) {
        return arr;
    }
    
    const pivot = arr[arr.length - 1];
    const left = [];
    const right = [];
    
    for (let i = 0; i < arr.length - 1; i++) {
        if (arr[i] < pivot) {
            left.push(arr[i]);
        } else {
            right.push(arr[i]);
        }
    }
    
    return [...quickSort(left), pivot, ...quickSort(right)];
};

console.log(quickSort([3, 6, 8, 10, 1, 2, 1]));
                </code></pre>
                <button class="play-button">▶</button>
            </div>
        </section>

        <section class="connect">
            <h2>Connect with me</h2>
            <div class="social-icons">
                <a href="https://github.com/ayanleaideed" target="_blank" class="social-icon">
                    <i class="fab fa-github"></i>
                </a>
                <a href="https://www.linkedin.com/in/ayanle-aideed-118752252/" target="_blank" class="social-icon">
                    <i class="fab fa-linkedin"></i>
                </a>
                <a href="https://ayanleaideed.github.io/myportfolio/" target="_blank" class="social-icon">
                    <i class="fas fa-globe"></i>
                </a>
            </div>
        </section>
    </div>

    <script>
        // Animations
        gsap.registerPlugin(ScrollTrigger);

        gsap.from('.hero-content', {
            opacity: 0,
            y: 50,
            duration: 1,
            ease: 'power3.out'
        });

        gsap.from('.skill-icon', {
            opacity: 0,
            scale: 0.5,
            duration: 0.5,
            stagger: 0.1,
            ease: 'back.out(1.7)',
            scrollTrigger: {
                trigger: '.skills',
                start: 'top 80%'
            }
        });

        gsap.from('.project-card', {
            opacity: 0,
            y: 50,
            duration: 0.8,
            stagger: 0.2,
            ease: 'power3.out',
            scrollTrigger: {
                trigger: '.projects',
                start: 'top 80%'
            }
        });

        // Stats counter animation
        const animateValue = (id, start, end, duration) => {
            const range = end - start;
            let current = start;
            const increment = end > start ? 1 : -1;
            const stepTime = Math.abs(Math.floor(duration / range));
            const obj = document.getElementById(id);
            const timer = setInterval(() => {
                current += increment;
                obj.innerHTML = current;
                if (current == end) {
                    clearInterval(timer);
                }
            }, stepTime);
        };

        ScrollTrigger.create({
            trigger: '.stats',
            start: 'top 80%',
            onEnter: () => {
                animateValue('repoCount', 0, 50, 2000);
                animateValue('starsCount', 0, 100, 2000);
                animateValue('contributionsCount', 0, 500, 2000);
            }
        });

        // Code player functionality
        document.querySelectorAll('.play-button').forEach(button => {
            button.addEventListener('click', function() {
                const code = this.previousElementSibling.textContent;
                // In a real implementation, you'd want to securely evaluate the code
                // For demonstration purposes, we'll just log it
                console.log('Executing code:', code);
                alert('Code executed! Check the console for output.');
            });
        });

        // Typewriter effect for the hero text
        const typewriter = (text, element, speed) => {
            let i = 0;
            const timer = setInterval(() => {
                if (i < text.length) {
                    element.innerHTML += text.charAt(i);
                    i++;
                } else {
                    clearInterval(timer);
                }
            }, speed);
        };

        typewriter('Full Stack/Backend Developer', document.querySelector('.hero-content p'), 100);
    </script>
