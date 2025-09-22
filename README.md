<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SEO Portfolio - Dipesh Ramteke</title>
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #f5f7fa;
      color: #333;
      overflow-x: hidden;
    }
    header {
      background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://source.unsplash.com/1600x600/?digital,marketing') center/cover;
      color: white;
      text-align: center;
      padding: 100px 20px;
      animation: fadeIn 2s ease-in-out;
    }
    header h1 {
      font-size: 3rem;
      margin: 0;
      animation: slideDown 1.5s ease;
    }
    header p {
      font-size: 1.3rem;
      margin-top: 10px;
    }
    nav {
      position: sticky;
      top: 0;
      background: #2c3e50;
      padding: 15px;
      display: flex;
      justify-content: center;
      z-index: 1000;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #3498db;
    }
    section {
      max-width: 1100px;
      margin: 50px auto;
      padding: 30px;
      background: white;
      border-radius: 15px;
      box-shadow: 0 6px 18px rgba(0,0,0,0.1);
      opacity: 0;
      transform: translateY(50px);
      transition: all 1s ease;
    }
    section.visible {
      opacity: 1;
      transform: translateY(0);
    }
    h2 {
      color: #2c3e50;
      margin-bottom: 15px;
      font-weight: 600;
    }
    ul {
      list-style: none;
      padding: 0;
    }
    ul li {
      background: #ecf0f1;
      margin: 10px 0;
      padding: 12px;
      border-radius: 8px;
      transition: transform 0.3s;
    }
    ul li:hover {
      transform: translateX(8px);
      background: #dfe6e9;
    }
    .skills img, .projects img, .about img {
      width: 100%;
      border-radius: 12px;
      margin: 15px 0;
      transition: transform 0.5s ease;
    }
    .skills img:hover, .projects img:hover, .about img:hover {
      transform: scale(1.05);
    }
    footer {
      text-align: center;
      padding: 25px;
      background: #2c3e50;
      color: white;
      margin-top: 40px;
    }
    a {
      color: #3498db;
      text-decoration: none;
    }
    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }
    @keyframes slideDown {
      from {transform: translateY(-50px); opacity: 0;}
      to {transform: translateY(0); opacity: 1;}
    }
  </style>
</head>
<body>

  <header>
    <h1>Dipesh Ramteke</h1>
    <p>SEO Enthusiast | Learner | Future Entrepreneur</p>
  </header>

  <nav>
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="about" class="about">
    <h2>About Me</h2>
    <p>I help businesses increase their online visibility, improve Google rankings, and drive targeted organic traffic through proven SEO strategies.</p>
    <img src="https://source.unsplash.com/1000x400/?seo,analytics" alt="SEO Work">
  </section>

  <section id="skills" class="skills">
    <h2>Core SEO Skills</h2>
    <ul>
      <li>✔ Keyword Research & Competitor Analysis</li>
      <li>✔ On-Page SEO Optimization</li>
      <li>✔ Technical SEO (Speed, Mobile, Indexing)</li>
      <li>✔ Off-Page SEO</li>
      <li>✔ Local SEO & Google My Business</li>
      <li>✔ SEO Content Strategy & Writing</li>
      <li>✔ Tools: Google Analytics, SEMrush, Ahrefs</li>
    </ul>
    <img src="https://source.unsplash.com/1000x400/?keywords,seo" alt="SEO Skills">
  </section>

  <section id="projects" class="projects">
    <h2>Projects & Results</h2>
    <ul>
      <li>📈 Increased organic traffic by 150% for an e-commerce brand in 6 months.</li>
      <li>🏆 Ranked 20+ high-competition keywords on page 1 of Google.</li>
      <li>🔧 Performed SEO audits fixing critical technical issues.</li>
      <li>📍 Helped a local business rank #1 for top local keywords.</li>
    </ul>
    <img src="https://source.unsplash.com/1000x400/?business,success" alt="SEO Projects">
  </section>

  <section id="contact" class="contact">
    <h2>Contact</h2>
    <p>📧 Email: <a href="mailto:yourname@email.com">monuramteke71@gmail.com</a></p>
    <p>💼 LinkedIn: <a href="#">linkedin.com/in/www.linkedin.com/in/dipesh-ramteke-1b5607238?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app</a></p>
    <p>📱 Phone: +91-6266961440</p>
  </section>

  <footer>
    <p>© 2025 Dipesh Ramteke | SEO Portfolio</p>
  </footer>

  <script>
    // Smooth scroll
    document.querySelectorAll('nav a').forEach(anchor => {
      anchor.addEventListener('click', function(e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
          behavior: 'smooth'
        });
      });
    });

    // Fade-in sections on scroll
    const sections = document.querySelectorAll('section');
    const revealOnScroll = () => {
      const triggerBottom = window.innerHeight * 0.85;
      sections.forEach(section => {
        const sectionTop = section.getBoundingClientRect().top;
        if (sectionTop < triggerBottom) {
          section.classList.add('visible');
        }
      });
    };
    window.addEventListener('scroll', revealOnScroll);
    revealOnScroll();
  </script>

</body>
</html>
