<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rishabh Kumar Pandey</title>
    <style>
        :root {
            --primary-color: #3a86ff;
            --secondary-color: #8338ec;
            --accent-color: #ff006e;
            --light-color: #f8f9fa;
            --dark-color: #212529;
            --success-color: #38b000;
            --warning-color: #ffbb00;
            --danger-color: #d00000;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--light-color);
            color: var(--dark-color);
            line-height: 1.6;
        }

        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 2rem 0;
            text-align: center;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            letter-spacing: 1px;
        }

        .nav-links {
            display: flex;
            list-style: none;
        }

        .nav-links li {
            margin-left: 2rem;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
        }

        .nav-links a:hover {
            color: var(--accent-color);
        }

        .hero {
            text-align: center;
            padding: 4rem 0;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            background: linear-gradient(to right, var(--accent-color), var(--warning-color));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 2rem;
        }

        .btn {
            display: inline-block;
            background-color: var(--accent-color);
            color: white;
            padding: 0.8rem 1.8rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }

        .features {
            padding: 5rem 0;
            background-color: white;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }

        .section-title h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .section-title p {
            color: #6c757d;
            max-width: 700px;
            margin: 0 auto;
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .feature-card {
            background-color: var(--light-color);
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease;
        }

        .feature-card:hover {
            transform: translateY(-10px);
        }

        .feature-icon {
            font-size: 2.5rem;
            margin-bottom: 1.5rem;
            color: var(--primary-color);
        }

        .feature-card h3 {
            margin-bottom: 1rem;
        }

        .showcase {
            padding: 5rem 0;
            background: linear-gradient(to right, #f8f9fa, #e9ecef);
        }

        .showcase-content {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: space-between;
        }

        .showcase-text {
            flex: 1;
            min-width: 300px;
            padding-right: 2rem;
        }

        .showcase-image {
            flex: 1;
            min-width: 300px;
        }

        .showcase-image img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        .testimonials {
            padding: 5rem 0;
            background-color: white;
        }

        .testimonial-slider {
            display: flex;
            overflow-x: auto;
            scroll-snap-type: x mandatory;
            gap: 2rem;
            padding: 2rem 0;
            scrollbar-width: none;
        }

        .testimonial-slider::-webkit-scrollbar {
            display: none;
        }

        .testimonial-card {
            min-width: 300px;
            scroll-snap-align: start;
            background-color: var(--light-color);
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }

        .testimonial-card img {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 1.5rem;
        }

        .testimonial-text {
            margin-bottom: 1.5rem;
            font-style: italic;
        }

        .testimonial-author {
            font-weight: 700;
        }

        .cta {
            padding: 5rem 0;
            text-align: center;
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
        }

        .cta h2 {
            font-size: 2.5rem;
            margin-bottom: 1.5rem;
        }

        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 3rem 0;
            text-align: center;
        }

        .footer-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin-bottom: 2rem;
        }

        .footer-column {
            flex: 1;
            min-width: 250px;
            margin-bottom: 2rem;
        }

        .footer-column h3 {
            margin-bottom: 1.5rem;
            font-size: 1.2rem;
        }

        .footer-column ul {
            list-style: none;
        }

        .footer-column li {
            margin-bottom: 0.8rem;
        }

        .footer-column a {
            color: #adb5bd;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-column a:hover {
            color: var(--primary-color);
        }

        .copyright {
            padding-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
            color: #adb5bd;
        }

        /* Responsive styles */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .hero h1 {
                font-size: 2.2rem;
            }

            .showcase-content {
                flex-direction: column;
            }

            .showcase-text {
                padding-right: 0;
                margin-bottom: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <nav>
                <div class="logo">Digital Horizon</div>
                <ul class="nav-links">
                    <li><a href="#features">Features</a></li>
                    <li><a href="#showcase">Showcase</a></li>
                    <li><a href="#testimonials">Testimonials</a></li>
                    <li><a href="#contact" class="btn">Contact</a></li>
                </ul>
            </nav>
            <div class="hero">
                <h1>Transform Your Digital Experience</h1>
                <p>Discover innovative solutions designed to elevate your business and personal projects to new heights.</p>
                <a href="#features" class="btn">Explore More</a>
            </div>
        </div>
    </header>

    <section class="features" id="features">
        <div class="container">
            <div class="section-title">
                <h2>Powerful Features</h2>
                <p>Our platform offers everything you need to succeed in the digital landscape.</p>
            </div>
            <div class="feature-grid">
                <div class="feature-card">
                    <div class="feature-icon">⚡</div>
                    <h3>Lightning Fast</h3>
                    <p>Optimized for performance with cutting-edge technology to deliver blazing fast results.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">🔒</div>
                    <h3>Secure & Private</h3>
                    <p>Enterprise-grade security protocols to keep your data safe and confidential.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">🔄</div>
                    <h3>Seamless Integration</h3>
                    <p>Compatible with all major platforms and services for smooth interoperability.</p>
                </div>
            </div>
        </div>
    </section>

    <section class="showcase" id="showcase">
        <div class="container">
            <div class="showcase-content">
                <div class="showcase-text">
                    <h2>Intuitive Design</h2>
                    <p>Our platform features a clean, user-friendly interface that simplifies complex tasks. With thoughtful UX design and smart workflows, you'll be more productive from day one.</p>
                    <p>Customizable dashboards allow you to personalize your workspace to match your unique workflow preferences.</p>
                    <a href="#" class="btn">Try Demo</a>
                </div>
                <div class="showcase-image">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/62961ed9-e1b3-4332-9ea1-fb93b2a45b0f.png" alt="Modern dashboard interface showing analytics with colorful charts and graphs" />
                </div>
            </div>
        </div>
    </section>

    <section class="testimonials" id="testimonials">
        <div class="container">
            <div class="section-title">
                <h2>What People Say</h2>
                <p>Don't just take our word for it - hear from our satisfied customers.</p>
            </div>
            <div class="testimonial-slider">
                <div class="testimonial-card">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/d1403677-298a-4110-8e66-41aa3364ca7e.png" alt="Professional headshot of Sarah Johnson, Marketing Director" />
                    <p class="testimonial-text">"Digital Horizon transformed our workflow efficiency. We've seen a 40% increase in productivity since implementation."</p>
                    <p class="testimonial-author">Sarah Johnson</p>
                    <p>Marketing Director, TechCorp</p>
                </div>
                <div class="testimonial-card">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/79622ad0-99b4-4537-9fdd-cc195124cd01.png" alt="Portrait of Michael Chen, startup founder smiling confidently" />
                    <p class="testimonial-text">"As a startup founder, I needed affordable but powerful tools. Digital Horizon delivered beyond my expectations."</p>
                    <p class="testimonial-author">Michael Chen</p>
                    <p>Founder, NextGen Apps</p>
                </div>
                <div class="testimonial-card">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/d1ffa495-af39-45c9-b286-595a633ffedc.png" alt="Lisa Rodriguez in business attire looking professional" />
                    <p class="testimonial-text">"The customer support team is phenomenal. They helped us customize the platform for our specific industry needs."</p>
                    <p class="testimonial-author">Lisa Rodriguez</p>
                    <p>Operations Manager, RetailPro</p>
                </div>
            </div>
        </div>
    </section>

    <section class="cta" id="contact">
        <div class="container">
            <h2>Ready to Get Started?</h2>
            <p>Join thousands of satisfied customers who are already benefiting from our platform.</p>
            <a href="#" class="btn" style="background-color: white; color: var(--primary-color);">Sign Up Free</a>
        </div>
    </section>

    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Digital Horizon</h3>
                    <p>Innovative solutions for the digital age.</p>
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#features">Features</a></li>
                        <li><a href="#showcase">Showcase</a></li>
                        <li><a href="#testimonials">Testimonials</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Legal</h3>
                    <ul>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Terms of Service</a></li>
                        <li><a href="#">Cookie Policy</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>© 2023 Digital Horizon. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Mobile menu toggle functionality
        const mobileMenuBtn = document.createElement('button');
        mobileMenuBtn.innerHTML = '☰';
        mobileMenuBtn.style.cssText = 'display: none; background: none; border: none; font-size: 1.5rem; color: white; cursor: pointer;';

        function setupMobileMenu() {
            const nav = document.querySelector('nav');
            const navLinks = document.querySelector('.nav-links');
            
            if (window.innerWidth <= 768) {
                mobileMenuBtn.style.display = 'block';
                nav.insertBefore(mobileMenuBtn, navLinks);
                navLinks.style.display = 'none';
                
                mobileMenuBtn.addEventListener('click', () => {
                    if (navLinks.style.display === 'none') {
                        navLinks.style.display = 'flex';
                        navLinks.style.flexDirection = 'column';
                        navLinks.style.position = 'absolute';
                        navLinks.style.top = '100%';
                        navLinks.style.left = '0';
                        navLinks.style.right = '0';
                        navLinks.style.backgroundColor = 'rgba(58, 134, 255, 0.9)';
                        navLinks.style.padding = '1rem';
                        navLinks.style.zIndex = '100';
                    } else {
                        navLinks.style.display = 'none';
                    }
                });
            } else {
                mobileMenuBtn.style.display = 'none';
                if (navLinks) navLinks.style.display = 'flex';
            }
        }

        // Initial setup
        setupMobileMenu();
        
        // Update on window resize
        window.addEventListener('resize', setupMobileMenu);
    </script>
</body>
</html>


