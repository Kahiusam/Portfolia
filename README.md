# Portfolia
Basic code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sarah Johnson | Graphic Designer Portfolio</title>
    <meta name="description" content="Sarah Johnson - Graphic Designer Portfolio">
    <meta name="keywords" content="graphic designer, branding, freelance designer">

    <style>
        /* Base Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #fff;
        }

        /* Navbar */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #222;
            color: #fff;
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 1.5rem;
        }

        .nav-links li a {
            color: #fff;
            text-decoration: none;
            transition: color 0.3s;
        }

        .nav-links li a:hover {
            color: #f39c12;
        }

        /* Hero Section */
        .hero {
            position: relative;
            text-align: center;
            color: white;
            padding: 4rem 1rem;
            background-color: #000;
        }

        .hero-image {
            width: 100%;
            height: auto;
            opacity: 0.3;
            position: absolute;
            top: 0;
            left: 0;
            z-index: -1;
        }

        .hero-text {
            max-width: 800px;
            margin: auto;
        }

        .hero-text h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .cta-button {
            display: inline-block;
            margin: 0.5rem;
            padding: 0.75rem 1.5rem;
            background-color: #f39c12;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: background 0.3s;
        }

        .cta-button:hover {
            background-color: #d35400;
        }

        .cta-button.secondary {
            background-color: transparent;
            border: 2px solid #f39c12;
            color: #f39c12;
        }

        .cta-button.secondary:hover {
            background-color: #f39c12;
            color: #fff;
        }

        /* Sections */
        .section {
            padding: 4rem 2rem;
            text-align: center;
        }

        .section h2 {
            font-size: 2rem;
            margin-bottom: 2rem;
        }

        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }

        .portfolio-item img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
        }

        .portfolio-item h3 {
            margin-top: 1rem;
            color: #222;
        }

        .case-study-link {
            display: inline-block;
            margin-top: 0.5rem;
            color: #f39c12;
            text-decoration: underline;
        }

        .testimonial {
            max-width: 700px;
            margin: auto;
            font-style: italic;
        }

        /* Contact Form */
        form {
            max-width: 600px;
            margin: auto;
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        input, textarea {
            padding: 0.75rem;
            border: 1px solid #ccc;
            border-radius: 5px;
            width: 100%;
        }

        textarea {
            resize: vertical;
            min-height: 120px;
        }

        /* Social Links */
        .social-links {
            margin-top: 1rem;
        }

        .social-links a {
            color: #f39c12;
            margin: 0 0.5rem;
            text-decoration: none;
        }

        .social-links a:hover {
            text-decoration: underline;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            background-color: #222;
            color: #fff;
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <div class="logo">Sarah Johnson Design</div>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#portfolio">Portfolio</a></li>
            <li><a href="#resume">Resume</a></li>
            <li><a href="#testimonials">Testimonials</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <img src="images/hero.jpg" alt="Hero Image" class="hero-image">
        <div class="hero-text">
            <h1>Crafting Bold, Memorable Brands That Connect</h1>
            <a href="#portfolio" class="cta-button">View My Work</a>
            <a href="#contact" class="cta-button secondary">Contact Me</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="section">
        <h2>About Me</h2>
        <p>I’m Sarah Johnson, a passionate graphic designer with over 8 years of experience specializing in branding, digital design, and print media. I help businesses tell their story visually through creative and strategic design solutions.</p>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="section">
        <h2>Portfolio</h2>
        <div class="portfolio-grid">
            <div class="portfolio-item">
                <img src="images/project1.jpg" alt="Brew & Bean Branding">
                <h3>Brew & Bean Coffee Shop</h3>
                <p>Designed a full branding package for a local coffee shop, including logo, business cards, and menus. <br><strong>Tools:</strong> Adobe Illustrator, InDesign <br><strong>Impact:</strong> 15% increase in foot traffic.</p>
                <a href="#portfolio" class="case-study-link">View Case Study</a>
            </div>
            <div class="portfolio-item">
                <img src="images/project2.jpg" alt="Tech Startup Graphics">
                <h3>Tech Startup Website Graphics</h3>
                <p>Developed web graphics and UI components for a SaaS startup’s website. <br><strong>Tools:</strong> Figma, Adobe XD <br><strong>Impact:</strong> 20% improved user engagement.</p>
                <a href="#portfolio" class="case-study-link">View Case Study</a>
            </div>
            <div class="portfolio-item">
                <img src="images/project3.jpg" alt="Music Festival Posters">
                <h3>Music Festival Posters</h3>
                <p>Created vibrant promotional posters for an annual music festival. <br><strong>Tools:</strong> Photoshop, Illustrator <br><strong>Impact:</strong> Boosted ticket sales via social media.</p>
                <a href="#portfolio" class="case-study-link">View Case Study</a>
            </div>
        </div>
    </section>

    <!-- Resume Section -->
    <section id="resume" class="section">
        <h2>Resume</h2>
        <p>Download my resume to learn more about my experience and skills.</p>
        <a href="images/resume.pdf" class="cta-button" download>Download Resume</a>
    </section>

    <!-- Testimonials Section -->
    <section id="testimonials" class="section">
        <h2>What Clients Say</h2>
        <div class="testimonial">
            <p>“Sarah’s designs transformed our brand identity. Her creativity and attention to detail were outstanding!”</p>
            <p><strong>— Lisa, Owner, Brew & Bean</strong></p>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section">
        <h2>Contact Me</h2>
        <p>I typically respond within 24 hours. Let’s create something amazing together!</p>
        <form id="contact-form">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" placeholder="Your Message" required></textarea>
            <button type="submit" class="cta-button">Send Message</button>
        </form>
        <div class="social-links">
            <a href="mailto:sarah@johnsondesign.com">Email</a> |
            <a href="https://linkedin.com/in/sarahjohnson" target="_blank">LinkedIn</a> |
            <a href="https://instagram.com/sarahjdesigns" target="_blank">Instagram</a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 Sarah Johnson Design. All rights reserved.</p>
    </footer>

    <script>
        // Handle contact form submission
        document.getElementById('contact-form').addEventListener('submit', function (e) {
            e.preventDefault();

            const name = this.name.value.trim();
            const email = this.email.value.trim();
            const message = this.message.value.trim();

            if (!name || !email || !message) {
                alert('Please fill in all fields.');
                return;
            }

            alert('Thank you for your message, ' + name + '! I will get back to you soon.');
            this.reset();
        });
    </script>
</body>
</html>
