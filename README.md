<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jonel's GitHub Profile</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
            color: #f0f6fc;
            line-height: 1.6;
            padding: 20px;
            background-attachment: fixed;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            background: rgba(13, 17, 23, 0.85);
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.4);
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        header {
            text-align: center;
            padding: 30px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
            margin-bottom: 30px;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: #58a6ff;
            text-shadow: 0 0 10px rgba(88, 166, 255, 0.3);
        }
        
        .tagline {
            font-size: 1.2rem;
            color: #c9d1d9;
            margin-bottom: 20px;
        }
        
        .badges {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
            flex-wrap: wrap;
        }
        
        .badge {
            background: rgba(47, 129, 247, 0.15);
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 0.9rem;
            display: inline-flex;
            align-items: center;
            border: 1px solid rgba(88, 166, 255, 0.3);
        }
        
        .divider {
            height: 1px;
            background: linear-gradient(90deg, transparent, rgba(88, 166, 255, 0.5), transparent);
            margin: 30px 0;
        }
        
        h2 {
            color: #58a6ff;
            margin: 25px 0 15px;
            padding-bottom: 8px;
            border-bottom: 1px solid rgba(88, 166, 255, 0.3);
        }
        
        .about-content {
            background: rgba(22, 27, 34, 0.5);
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }
        
        .goals-list {
            list-style: none;
            padding: 15px;
            background: rgba(22, 27, 34, 0.5);
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }
        
        .goals-list li {
            margin-bottom: 12px;
            padding-left: 25px;
            position: relative;
        }
        
        .goals-list li:before {
            content: "•";
            color: #58a6ff;
            font-weight: bold;
            position: absolute;
            left: 10px;
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 15px;
            margin: 20px 0;
        }
        
        .skill-category {
            background: rgba(22, 27, 34, 0.5);
            padding: 15px;
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }
        
        .skill-category h3 {
            color: #58a6ff;
            margin-bottom: 12px;
            font-size: 1.1rem;
        }
        
        .skill-items {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }
        
        .skill-item {
            background: rgba(47, 129, 247, 0.15);
            padding: 5px 10px;
            border-radius: 15px;
            font-size: 0.85rem;
            border: 1px solid rgba(88, 166, 255, 0.3);
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }
        
        .project-card {
            background: rgba(22, 27, 34, 0.5);
            padding: 20px;
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: transform 0.3s ease;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            border-color: rgba(88, 166, 255, 0.3);
        }
        
        .project-card h3 {
            color: #58a6ff;
            margin-bottom: 10px;
        }
        
        .stats-container {
            display: flex;
            gap: 20px;
            margin: 20px 0;
            flex-wrap: wrap;
        }
        
        .stat {
            flex: 1;
            min-width: 250px;
            background: rgba(22, 27, 34, 0.5);
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }
        
        .contact-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 30px 0;
        }
        
        .contact-link {
            display: flex;
            align-items: center;
            gap: 8px;
            padding: 10px 20px;
            background: rgba(47, 129, 247, 0.15);
            border-radius: 8px;
            text-decoration: none;
            color: #58a6ff;
            border: 1px solid rgba(88, 166, 255, 0.3);
            transition: all 0.3s ease;
        }
        
        .contact-link:hover {
            background: rgba(47, 129, 247, 0.25);
            transform: translateY(-2px);
        }
        
        footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #8b949e;
        }
        
        @media (max-width: 768px) {
            .skills-grid {
                grid-template-columns: 1fr;
            }
            
            .stats-container {
                flex-direction: column;
            }
            
            .contact-links {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1><i class="fas fa-handshake"></i> Hi there, I'm Jonel</h1>
            <p class="tagline">I'm delighted to have this opportunity to introduce myself.</p>
            
            <div class="badges">
                <div class="badge">
                    <i class="fas fa-eye"></i> Profile Views: 128
                </div>
                <div class="badge">
                    <i class="fas fa-users"></i> Followers: 15
                </div>
                <div class="badge">
                    <i class="fas fa-star"></i> Stars: 28
                </div>
            </div>
        </header>
        
        <section>
            <h2><i class="fas fa-user-tie"></i> Professional Profile</h2>
            <div class="about-content">
                <p><i class="fas fa-graduation-cap"></i> <strong>BSIT Student</strong> • <strong>Laguna State Polytechnic University (LSPU)</strong></p>
                <p><i class="fas fa-book"></i> <strong>Currently learning:</strong> PHP • Python • SQL • HTML • CSS</p>
            </div>
        </section>
        
        <div class="divider"></div>
        
        <section>
            <h2><i class="fas fa-bullseye"></i> My Goals</h2>
            <ul class="goals-list">
                <li>Learn more to become a <strong>Web & Mobile Application Developer</strong></li>
                <li>Enhance skills in <strong>UI/UX</strong> using <strong>Figma & Adobe</strong></li>
                <li>Improve knowledge in <strong>Graphic Design</strong> using <strong>Photoshop</strong></li>
                <li>Interested in <strong>UI/UX Design</strong> and <strong>PHP Programming</strong></li>
            </ul>
        </section>
        
        <div class="divider"></div>
        
        <section>
            <h2><i class="fas fa-tools"></i> Skills</h2>
            <div class="skills-grid">
                <div class="skill-category">
                    <h3>Languages</h3>
                    <div class="skill-items">
                        <span class="skill-item">PHP</span>
                        <span class="skill-item">Python</span>
                        <span class="skill-item">SQL</span>
                        <span class="skill-item">HTML5</span>
                        <span class="skill-item">CSS3</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>Frameworks & Tools</h3>
                    <div class="skill-items">
                        <span class="skill-item">XAMPP</span>
                        <span class="skill-item">VS Code</span>
                        <span class="skill-item">Git</span>
                        <span class="skill-item">GitHub</span>
                        <span class="skill-item">Figma</span>
                        <span class="skill-item">Photoshop</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>Other Skills</h3>
                    <div class="skill-items">
                        <span class="skill-item">Database Management</span>
                        <span class="skill-item">Prototyping</span>
                        <span class="skill-item">Project Documentation</span>
                    </div>
                </div>
            </div>
        </section>
        
        <div class="divider"></div>
        
        <section>
            <h2><i class="fas fa-rocket"></i> Current Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <h3>Web-based Monitoring System</h3>
                    <p>For the Office of the Municipal Agriculturist</p>
                </div>
                
                <div class="project-card">
                    <h3>UI/UX Design Concepts</h3>
                    <p>Using Figma & Adobe XD</p>
                </div>
                
                <div class="project-card">
                    <h3>PHP & MySQL Projects</h3>
                    <p>Database-driven applications</p>
                </div>
            </div>
        </section>
        
        <div class="divider"></div>
        
        <section>
            <h2><i class="fas fa-chart-line"></i> GitHub Stats</h2>
            <div class="stats-container">
                <div class="stat">
                    <img src="https://github-readme-stats.vercel.app/api?username=jonelfa&show_icons=true&theme=dark" alt="GitHub stats" style="width: 100%">
                </div>
                <div class="stat">
                    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=jonelfa&layout=compact&theme=dark" alt="Top languages" style="width: 100%">
                </div>
            </div>
        </section>
        
        <div class="divider"></div>
        
        <section>
            <h2><i class="fas fa-handshake"></i> Connect with Me</h2>
            <div class="contact-links">
                <a href="mailto:joneldayapera8@gmail.com" class="contact-link">
                    <i class="fas fa-envelope"></i> Email
                </a>
                <a href="https://github.com/jonelfa" class="contact-link">
                    <i class="fab fa-github"></i> GitHub
                </a>
            </div>
        </section>
        
        <footer>
            <p>Thanks for visiting! <i class="fas fa-star"></i> Star a repo if you like it!</p>
        </footer>
    </div>
</body>
</html>
