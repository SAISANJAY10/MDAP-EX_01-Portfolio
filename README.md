# MDAP-EX_01-Portfolio

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
index.js
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
    <header>
        <nav class="navbar">
            <div class="logo">🌟 MyPortfolio</div>
            <ul class="nav-links">
                <li><a href="#" onclick="showSection('home')">Home</a></li>
                <li><a href="#" onclick="showSection('about')">About</a></li>
                <li><a href="#" onclick="showSection('projects')">Projects</a></li>
                <li><a href="#" onclick="showSection('contact')">Contact</a></li>
            </ul>
        </nav>
    </header>
    <section id="home" class="content-section home-section">
        <h1>Hello, I'm <span>SAI SANJAY R</span> 👋</h1>
        <p>Creative Web Developer | Designer | Learner</p>
    </section>

    <section id="about" class="content-section about-section" style="display:none;">
        <h2>About Me</h2>
        <img src="index.jpg" alt="My Photo" class="profile-pic">
        <p><center>
           Ever since I discovered the world of web development, I have been fascinated by the way technology can bring ideas to life. In the beginning, I was simply curious about how websites worked. I would open different sites, click around, and wonder how the colors, shapes, buttons, and animations were all made. This curiosity quickly turned into a passion, and I started learning HTML, CSS, and JavaScript step by step. Each time I created something new, even if it was just a simple page with a few buttons, I felt proud and excited to learn more.

Over time, I began to realize that web development is not just about writing code—it’s about creating experiences. A good website is more than a place where people read information; it’s a space where they feel comfortable, where they can easily find what they need, and where the design feels pleasant and natural. That’s why, whenever I start a project, I think about the people who will use it. I imagine what they might be looking for, how they will move from one page to another, and how I can make that journey smooth and enjoyable.

I love working on the design side of things, too. My style is a mix of bright, eye-catching colors with clean and simple layouts. I believe that a website should be easy to navigate but also exciting to look at. Too much clutter can confuse visitors, so I focus on keeping my designs clear, balanced, and user-friendly. Whether it’s choosing the right color combination, arranging elements on the page, or deciding how animations will appear, I pay attention to every detail because I know these small choices can make a big difference.

Another thing that excites me is building websites that work perfectly on all devices. We live in a world where people browse the internet on phones, tablets, laptops, and desktops, and I want to make sure my work looks and feels great on every screen. This is why I always build responsive designs, so no matter what device someone is using, they have a smooth experience.

Outside of coding and designing, I spend a lot of time learning. The world of web development changes so quickly, and I want to stay ahead by exploring new tools, frameworks, and design trends. Sometimes I read articles or watch tutorials, and other times I experiment with new ideas in my own projects. I enjoy trying out fresh UI and UX techniques, not only because it makes my skills stronger, but also because it keeps my work creative and exciting.

For me, web development is like a blend of art and engineering. On one hand, I get to be creative—choosing colors, designing layouts, and adding animations. On the other hand, I solve technical problems—fixing bugs, improving performance, and making everything work together. This mix of creativity and logic is what keeps me motivated every day.

Every project I work on is a chance to grow, learn, and challenge myself. I believe that the best websites are the ones made with passion, care, and attention to detail. My ultimate goal is to keep improving my skills and to create digital experiences that are not only functional but also leave a lasting positive impression on the people who use them.
        </center></p>
    </section>

    <section id="projects" class="content-section projects-section" style="display:none;">
        <h2>My Projects</h2>
        <div class="project-container">
            <div class="project-card">
                <h3>🌐 Project One</h3>
                <p>A stunning website built with HTML, CSS, and JavaScript.</p>
            </div>
            <div class="project-card">
                <h3>📱 Project Two</h3>
                <p>A mobile-friendly design that adapts to any screen size.</p>
            </div>
            <div class="project-card">
                <h3>🎨 Project Three</h3>
                <p>A creative and colorful portfolio template.</p>
            </div>
        </div>
    </section>

    <section id="contact" class="content-section contact-section" style="display:none;">
        <h2>Contact Me</h2>
        <p>📧 Email: <a href="mailto:youremail@example.com">saisanjay10@gmail.com</a></p>
        <p>📞 Phone: +91 7550149643</p>
    </section>

    <footer>
        <p>&copy; 2025 SAI SANJAY R | Made with ❤️</p>
    </footer>
    <script>
        function showSection(sectionId) {
            document.querySelectorAll('.content-section').forEach(sec => {
                sec.style.display = 'none';
            });
            document.getElementById(sectionId).style.display = 'block';
        }
    </script>

</body>
</html>
```
style.css
```
body {
    font-family: 'Segoe UI', sans-serif;
    margin: 0;
    padding: 0;
}
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: linear-gradient(90deg, #ff5f6d, #ffc371);
    padding: 12px 20px;
}

.logo {
    color: white;
    font-size: 22px;
    font-weight: bold;
}

.nav-links {
    list-style: none;
    display: flex;
    margin: 0;
}

.nav-links li {
    margin: 0 10px;
}

.nav-links a {
    text-decoration: none;
    color: white;
    font-weight: bold;
    padding: 6px 12px;
    border-radius: 6px;
    transition: all 0.3s ease;
}

.nav-links a:hover {
    background: white;
    color: #ff5f6d;
}
.content-section {
    padding: 50px;
    text-align: center;
    min-height: 70vh;
    color: white;
}

.home-section {
    background: linear-gradient(135deg, #667eea, #764ba2);
}

.about-section {
    background: linear-gradient(135deg, #ff758c, #ff7eb3);
}

.projects-section {
    background: linear-gradient(135deg, #43cea2, #185a9d);
}

.contact-section {
    background: linear-gradient(135deg, #f7971e, #ffd200);
}
.project-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
}
.profile-pic {
    width: 150px;
    height: 150px;
    object-fit: cover;
    border-radius: 50%;
    border: 4px solid white;
    box-shadow: 0px 5px 15px rgba(0,0,0,0.3);
}
.project-card {
    background: white;
    color: black;
    padding: 20px;
    border-radius: 10px;
    width: 250px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 25px rgba(0,0,0,0.3);
}
footer {
    text-align: center;
    background: linear-gradient(90deg, #ff5f6d, #ffc371);
    color: white;
    padding: 10px;
}
a {
    color: white;
    text-decoration: underline;
}
```
## OUTPUT

<img width="1916" height="1028" alt="Screenshot 2025-08-24 202823" src="https://github.com/user-attachments/assets/838c75a2-20e5-4771-840a-cf9fbdf27765" />
<img width="1909" height="1021" alt="Screenshot 2025-08-24 202839" src="https://github.com/user-attachments/assets/4ce6229f-004a-481a-80b3-c611b159fb99" />
<img width="1915" height="1026" alt="Screenshot 2025-08-24 202849" src="https://github.com/user-attachments/assets/17e72bcc-ead8-4ab1-baee-fd0fa3bee396" />
<img width="1919" height="1027" alt="Screenshot 2025-08-24 202901" src="https://github.com/user-attachments/assets/81e6cf26-9102-436b-990c-29963352526b" />



## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
