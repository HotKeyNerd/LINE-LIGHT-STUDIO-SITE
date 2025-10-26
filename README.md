# LINE-LIGHT-STUDIO-SITE
WEBSITE LINK TO LINE &amp; LIGHT
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Light & Line Studio - Engraved Excellence</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Roboto:wght@300;400&display=swap" rel="stylesheet">
    <style>
        /*
        * CSS Zen Garden / Modernist Inspired Styles
        * Clean, structured, thoughtful typography, minimal color palette.
        */

        :root {
            --color-primary: #333;     /* Dark Charcoal for text/structure */
            --color-secondary: #007bff; /* Bright Blue - representing the 'Light' and the laser */
            --color-light: #f9f9f9;    /* Off-White for background */
            --color-accent: #A9A9A9;   /* Dark Gray for subtle borders/accents */
            --font-serif: 'Playfair Display', serif;
            --font-sans: 'Roboto', sans-serif;
            --max-width: 1200px;
        }

        /* Base & Reset */
        *, *::before, *::after {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: var(--font-sans);
            line-height: 1.6;
            color: var(--color-primary);
            background-color: var(--color-light);
            scroll-behavior: smooth;
        }

        a {
            color: var(--color-primary);
            text-decoration: none;
            transition: color 0.3s;
        }

        a:hover {
            color: var(--color-secondary);
        }

        /* Utility Classes */
        .container {
            width: 90%;
            max-width: var(--max-width);
            margin: 0 auto;
            padding: 20px 0;
        }

        .text-center {
            text-align: center;
        }

        /* Header / Navigation */
        .header {
            background: var(--color-light);
            border-bottom: 1px solid var(--color-accent);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .nav-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }

        .logo {
            font-family: var(--font-serif);
            font-size: 1.8em;
            font-weight: 700;
            letter-spacing: 1px;
            color: var(--color-secondary);
        }

        .nav-menu {
            list-style: none;
            display: flex;
        }

        .nav-item a {
            padding: 10px 15px;
            text-transform: uppercase;
            font-size: 0.9em;
            font-weight: 400;
            letter-spacing: 0.5px;
            position: relative;
        }

        /* Zen Garden Underline Effect */
        .nav-item a::after {
            content: '';
            position: absolute;
            left: 50%;
            bottom: 0;
            width: 0;
            height: 2px;
            background: var(--color-secondary);
            transition: width 0.3s ease-out, left 0.3s ease-out;
        }

        .nav-item a:hover::after {
            width: 100%;
            left: 0;
        }

        .menu-toggle {
            display: none; /* Hide on desktop */
            font-size: 1.5em;
            cursor: pointer;
            border: none;
            background: none;
        }

        /* Hero Section */
        .hero {
            background: url('https://picsum.photos/seed/laserwood/1920/800') center/cover no-repeat;
            color: white;
            height: 80vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            position: relative;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.4); /* Dark overlay */
        }

        .hero-content {
            z-index: 10;
            max-width: 800px;
            padding: 20px;
        }

        .hero-content h1 {
            font-family: var(--font-serif);
            font-size: 4em;
            margin-bottom: 0.2em;
            letter-spacing: 2px;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
        }

        .hero-content p {
            font-size: 1.3em;
            margin-bottom: 30px;
            font-weight: 300;
        }

        .hero-cta {
            background-color: var(--color-secondary);
            color: var(--color-light);
            padding: 15px 30px;
            text-transform: uppercase;
            font-weight: 700;
            letter-spacing: 1px;
            border: 2px solid var(--color-secondary);
            transition: background-color 0.3s, color 0.3s, border-color 0.3s;
        }

        .hero-cta:hover {
            background-color: transparent;
            color: var(--color-secondary);
            border-color: var(--color-secondary);
        }

        /* Section Styling */
        section {
            padding: 60px 0;
        }

        h2 {
            font-family: var(--font-serif);
            font-size: 2.5em;
            text-align: center;
            margin-bottom: 40px;
            color: var(--color-primary); /* Keeping H2 primary, let the line be secondary */
            position: relative;
        }

        h2::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background: var(--color-secondary);
            margin: 10px auto 0;
        }

        /* Product Grid */
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
            text-align: center;
        }

        .product-card {
            border: 1px solid var(--color-accent);
            padding: 20px;
            transition: transform 0.3s, box-shadow 0.3s;
            background: white;
        }

        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.05);
        }

        .product-card img {
            max-width: 100%;
            height: auto;
            margin-bottom: 15px;
            display: block;
            border: 1px solid var(--color-accent);
            /* Aspect ratio placeholder for images */
            min-height: 250px;
            background-color: #ddd;
        }

        .product-card h3 {
            font-family: var(--font-serif);
            color: var(--color-primary);
            margin-bottom: 10px;
        }

        .product-card p {
            font-size: 0.9em;
            color: var(--color-primary);
            margin-bottom: 15px;
        }

        .price {
            font-weight: 700;
            color: var(--color-secondary);
            font-size: 1.2em;
            display: block;
            margin-bottom: 15px;
        }

        .buy-btn {
            background-color: var(--color-primary);
            color: var(--color-light);
            padding: 10px 20px;
            text-transform: uppercase;
            font-size: 0.8em;
            font-weight: 400;
            border: none;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .buy-btn:hover {
            background-color: var(--color-secondary);
        }

        /* About Section (Zen Garden Content) */
        .about-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }

        .about-text {
            flex: 1;
            font-size: 1.1em;
        }

        .about-image {
            flex: 1;
            min-width: 300px;
            background: url('https://picsum.photos/seed/laser/600/400') center/cover no-repeat;
            height: 400px;
            border: 5px double var(--color-secondary); /* Zen Garden border style */
        }

        /* Footer */
        .footer {
            background-color: var(--color-primary);
            color: var(--color-light);
            padding: 40px 0;
            text-align: center;
            border-top: 5px solid var(--color-secondary);
        }

        .footer-links {
            list-style: none;
            margin-bottom: 20px;
        }

        .footer-links li {
            display: inline;
            margin: 0 15px;
        }

        .footer-links a {
            color: var(--color-light);
            text-transform: uppercase;
            font-size: 0.9em;
        }

        .footer-links a:hover {
            color: var(--color-secondary);
        }

        .footer p {
            font-size: 0.8em;
            color: var(--color-accent);
        }

        /* Accessibility/Mobile */
        @media (max-width: 768px) {
            .nav-menu {
                display: none;
                flex-direction: column;
                width: 100%;
                position: absolute;
                top: 70px; /* Adjust based on header height */
                left: 0;
                background: var(--color-light);
                border-top: 1px solid var(--color-accent);
                padding: 10px 0;
            }

            .nav-menu.active {
                display: flex;
            }

            .nav-item {
                text-align: center;
                margin: 5px 0;
                border-bottom: 1px solid var(--color-light);
            }

            .nav-item a {
                display: block;
                padding: 15px;
            }

            .menu-toggle {
                display: block; /* Show menu toggle button */
            }

            .hero-content h1 {
                font-size: 2.5em;
            }

            .hero-content p {
                font-size: 1em;
            }

            .about-content {
                flex-direction: column;
            }

            .about-image {
                width: 100%;
                height: 300px;
            }
        }
    </style>
</head>
<body>

    <header class="header">
        <div class="container nav-content">
            <a href="#hero" class="logo">Light & Line Studio</a>
            <button class="menu-toggle" id="menu-toggle" aria-label="Toggle navigation menu">&#9776;</button>
            <nav>
                <ul class="nav-menu" id="nav-menu">
                    <li class="nav-item"><a href="#shop">Shop</a></li>
                    <li class="nav-item"><a href="#about">About Us</a></li>
                    <li class="nav-item"><a href="#process">The Process</a></li>
                    <li class="nav-item"><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section class="hero" id="hero">
        <div class="hero-content">
            <h1>Where Precision Light Meets Perfect Line.</h1>
            <p>Masterfully laser-engraved wooden checkerboards and unique, small pigeon statues, crafted with precision and passion.</p>
            <a href="#shop" class="hero-cta">Explore the Collection</a>
        </div>
    </section>

    <section id="shop">
        <div class="container">
            <h2>Our Featured Wares</h2>
            <div class="product-grid">
                <div class="product-card">
                    <img src="https://picsum.photos/seed/checkers1/300/300" alt="Laser Engraved Oak Checkerboard">
                    <h3>The Classic Oak Board</h3>
                    <span class="price">$149.99</span>
                    <p>Precisely engraved on solid American Oak. A centerpiece for any game night.</p>
                    <button class="buy-btn">Add to Cart</button>
                </div>

                <div class="product-card">
                    <img src="https://picsum.photos/seed/pigeon1/300/300" alt="Small Wooden Pigeon Statue">
                    <h3>The Studio Mascot Pigeon</h3>
                    <span class="price">$39.00</span>
                    <p>Small, detailed, and surprisingly charming. A mascot for your desk or shelf.</p>
                    <button class="buy-btn">Add to Cart</button>
                </div>

                <div class="product-card">
                    <img src="https://picsum.photos/seed/checkers2/300/300" alt="Custom Engraved Walnut Checkerboard">
                    <h3>The Walnut Heirloom Board</h3>
                    <span class="price">$249.99</span>
                    <p>Deep rich walnut. Includes custom engraving options for names or dates.</p>
                    <button class="buy-btn">Customize & Buy</button>
                </div>
            </div>
        </div>
    </section>

    <section id="about" style="background-color: white;">
        <div class="container">
            <h2>The Light & Line Studio Story</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>**Light & Line Studio** was born from a passion for combining the absolute precision of modern **laser engraving** with the timeless warmth of **traditional woodworking**. We are artists and engineers, crafting pieces that are both technologically perfect and emotionally resonant.</p>
                    <p>Our commitment is to meticulous detail, sustainable material sourcing, and a design philosophy rooted in accessible beauty. We don't just create products; we create durable, custom-made items meant to be passed down through generations. And yes, we have a soft spot for small, perfectly carved pigeon statues.</p>
                    <p class="text-center" style="margin-top: 20px;"><a href="#" style="color: var(--color-secondary); font-weight: 700;">Read Our Full Manifesto &rarr;</a></p>
                </div>
                <div class="about-image" role="img" aria-label="Image of a craftsman working with a laser machine"></div>
            </div>
        </div>
    </section>

    <section id="process" style="background-color: var(--color-light);">
        <div class="container text-center">
            <h2>The Meticulous Process</h2>
            <p style="max-width: 800px; margin: 0 auto 30px;">From the carefully selected rough lumber to the final oil rub, every product undergoes a four-stage journey of cutting, engraving, finishing, and quality inspection. The precision of the laser is matched only by the attention of the human eye.</p>
            <img src="https://picsum.photos/seed/process/1000/300" alt="Infographic showing the product creation process" style="max-width: 100%; height: auto; border: 1px solid var(--color-accent);">
        </div>
    </section>

    <section id="contact" style="background-color: white;">
        <div class="container text-center">
            <h2>Connect with Us</h2>
            <p>Have a custom design idea? Need corporate gifting options? Drop us a line.</p>
            <form action="#" style="max-width: 500px; margin: 30px auto; display: flex; flex-direction: column; gap: 15px;">
                <input type="text" placeholder="Your Name" required style="padding: 10px; border: 1px solid var(--color-accent);">
                <input type="email" placeholder="Your Email" required style="padding: 10px; border: 1px solid var(--color-accent);">
                <textarea placeholder="Your Message" rows="5" required style="padding: 10px; border: 1px solid var(--color-accent);"></textarea>
                <button type="submit" class="buy-btn" style="background-color: var(--color-secondary);">Send Message</button>
            </form>
        </div>
    </section>

    <footer class="footer">
        <div class="container">
            <ul class="footer-links">
                <li><a href="#shop">Shop</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#">Privacy</a></li>
            </ul>
            <p>&copy; 2025 Light & Line Studio. All Rights Reserved. Crafted with care in the USA.</p>
            <p style="margin-top: 10px; font-size: 0.7em;">Images sourced from Picsum for placeholder demonstration.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const menuToggle = document.getElementById('menu-toggle');
            const navMenu = document.getElementById('nav-menu');

            // Toggle the menu visibility
            menuToggle.addEventListener('click', () => {
                navMenu.classList.toggle('active');
            });

            // Close the menu when a link is clicked (for single-page navigation)
            document.querySelectorAll('.nav-item a').forEach(link => {
                link.addEventListener('click', () => {
                    if (window.innerWidth <= 768) {
                        navMenu.classList.remove('active');
                    }
                });
            });
        });
    </script>
</body>
</html>
