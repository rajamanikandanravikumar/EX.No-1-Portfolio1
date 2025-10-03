# Ex01 Portfolio
## Date: 03-10-2025

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM

### HTML:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Rajamanikandan | Portfolio</title>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
  <!-- Font Awesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" />
  <!-- CSS -->
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <!-- Navigation -->
  <nav>
    <div class="container nav-container">
      <a href="#" class="logo">Rajamanikandan</a>
      <ul class="nav-links">
        <li><a href="#About">About</a></li>
        <li><a href="#Services">Services</a></li>
        <li><a href="#Projects">Projects</a></li>
        <li><a href="#Skills">Skills</a></li>
        <li><a href="#Contact">Contact</a></li>
      </ul>
      <div class="burger">
        <div class="line1"></div>
        <div class="line2"></div>
        <div class="line3"></div>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <header>
    <div class="header-container container">
      <div class="header-left">
        <h1>Hello, I'm <span>Rajamanikandan</span></h1>
        <p class="subtitle">Software Developer | CSE Student</p>
        <p class="desc">
          I craft scalable software and build interactive web experiences.
          Passionate about coding, web development, and machine learning.
        </p>
        <a href="#Contact" class="btn">Hire Me</a>
      </div>
      <div class="header-right">
        <img src="profile.jpg" alt="Rajamanikandan">
      </div>
    </div>
  </header>

  <!-- About -->
  <section id="About" class="section">
    <div class="container">
      <h2>About Me</h2>
      <div class="about-grid">
        <div class="about-left">
          <p>
            I'm a Computer Science Engineer with expertise in web development, programming,
            and problem-solving. I love turning ideas into functional, elegant applications.
          </p>
          <a href="#Projects" class="btn-outline">See My Work</a>
        </div>
        <div class="about-right">
          <img src="profile.jpg" alt="Rajamanikandan" />
        </div>
      </div>
    </div>
  </section>

  <!-- Services -->
  <section id="Services" class="section bg-light">
    <div class="container">
      <h2>Services</h2>
      <div class="services-grid">
        <div class="service-card">
          <i class="fas fa-code fa-2x"></i>
          <h3>Web Development</h3>
          <p>Responsive, modern websites using HTML, CSS, JS & frameworks.</p>
        </div>
        <div class="service-card">
          <i class="fas fa-lightbulb fa-2x"></i>
          <h3>Problem Solving</h3>
          <p>Strong foundation in algorithms & data structures for efficient solutions.</p>
        </div>
        <div class="service-card">
          <i class="fas fa-robot fa-2x"></i>
          <h3>Machine Learning</h3>
          <p>Building predictive models and AI solutions for real-world problems.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Projects -->
  <section id="Projects" class="section">
    <div class="container">
      <h2>Projects</h2>
      <div class="projects-grid">
        <div class="project-card">
          <h3>Portfolio Website</h3>
          <p>Responsive portfolio built with modern HTML, CSS & JS.</p>
          <a href="#" class="btn-outline">View Project</a>
        </div>
        <div class="project-card">
          <h3>Student Result Predictor</h3>
          <p>ML model predicting student performance with high accuracy.</p>
          <a href="#" class="btn-outline">View Project</a>
        </div>
        <div class="project-card">
          <h3>Online Food Ordering</h3>
          <p>Full-stack web application for ordering and delivery services.</p>
          <a href="#" class="btn-outline">View Project</a>
        </div>
      </div>
    </div>
  </section>

  <!-- Skills -->
  <section id="Skills" class="section bg-light">
    <div class="container">
      <h2>Skills</h2>
      <div class="skills-grid">
        <span class="skill">HTML</span>
        <span class="skill">CSS</span>
        <span class="skill">JavaScript</span>
        <span class="skill">Python</span>
        <span class="skill">SQL</span>
        <span class="skill">Problem Solving</span>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="Contact" class="section">
    <div class="container">
      <h2>Contact Me</h2>
      <form>
        <input type="text" placeholder="Name" required>
        <input type="email" placeholder="Email" required>
        <input type="text" placeholder="Subject" required>
        <textarea placeholder="Message" required></textarea>
        <button class="btn" type="submit">Send Message</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 Rajamanikandan. All Rights Reserved.</p>
    <div class="socials">
      <a href="#"><i class="fab fa-linkedin"></i></a>
      <a href="#"><i class="fab fa-github"></i></a>
      <a href="#"><i class="fab fa-twitter"></i></a>
    </div>
  </footer>

  <!-- JS for burger menu -->
  <script>
    const burger = document.querySelector('.burger');
    const nav = document.querySelector('.nav-links');

    burger.addEventListener('click', () => {
      nav.classList.toggle('nav-active');
      burger.classList.toggle('toggle');
    });
  </script>
</body>
</html>

```

### CSS:
```
/* Reset & Base */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Roboto', sans-serif;
}

body {
  line-height: 1.6;
  color: #333;
  background: #fefefe;
  scroll-behavior: smooth;
}

/* Container */
.container {
  width: 90%;
  max-width: 1200px;
  margin: auto;
}

/* Navigation */
nav {
  background: linear-gradient(90deg, #4e54c8, #8f94fb);
  padding: 1rem 0;
  position: sticky;
  top: 0;
  z-index: 1000;
  box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

.nav-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.6rem;
  font-weight: 700;
  color: #fff;
  text-decoration: none;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 2rem;
}

.nav-links li a {
  color: #fff;
  text-decoration: none;
  font-weight: 500;
  padding: 0.5rem 1rem;
  border-radius: 5px;
  transition: all 0.3s;
}

.nav-links li a:hover {
  background: #fff;
  color: #4e54c8;
}

/* Burger menu */
.burger {
  display: none;
  cursor: pointer;
  flex-direction: column;
  gap: 5px;
}

.burger div {
  width: 25px;
  height: 3px;
  background: #fff;
  transition: all 0.3s ease;
}

.burger.toggle .line1 { transform: rotate(-45deg) translate(-5px,6px); }
.burger.toggle .line2 { opacity: 0; }
.burger.toggle .line3 { transform: rotate(45deg) translate(-5px,-6px); }

.nav-active {
  display: flex !important;
  flex-direction: column;
  position: absolute;
  top: 60px;
  right: 0;
  background: #4e54c8;
  width: 100%;
  text-align: center;
}

/* Header */
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 6rem 0;
  background: linear-gradient(135deg, #8f94fb, #4e54c8);
  color: #fff;
  flex-wrap: wrap;
}

.header-left h1 {
  font-size: 2.8rem;
  margin-bottom: 1rem;
  background: linear-gradient(to right, #fff, #f3f3f3);
  -webkit-background-clip: text;
  color: transparent;
}

.header-left .subtitle {
  font-size: 1.2rem;
  margin-bottom: 1rem;
  color: #e0e0e0;
}

.header-left .desc {
  margin-bottom: 1.5rem;
  font-size: 1rem;
  max-width: 500px;
}

.header-left .btn {
  padding: 0.8rem 1.5rem;
  border-radius: 50px;
  background: #fff;
  color: #4e54c8;
  font-weight: bold;
  text-decoration: none;
  transition: all 0.3s;
}

.header-left .btn:hover {
  background: #4e54c8;
  color: #fff;
  transform: scale(1.05);
}

.header-right img {
  width: 300px;
  border-radius: 50%;
  box-shadow: 0 15px 25px rgba(0,0,0,0.3);
  transition: transform 0.3s;
}

.header-right img:hover {
  transform: scale(1.05) rotate(3deg);
}

/* Sections */
.section {
  padding: 5rem 0;
  text-align: center;
}

.bg-light {
  background: #f5f5ff;
}

h2 {
  font-size: 2.8rem;
  color: #4e54c8;
  margin-bottom: 2rem;
  position: relative;
}

h2::after {
  content: '';
  width: 60px;
  height: 4px;
  background: #8f94fb;
  display: block;
  margin: 10px auto 0;
  border-radius: 2px;
}

/* About Grid */
.about-grid {
  display: flex;
  align-items: center;
  gap: 2rem;
  flex-wrap: wrap;
  justify-content: center;
}

.about-left p {
  font-size: 1rem;
  margin-bottom: 1rem;
  color: #555;
}

.about-left .btn-outline {
  padding: 0.8rem 1.5rem;
  border: 2px solid #4e54c8;
  color: #4e54c8;
  border-radius: 50px;
  text-decoration: none;
  transition: all 0.3s;
}

.about-left .btn-outline:hover {
  background: #4e54c8;
  color: #fff;
  transform: scale(1.05);
}

.about-right img {
  width: 300px;
  border-radius: 20px;
  box-shadow: 0 15px 25px rgba(0,0,0,0.2);
}

/* Services Grid */
.services-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
}

.service-card {
  background: #fff;
  padding: 2rem;
  border-radius: 20px;
  box-shadow: 0 15px 25px rgba(0,0,0,0.1);
  transition: all 0.3s;
}

.service-card:hover {
  transform: translateY(-10px);
}

.service-card i {
  color: #8f94fb;
  margin-bottom: 1rem;
}

/* Projects Grid */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
}

.project-card {
  background: #fff;
  padding: 1.5rem;
  border-radius: 20px;
  box-shadow: 0 15px 25px rgba(0,0,0,0.1);
  transition: all 0.3s;
}

.project-card:hover {
  transform: translateY(-10px) scale(1.03);
}

.project-card a.btn-outline {
  margin-top: 1rem;
  display: inline-block;
}

/* Skills Grid */
.skills-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 1rem;
}

.skill {
  background: #fff;
  padding: 0.5rem 1.5rem;
  border-radius: 25px;
  font-weight: 600;
  color: #4e54c8;
  box-shadow: 0 10px 20px rgba(0,0,0,0.1);
  transition: transform 0.3s;
}

.skill:hover {
  transform: scale(1.1);
}

/* Contact Form */
form {
  max-width: 600px;
  margin: auto;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

form input, form textarea {
  padding: 0.8rem;
  border-radius: 10px;
  border: 1px solid #ccc;
  width: 100%;
  transition: all 0.3s;
}

form input:focus, form textarea:focus {
  border-color: #4e54c8;
  box-shadow: 0 0 10px rgba(78, 84, 200, 0.2);
}

form button {
  padding: 0.8rem;
  border-radius: 50px;
  border: none;
  background: linear-gradient(90deg, #4e54c8, #8f94fb);
  color: #fff;
  cursor: pointer;
  transition: all 0.3s;
}

form button:hover {
  transform: scale(1.05);
}

/* Footer */
footer {
  background: #222;
  color: #fff;
  padding: 2rem 0;
  text-align: center;
}

footer .socials a {
  margin: 0 0.5rem;
  color: #fff;
  transition: all 0.3s;
}

footer .socials a:hover {
  color: #8f94fb;
}

/* Responsive */
@media(max-width: 768px) {
  .header-container {
    flex-direction: column;
  }
  .about-grid {
    flex-direction: column-reverse;
  }
  .burger {
    display: flex;
  }
  .nav-links {
    display: none;
  }
}

```

## OUTPUT
<br>
<img width="1891" height="903" alt="image" src="https://github.com/user-attachments/assets/c33e7197-0d48-4ede-ac5a-1b3c0602bc1b" />
<br>
<img width="1871" height="697" alt="image" src="https://github.com/user-attachments/assets/358e8483-dce6-407c-92d5-06347521b830" />
<br>
<img width="1878" height="565" alt="image" src="https://github.com/user-attachments/assets/09742102-bae1-4976-8291-cb86b9b179e8" />
<br>
<img width="1899" height="816" alt="image" src="https://github.com/user-attachments/assets/6b843db5-5085-466f-8fd8-51fd7b2fdca1" />






## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
