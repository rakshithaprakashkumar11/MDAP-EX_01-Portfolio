# MDAP-EX_01-Portfolio
## Date:

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

## index.html 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rakshitha P - Portfolio</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
</head>
<body>

    <nav class="navbar">
        <div class="logo">Rakshitha P</div>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#experience">Experience</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#achievements">Achievements</a></li>
            <li><a href="#testimonials">Testimonials</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <section id="home" class="section home-section">
        <div class="content">
            <h1>Hello, I'm <span class="typing"></span></h1>
            <p>Passionate Developer | Creative Thinker | Problem Solver</p>
            <a href="#projects" class="btn">View My Work</a>
        </div>
    </section>

    <section id="about" class="section about-section">
        <h2>About Me</h2>
        <p>I am a Computer Science Engineer who believes in crafting solutions with creativity, precision, and excellence. 
        With a solid foundation in programming and design, I strive to build products that not only work but inspire.</p>
        <div class="about-cards">
            <div class="about-card">
                <h3>Web Development</h3>
                <p>Creating responsive, user-friendly websites and applications.</p>
            </div>
            <div class="about-card">
                <h3>UI/UX Design</h3>
                <p>Designing intuitive interfaces focused on great user experiences.</p>
            </div>
            <div class="about-card">
                <h3>Cloud & DevOps</h3>
                <p>Working with cloud technologies to deliver scalable solutions.</p>
            </div>
        </div>
    </section>

    <section id="skills" class="section">
        <h2>Skills</h2>
        <div class="skills-container">
            <div class="skill-card">HTML5</div>
            <div class="skill-card">CSS3</div>
            <div class="skill-card">JavaScript</div>
            <div class="skill-card">React</div>
            <div class="skill-card">Node.js</div>
            <div class="skill-card">MongoDB</div>
            <div class="skill-card">Python</div>
            <div class="skill-card">Java</div>
            <div class="skill-card">SQL</div>
            <div class="skill-card">Firebase</div>
        </div>
    </section>

    <section id="experience" class="section timeline-section">
        <h2>Experience</h2>
        <div class="timeline">
            <div class="timeline-item">
                <div class="timeline-dot"></div>
                <div class="timeline-content">
                    <h3>Frontend Developer Intern</h3>
                    <span>May 2024 - August 2024</span>
                    <p>Worked on enhancing UI/UX for client projects using React and TailwindCSS.</p>
                </div>
            </div>
            <div class="timeline-item">
                <div class="timeline-dot"></div>
                <div class="timeline-content">
                    <h3>Backend Developer - Freelance</h3>
                    <span>January 2025 - Present</span>
                    <p>Developed scalable REST APIs using Node.js and MongoDB for startups.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="projects" class="section">
        <h2>Projects</h2>
        <div class="projects-container">
            <div class="project-card">
                <h3>Alumni Bridge</h3>
                <p>Connecting students and alumni for mentorship and guidance.</p>
            </div>
            <div class="project-card">
                <h3>Smart Weather App</h3>
                <p>Live weather forecasts with a beautiful and responsive interface.</p>
            </div>
            <div class="project-card">
                <h3>Portfolio Builder</h3>
                <p>A no-code platform for creating beautiful portfolios.</p>
            </div>
        </div>
    </section>

    <section id="achievements" class="section">
        <h2>Achievements</h2>
        <ul class="achievements-list">
            <li>Won 1st Place in National Hackathon 2024</li>
            <li>Certified AWS Cloud Practitioner</li>
            <li>Built an AI Chatbot used by 500+ users</li>
        </ul>
    </section>

    <section id="testimonials" class="section">
        <h2>Testimonials</h2>
        <div class="testimonials-container">
            <div class="testimonial-card">
                <p>"Rakshitha delivered beyond expectations. Highly recommend for any web projects!"</p>
                <h4>- Client A</h4>
            </div>
            <div class="testimonial-card">
                <p>"Extremely professional, creative, and timely. Looking forward to more collaborations."</p>
                <h4>- Client B</h4>
            </div>
        </div>
    </section>

    <section id="contact" class="section contact-section">
        <h2>Contact Me</h2>
        <p>Open to freelance, internships, and full-time opportunities!</p>
        <div class="contact-buttons">
            <a href="mailto:Rakshitha@example.com" class="btn">Email Me</a>
            <a href="https://www.linkedin.com" target="_blank" class="btn">LinkedIn</a>
        </div>
    </section>

    <footer>
        <p>© 2025 Rakshitha P | Crafted with passion ❤️</p>
    </footer>

    <script>
        const typingText = ["Rakshitha", "Web Developer", "Creative Coder", "Tech Enthusiast"];
        let count = 0;
        let index = 0;
        let currentText = '';
        let letter = '';

        (function type() {
            if (count === typingText.length) {
                count = 0;
            }
            currentText = typingText[count];
            letter = currentText.slice(0, ++index);

            document.querySelector('.typing').textContent = letter;
            if (letter.length === currentText.length) {
                count++;
                index = 0;
                setTimeout(type, 800);
            } else {
                setTimeout(type, 150);
            }
        }());
    </script>

</body>
</html>

## style.css
```
/* Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Poppins', sans-serif;
    background: linear-gradient(to bottom, #5f7aa2, #68986f);
    color: #333;
    overflow-x: hidden;
}

/* Navbar */
.navbar {
    background: #88a45d;
    padding: 1rem 2rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    top: 0;
    z-index: 1000;
}

.logo {
    font-size: 2rem;
    color: #fff;
    font-weight: 700;
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
    transition: color 0.3s ease;
}

.nav-links li a:hover {
    color: #ffbe0b;
}

/* Sections */
.section {
    padding: 100px 20px;
    text-align: center;
}

.section h2 {
    font-size: 2.8rem;
    margin-bottom: 20px;
    color: #3a86ff;
    position: relative;
}

.section h2::after {
    content: "";
    width: 60px;
    height: 4px;
    background: #ffbe0b;
    display: block;
    margin: 10px auto 0;
    border-radius: 10px;
}

.section p {
    font-size: 1.2rem;
    color: #555;
    max-width: 800px;
    margin: 0 auto;
}

/* Home Section */
.home-section {
    min-height: 90vh;
    background: linear-gradient(135deg, #3a86ff, #8338ec);
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
}

.home-section h1 {
    font-size: 3rem;
    margin-bottom: 20px;
}

.typing {
    color: #ffbe0b;
}

/* Buttons */
.btn {
    display: inline-block;
    margin-top: 20px;
    background: #ffbe0b;
    padding: 12px 30px;
    border-radius: 30px;
    color: #333;
    font-weight: bold;
    text-decoration: none;
    transition: all 0.4s ease;
    box-shadow: 0 0 8px rgba(0, 0, 0, 0.2);
}

.btn:hover {
    background: #fff;
    color: #3a86ff;
    transform: scale(1.05);
}

/* About Section */
.about-cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
    margin-top: 40px;
}

.about-card {
    background: #fff;
    padding: 20px;
    width: 300px;
    border-radius: 15px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.1);
    transition: transform 0.3s;
}

.about-card:hover {
    transform: translateY(-10px);
}

/* Skills Section */
.skills-container {
    margin-top: 50px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
    gap: 20px;
}

.skill-card {
    background: #ffffff;
    padding: 15px;
    border-radius: 10px;
    font-weight: 600;
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    transition: transform 0.3s ease, background 0.3s ease;
}

.skill-card:hover {
    background: #d0e8ff;
    transform: translateY(-8px);
}

/* Timeline Section */
.timeline {
    margin-top: 50px;
    position: relative;
}

.timeline::before {
    content: '';
    position: absolute;
    left: 50%;
    width: 4px;
    height: 100%;
    background: #3a86ff;
    transform: translateX(-50%);
}

.timeline-item {
    margin: 30px 0;
    position: relative;
    width: 50%;
    padding: 20px;
}

.timeline-item:nth-child(odd) {
    left: 0;
}

.timeline-item:nth-child(even) {
    left: 50%;
}

.timeline-dot {
    width: 15px;
    height: 15px;
    background: #ffbe0b;
    border-radius: 50%;
    position: absolute;
    top: 20px;
    left: 50%;
    transform: translateX(-50%);
}

/* Projects */
.projects-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 30px;
    margin-top: 40px;
}

.project-card {
    background: #fff;
    padding: 20px;
    border-radius: 15px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
    transition: transform 0.4s ease;
}

.project-card:hover {
    transform: translateY(-10px);
    background: #ffe066;
}

/* Achievements */
.achievements-list {
    list-style: none;
    margin-top: 40px;
    font-size: 1.2rem;
}

.achievements-list li {
    margin: 10px 0;
}

/* Testimonials */
.testimonials-container {
    display: flex;
    justify-content: center;
    gap: 30px;
    margin-top: 40px;
    flex-wrap: wrap;
}

.testimonial-card {
    background: #ffffff;
    padding: 20px;
    border-radius: 15px;
    width: 300px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.1);
}

/* Contact */
.contact-buttons {
    margin-top: 30px;
}

/* Footer */
footer {
    background: #3a86ff;
    color: #fff;
    text-align: center;
    padding: 20px 10px;
    margin-top: 50px;
}

```


## OUTPUT

<img width="1891" height="907" alt="image" src="https://github.com/user-attachments/assets/1f38e783-2428-4142-a44a-ae21e3f513da" />

<img width="1894" height="907" alt="image" src="https://github.com/user-attachments/assets/0d59d18e-ad13-42a1-9a41-6da7ea0d0db9" />

<img width="1860" height="487" alt="image" src="https://github.com/user-attachments/assets/85bfd9ac-6624-4b07-ad98-1b0bd778e2f0" />

<img width="1894" height="877" alt="image" src="https://github.com/user-attachments/assets/bae91631-caf6-4abe-8590-07b21452503a" />

<img width="1887" height="904" alt="image" src="https://github.com/user-attachments/assets/b9828e3d-e96d-48a6-85d3-f38316fff655" />

<img width="1895" height="689" alt="image" src="https://github.com/user-attachments/assets/a0571d60-13d7-46aa-ab88-c265a7a5eaff" />

<img width="1892" height="902" alt="image" src="https://github.com/user-attachments/assets/24febc47-dbd9-46e6-a84e-80447ea9cadb" />









## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
