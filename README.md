<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Google tag (gtag.js) -->
  <script async src="https://www.googletagmanager.com/gtag/js?id=G-MMTYJE2P9G"></script>
  <script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'G-MMTYJE2P9G');
  </script>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Abuzar Khan | AI Engineer Portfolio</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Orbitron:wght@400;500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #38bdf8;
      --primary-dark: #0ea5e9;
      --secondary: #8b5cf6;
      --dark: #0f172a;
      --dark-light: #1e293b;
      --light: #f8fafc;
      --gradient: linear-gradient(135deg, #38bdf8, #8b5cf6);
      --neon-glow: 0 0 15px rgba(56, 189, 248, 0.7);
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background-color: var(--dark);
      color: var(--light);
      overflow-x: hidden;
    }

    /* Header & Navigation */
    header {
      background-color: rgba(15, 23, 42, 0.95);
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 1000;
      backdrop-filter: blur(10px);
      border-bottom: 1px solid rgba(56, 189, 248, 0.2);
      animation: slideDown 0.8s ease-out;
    }

    @keyframes slideDown {
      from { transform: translateY(-100%); }
      to { transform: translateY(0); }
    }

    .logo {
      font-family: 'Orbitron', sans-serif;
      font-size: 1.8rem;
      font-weight: 700;
      background: var(--gradient);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      display: flex;
      align-items: center;
    }

    .logo i {
      margin-right: 10px;
      font-size: 1.5rem;
    }

    .nav-links {
      display: flex;
      gap: 30px;
    }

    .nav-links a {
      color: var(--light);
      text-decoration: none;
      font-weight: 500;
      position: relative;
      padding: 5px 0;
      transition: color 0.3s;
    }

    .nav-links a:hover {
      color: var(--primary);
    }

    .nav-links a::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      width: 0;
      height: 2px;
      background: var(--gradient);
      transition: width 0.3s ease;
    }

    .nav-links a:hover::after {
      width: 100%;
    }

    .linkedin-btn {
      background: var(--gradient);
      color: white;
      padding: 8px 20px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: 600;
      display: flex;
      align-items: center;
      gap: 8px;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .linkedin-btn:hover {
      transform: translateY(-3px);
      box-shadow: var(--neon-glow);
    }

    /* Hero Section */
    .hero {
      min-height: 100vh;
      display: flex;
      align-items: center;
      padding: 0 40px;
      position: relative;
      overflow: hidden;
      margin-top: 80px;
    }

    .hero-bg {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: radial-gradient(circle at 20% 50%, rgba(56, 189, 248, 0.1) 0%, transparent 50%),
                  radial-gradient(circle at 80% 20%, rgba(139, 92, 246, 0.1) 0%, transparent 50%);
      z-index: -1;
    }

    .hero-content {
      max-width: 700px;
      z-index: 2;
      animation: fadeInUp 1s ease-out;
    }

    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .hero h1 {
      font-size: 3.5rem;
      margin-bottom: 20px;
      background: var(--gradient);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      line-height: 1.2;
    }

    .hero h2 {
      font-size: 1.8rem;
      font-weight: 600;
      margin-bottom: 25px;
      color: var(--light);
    }

    .hero p {
      font-size: 1.1rem;
      line-height: 1.8;
      margin-bottom: 40px;
      max-width: 600px;
    }

    .ai-highlight {
      color: var(--primary);
      font-weight: 600;
      position: relative;
      display: inline-block;
    }

    .ai-highlight::after {
      content: '';
      position: absolute;
      bottom: -2px;
      left: 0;
      width: 100%;
      height: 3px;
      background: var(--gradient);
      border-radius: 2px;
    }

    .cta-buttons {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
    }

    .btn {
      padding: 12px 30px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: 600;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      transition: all 0.3s;
      cursor: pointer;
    }

    .btn-primary {
      background: var(--gradient);
      color: white;
      border: none;
    }

    .btn-primary:hover {
      transform: translateY(-5px);
      box-shadow: var(--neon-glow);
    }

    .btn-secondary {
      background: transparent;
      color: var(--primary);
      border: 2px solid var(--primary);
    }

    .btn-secondary:hover {
      background: rgba(56, 189, 248, 0.1);
      transform: translateY(-5px);
    }

    /* Floating AI Elements */
    .floating-elements {
      position: absolute;
      width: 100%;
      height: 100%;
      top: 0;
      left: 0;
      pointer-events: none;
      z-index: 1;
    }

    .floating-element {
      position: absolute;
      color: rgba(56, 189, 248, 0.3);
      font-size: 1.5rem;
      animation: float 15s infinite linear;
    }

    @keyframes float {
      0% { transform: translateY(0) rotate(0deg); }
      25% { transform: translateY(-20px) rotate(90deg); }
      50% { transform: translateY(0) rotate(180deg); }
      75% { transform: translateY(20px) rotate(270deg); }
      100% { transform: translateY(0) rotate(360deg); }
    }

    /* Section Styling */
    section {
      padding: 80px 40px;
      position: relative;
    }

    .section-title {
      font-family: 'Orbitron', sans-serif;
      font-size: 2.5rem;
      margin-bottom: 50px;
      text-align: center;
      position: relative;
    }

    .section-title::after {
      content: '';
      position: absolute;
      bottom: -10px;
      left: 50%;
      transform: translateX(-50%);
      width: 100px;
      height: 4px;
      background: var(--gradient);
      border-radius: 2px;
    }

    /* About Section */
    .about-content {
      display: flex;
      align-items: center;
      gap: 50px;
      flex-wrap: wrap;
    }

    .about-text {
      flex: 1;
      min-width: 300px;
    }

    .about-text p {
      font-size: 1.1rem;
      line-height: 1.8;
      margin-bottom: 20px;
    }

    .ai-badge {
      display: inline-block;
      background: rgba(56, 189, 248, 0.1);
      color: var(--primary);
      padding: 5px 15px;
      border-radius: 50px;
      font-weight: 600;
      margin: 5px;
      border: 1px solid rgba(56, 189, 248, 0.3);
      animation: pulse 2s infinite;
    }

    @keyframes pulse {
      0% { box-shadow: 0 0 0 0 rgba(56, 189, 248, 0.4); }
      70% { box-shadow: 0 0 0 10px rgba(56, 189, 248, 0); }
      100% { box-shadow: 0 0 0 0 rgba(56, 189, 248, 0); }
    }

    .ai-visual {
      flex: 1;
      min-width: 300px;
      height: 300px;
      background: var(--dark-light);
      border-radius: 20px;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
      border: 1px solid rgba(56, 189, 248, 0.2);
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    }

    .ai-visual::before {
      content: '';
      position: absolute;
      width: 200%;
      height: 200%;
      background: conic-gradient(from 0deg, transparent, var(--primary), transparent);
      animation: rotate 10s linear infinite;
    }

    .ai-visual::after {
      content: 'AI ENGINEER';
      position: absolute;
      width: calc(100% - 10px);
      height: calc(100% - 10px);
      background: var(--dark-light);
      border-radius: 18px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Orbitron', sans-serif;
      font-size: 2rem;
      font-weight: 700;
      background: var(--gradient);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      text-align: center;
    }

    @keyframes rotate {
      from { transform: rotate(0deg); }
      to { transform: rotate(360deg); }
    }

    /* Skills Section */
    .skills-container {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
      gap: 20px;
    }

    .skill-card {
      background: var(--dark-light);
      padding: 25px;
      border-radius: 15px;
      text-align: center;
      transition: transform 0.3s, box-shadow 0.3s;
      border: 1px solid rgba(56, 189, 248, 0.1);
      position: relative;
      overflow: hidden;
    }

    .skill-card:hover {
      transform: translateY(-10px);
      box-shadow: var(--neon-glow);
      border-color: var(--primary);
    }

    .skill-card i {
      font-size: 2.5rem;
      margin-bottom: 15px;
      color: var(--primary);
    }

    .skill-card h3 {
      font-size: 1.3rem;
      margin-bottom: 10px;
    }

    /* Projects Section */
    .projects-container {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 30px;
    }

    .project-card {
      background: var(--dark-light);
      border-radius: 15px;
      overflow: hidden;
      transition: transform 0.5s, box-shadow 0.5s;
      border: 1px solid rgba(56, 189, 248, 0.1);
      position: relative;
    }

    .project-card:hover {
      transform: translateY(-15px);
      box-shadow: var(--neon-glow);
    }

    .project-img {
      height: 200px;
      background: linear-gradient(45deg, #1e293b, #334155);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 4rem;
      color: var(--primary);
      position: relative;
      overflow: hidden;
    }

    .project-img::before {
      content: '';
      position: absolute;
      width: 150%;
      height: 150%;
      background: linear-gradient(90deg, transparent, rgba(56, 189, 248, 0.1), transparent);
      animation: shine 3s infinite;
    }

    @keyframes shine {
      0% { transform: translateX(-100%); }
      100% { transform: translateX(100%); }
    }

    .project-content {
      padding: 25px;
    }

    .project-content h3 {
      font-size: 1.5rem;
      margin-bottom: 10px;
      color: var(--primary);
    }

    .project-content p {
      line-height: 1.6;
      margin-bottom: 20px;
    }

    .project-tech {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 15px;
    }

    .tech-tag {
      background: rgba(56, 189, 248, 0.1);
      color: var(--primary);
      padding: 5px 10px;
      border-radius: 20px;
      font-size: 0.8rem;
      font-weight: 500;
    }

    /* Contact Section */
    .contact-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }

    .contact-container p {
      max-width: 600px;
      margin-bottom: 40px;
      font-size: 1.1rem;
      line-height: 1.8;
    }

    .contact-links {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      justify-content: center;
      margin-top: 20px;
    }

    .contact-link {
      display: flex;
      align-items: center;
      gap: 10px;
      color: var(--light);
      text-decoration: none;
      padding: 12px 25px;
      border-radius: 50px;
      background: var(--dark-light);
      transition: all 0.3s;
      border: 1px solid rgba(56, 189, 248, 0.1);
    }

    .contact-link:hover {
      background: var(--gradient);
      transform: translateY(-5px);
      box-shadow: var(--neon-glow);
    }

    /* Footer */
    footer {
      background: var(--dark-light);
      padding: 40px;
      text-align: center;
      border-top: 1px solid rgba(56, 189, 248, 0.2);
    }

    .footer-content {
      max-width: 800px;
      margin: 0 auto;
    }

    .footer-logo {
      font-family: 'Orbitron', sans-serif;
      font-size: 1.8rem;
      font-weight: 700;
      background: var(--gradient);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      margin-bottom: 20px;
    }

    .copyright {
      margin-top: 20px;
      color: #94a3b8;
      font-size: 0.9rem;
    }

    /* Responsive Design */
    @media (max-width: 768px) {
      header {
        padding: 15px 20px;
        flex-direction: column;
        gap: 15px;
      }
      
      .nav-links {
        gap: 15px;
        flex-wrap: wrap;
        justify-content: center;
      }
      
      .hero {
        padding: 0 20px;
        text-align: center;
      }
      
      .hero h1 {
        font-size: 2.5rem;
      }
      
      .hero h2 {
        font-size: 1.5rem;
      }
      
      .cta-buttons {
        justify-content: center;
      }
      
      section {
        padding: 60px 20px;
      }
      
      .section-title {
        font-size: 2rem;
      }
    }
  </style>
</head>
<body>
  <!-- Header & Navigation -->
  <header>
    <div class="logo">
      <i class="fas fa-brain"></i> ABUZAR KHAN
    </div>
    <nav class="nav-links">
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </nav>
    <a href="https://www.linkedin.com/in/abuzar-khan-ba009a35b" class="linkedin-btn" target="_blank">
      <i class="fab fa-linkedin"></i> LinkedIn
    </a>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <div class="hero-bg"></div>
    <div class="floating-elements">
      <div class="floating-element" style="top: 20%; left: 10%;"><i class="fas fa-robot"></i></div>
      <div class="floating-element" style="top: 60%; left: 85%;"><i class="fas fa-microchip"></i></div>
      <div class="floating-element" style="top: 80%; left: 15%;"><i class="fas fa-cogs"></i></div>
      <div class="floating-element" style="top: 30%; left: 80%;"><i class="fas fa-code"></i></div>
    </div>
    <div class="hero-content">
      <h1>AI ENGINEER & ML DEVELOPER</h1>
      <h2>Hi, I'm <span class="ai-highlight">Abuzar Khan</span></h2>
      <p>
        I build intelligent systems that push the boundaries of what's possible with Artificial Intelligence. 
        Passionate about creating AI solutions that are not just smart, but also ethical, efficient, and accessible.
      </p>
      <div class="cta-buttons">
        <a href="#projects" class="btn btn-primary">
          <i class="fas fa-laptop-code"></i> View My Work
        </a>
        <a href="#contact" class="btn btn-secondary">
          <i class="fas fa-paper-plane"></i> Get In Touch
        </a>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="about">
    <h2 class="section-title">ABOUT ME</h2>
    <div class="about-content">
      <div class="about-text">
        <p>
          Hello! I'm <strong>Abuzar Khan</strong>, an aspiring <span class="ai-badge">AI Engineer</span> with a deep passion for 
          <span class="ai-badge">Artificial Intelligence</span>, <span class="ai-badge">Machine Learning</span>, and <span class="ai-badge">Data Science</span>.
        </p>
        <p>
          My journey in AI began with a fascination for how machines can learn and adapt. Today, I specialize in 
          building intelligent systems that make technology more intuitive and human-centric.
        </p>
        <p>
          I believe in the transformative power of AI to solve complex problems and create innovative solutions 
          that have a meaningful impact on people's lives and businesses.
        </p>
        <p>
          When I'm not training models or analyzing data, I'm exploring new AI research papers, contributing to 
          open-source projects, or sharing knowledge with the tech community.
        </p>
      </div>
      <div class="ai-visual"></div>
    </div>
  </section>

  <!-- Skills Section -->
  <section id="skills" class="skills">
    <h2 class="section-title">TECHNICAL SKILLS</h2>
    <div class="skills-container">
      <div class="skill-card">
        <i class="fab fa-python"></i>
        <h3>Python</h3>
        <p>Advanced programming for AI/ML applications</p>
      </div>
      <div class="skill-card">
        <i class="fas fa-brain"></i>
        <h3>Machine Learning</h3>
        <p>Supervised & unsupervised learning algorithms</p>
      </div>
      <div class="skill-card">
        <i class="fas fa-network-wired"></i>
        <h3>Deep Learning</h3>
        <p>Neural networks & advanced architectures</p>
      </div>
      <div class="skill-card">
        <i class="fas fa-chart-line"></i>
        <h3>Data Analysis</h3>
        <p>Data visualization & statistical analysis</p>
      </div>
      <div class="skill-card">
        <i class="fas fa-layer-group"></i>
        <h3>TensorFlow / PyTorch</h3>
        <p>Framework expertise for model development</p>
      </div>
      <div class="skill-card">
        <i class="fas fa-rocket"></i>
        <h3>AI Deployment</h3>
        <p>Model deployment & MLOps pipelines</p>
      </div>
    </div>
  </section>

  <!-- Projects Section -->
  <section id="projects" class="projects">
    <h2 class="section-title">AI PROJECTS</h2>
    <div class="projects-container">
      <div class="project-card">
        <div class="project-img">
          <i class="fas fa-robot"></i>
        </div>
        <div class="project-content">
          <h3>Intelligent AI Chatbot</h3>
          <p>Developed an advanced conversational AI using NLP techniques and transformer architectures to handle complex user queries with contextual understanding.</p>
          <div class="project-tech">
            <span class="tech-tag">Python</span>
            <span class="tech-tag">NLP</span>
            <span class="tech-tag">Transformers</span>
            <span class="tech-tag">OpenAI API</span>
          </div>
        </div>
      </div>
      <div class="project-card">
        <div class="project-img">
          <i class="fas fa-eye"></i>
        </div>
        <div class="project-content">
          <h3>Advanced Image Recognition</h3>
          <p>Built a deep learning vision system capable of real-time object detection and classification with 97%+ accuracy across multiple datasets.</p>
          <div class="project-tech">
            <span class="tech-tag">PyTorch</span>
            <span class="tech-tag">CNN</span>
            <span class="tech-tag">Computer Vision</span>
            <span class="tech-tag">OpenCV</span>
          </div>
        </div>
      </div>
      <div class="project-card">
        <div class="project-img">
          <i class="fas fa-chart-bar"></i>
        </div>
        <div class="project-content">
          <h3>Predictive Analytics Dashboard</h3>
          <p>Created an interactive AI-powered dashboard that predicts business trends and provides actionable insights through advanced ML models.</p>
          <div class="project-tech">
            <span class="tech-tag">Scikit-learn</span>
            <span class="tech-tag">Dash</span>
            <span class="tech-tag">Time Series</span>
            <span class="tech-tag">Flask</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="contact">
    <h2 class="section-title">LET'S CONNECT</h2>
    <div class="contact-container">
      <p>
        I'm always open to discussing AI projects, research opportunities, or potential collaborations. 
        Feel free to reach out if you want to connect or just talk about the future of artificial intelligence!
      </p>
      <a href="https://www.linkedin.com/in/abuzar-khan-ba009a35b" class="btn btn-primary" target="_blank">
        <i class="fab fa-linkedin"></i> Connect on LinkedIn
      </a>
      <div class="contact-links">
        <a href="mailto:hello@abuzarkhan.ai" class="contact-link">
          <i class="fas fa-envelope"></i> Email Me
        </a>
        <a href="https://github.com" class="contact-link" target="_blank">
          <i class="fab fa-github"></i> GitHub
        </a>
        <a href="https://twitter.com" class="contact-link" target="_blank">
          <i class="fab fa-twitter"></i> Twitter
        </a>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="footer-content">
      <div class="footer-logo">
        <i class="fas fa-brain"></i> ABUZAR KHAN
      </div>
      <p>AI Engineer specializing in Machine Learning, Deep Learning, and Intelligent System Design</p>
      <div class="copyright">
        © 2025 Abuzar Khan | All Rights Reserved<br>
        <a href="https://www.linkedin.com/in/abuzar-khan-ba009a35b" style="color: #38bdf8; text-decoration: none;" target="_blank">
          LinkedIn Profile
        </a>
      </div>
    </div>
  </footer>

  <script>
    // Add scroll animation for sections
    document.addEventListener('DOMContentLoaded', function() {
      const observerOptions = {
        threshold: 0.1,
        rootMargin: '0px 0px -50px 0px'
      };

      const observer = new IntersectionObserver(function(entries) {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.style.opacity = '1';
            entry.target.style.transform = 'translateY(0)';
          }
        });
      }, observerOptions);

      // Observe all sections for animation
      document.querySelectorAll('section').forEach(section => {
        section.style.opacity = '0';
        section.style.transform = 'translateY(20px)';
        section.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
        observer.observe(section);
      });

      // Add interactive floating elements
      const floatingContainer = document.querySelector('.floating-elements');
      for(let i = 0; i < 8; i++) {
        const element = document.createElement('div');
        element.className = 'floating-element';
        element.innerHTML = '<i class="fas fa-code"></i>';
        element.style.left = `${Math.random() * 90}%`;
        element.style.top = `${Math.random() * 90}%`;
        element.style.animationDuration = `${15 + Math.random() * 20}s`;
        element.style.animationDelay = `${Math.random() * 5}s`;
        element.style.fontSize = `${1 + Math.random()}rem`;
        element.style.color = `rgba(56, 189, 248, ${0.1 + Math.random() * 0.3})`;
        floatingContainer.appendChild(element);
      }

      // Smooth scrolling for navigation links
      document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function(e) {
          e.preventDefault();
          const targetId = this.getAttribute('href');
          if(targetId === '#') return;
          
          const targetElement = document.querySelector(targetId);
          if(targetElement) {
            window.scrollTo({
              top: targetElement.offsetTop - 80,
              behavior: 'smooth'
            });
          }
        });
      });
    });

    // AI-inspired typing effect for hero section
    window.addEventListener('load', function() {
      const heroTitle = document.querySelector('.hero h1');
      const originalText = heroTitle.textContent;
      heroTitle.textContent = '';
      
      let i = 0;
      function typeWriter() {
        if (i < originalText.length) {
          heroTitle.textContent += originalText.charAt(i);
          i++;
          setTimeout(typeWriter, 50);
        }
      }
      
      // Start typing after a short delay
      setTimeout(typeWriter, 500);
    });
  </script>
</body>
</html>
