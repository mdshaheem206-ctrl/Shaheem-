<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Zest & Flow - 100% Organic Cold-Pressed Juice in Bangalore. Fresh, healthy, delivered daily. Order via WhatsApp!">
    <meta name="keywords" content="cold pressed juice, organic juice, Bangalore juice, healthy drinks, fresh juice delivery">
    <meta name="author" content="Zest & Flow Juicery">
    <title>Zest & Flow | Organic Cold-Pressed Juice | Bangalore</title>
    <style>
        /* --- CSS STYLES --- */
        :root {
            --primary: #FF8C42; /* Citrus Orange */
            --secondary: #4E9F3D; /* Leaf Green */
            --dark: #333333;
            --light: #F9F9F9;
            --white: #ffffff;
            --font-main: 'Helvetica Neue', sans-serif;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: var(--font-main);
            color: var(--dark);
            background-color: var(--light);
            line-height: 1.6;
        }

        a { text-decoration: none; color: inherit; }
        ul { list-style: none; }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 5%;
            background: var(--white);
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--secondary);
        }
        .logo span { color: var(--primary); }

        .nav-links { display: flex; gap: 2rem; }
        .nav-links a:hover { color: var(--primary); transition: 0.3s; }

        .btn {
            background-color: var(--primary);
            color: var(--white);
            padding: 0.7rem 1.5rem;
            border-radius: 50px;
            font-weight: bold;
            transition: transform 0.2s ease;
            cursor: pointer;
            border: none;
            display: inline-block;
        }
        .btn:hover {
            background-color: #e67e3b;
            transform: scale(1.05);
        }

        /* Hero Section */
        .hero {
            height: 90vh;
            background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.3)), url('https://images.unsplash.com/photo-1620916566398-39f1143ab7be?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: var(--white);
            padding: 0 1rem;
        }
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            max-width: 600px;
        }

        /* Features Section */
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            padding: 4rem 5%;
            background: var(--white);
            text-align: center;
        }
        .feature-card h3 { color: var(--secondary); margin-bottom: 0.5rem; }

        /* Menu/Products Section */
        .menu { padding: 4rem 5%; }
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2.5rem;
            color: var(--dark);
        }
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        .product-card {
            background: var(--white);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        .product-card:hover { transform: translateY(-5px); }
        .product-img {
            height: 250px;
            width: 100%;
            object-fit: cover;
        }
        .product-info { padding: 1.5rem; }
        .price {
            color: var(--primary);
            font-weight: bold;
            font-size: 1.2rem;
            display: block;
            margin-top: 0.5rem;
        }

        /* About Section */
        .about {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            padding: 4rem 5%;
            background-color: #e8f5e9;
        }
        .about-text { flex: 1; padding-right: 2rem; min-width: 300px; }
        .about-image { flex: 1; min-width: 300px; }
        .about-image img { width: 100%; border-radius: 15px; }

        /* Payment Section */
        .payment-info {
            text-align: center;
            padding: 2rem 5%;
            background: var(--white);
            border-top: 1px solid #eee;
            border-bottom: 1px solid #eee;
        }
        .payment-info strong { color: var(--secondary); }
        .upi-id {
            background: var(--light);
            padding: 0.5rem 1rem;
            border-radius: 8px;
            font-family: monospace;
            font-weight: bold;
            color: var(--primary);
            display: inline-block;
            margin-top: 0.5rem;
        }

        /* Footer Styles */
        footer {
            background: var(--dark);
            color: var(--white);
            padding: 3rem 5%;
            text-align: center;
        }
        .contact-info { margin-bottom: 1.5rem; }
        .contact-info a {
            color: var(--white);
            text-decoration: underline;
        }
        .socials { margin: 1.5rem 0; }
        
        /* Social Link Buttons */
        .social-link {
            display: inline-block;
            margin: 0 10px 10px;
            color: var(--primary);
            font-weight: bold;
            border: 1px solid var(--primary);
            padding: 8px 15px;
            border-radius: 20px;
            transition: all 0.3s ease;
        }
        .social-link:hover {
            background-color: var(--primary);
            color: var(--white);
        }

        /* ✨ WhatsApp Floating Button */
        .whatsapp-float {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #25D366;
            color: white;
            border-radius: 50px;
            padding: 12px 20px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.15);
            z-index: 999;
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 8px;
            transition: transform 0.2s ease;
        }
        .whatsapp-float:hover {
            transform: scale(1.05);
            background-color: #128C7E;
        }

        /* Mobile Responsive */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2.5rem; }
            .nav-links { display: none; }
            .about { flex-direction: column-reverse; gap: 2rem; }
            .about-text { padding-right: 0; }
            .whatsapp-float {
                bottom: 15px;
                right: 15px;
                padding: 10px 16px;
                font-size: 0.9rem;
            }
        }
    </style>
</head>
<body>

    <!-- NAVIGATION -->
    <nav>
        <div class="logo">Zest<span>&</span>Flow</div>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#menu">Menu</a></li>
            <li><a href="#about">Our Story</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
        <a href="https://wa.me/919789877899?text=Hi!%20I'd%20like%20to%20order%20juice" class="btn" target="_blank">Order Now</a>
    </nav>

    <!-- HERO SECTION -->
    <header id="home" class="hero">
        <h1>Sip the Sunshine.</h1>
        <p>100% Organic, Cold-Pressed juices delivered fresh across Bangalore every morning.</p>
        <a href="#menu" class="btn">View Our Menu</a>
    </header>

    <!-- FEATURES -->
    <section class="features">
        <div class="feature-card">
            <h3>🌱 100% Organic</h3>
            <p>Sourced from local Karnataka farms, certified organic.</p>
        </div>
        <div class="feature-card">
            <h3>❄️ Cold-Pressed</h3>
            <p>Hydraulic pressed to retain maximum nutrients & enzymes.</p>
        </div>
        <div class="feature-card">
            <h3>♻️ Eco-Friendly</h3>
            <p>Glass bottles – return for ₹20 off your next order!</p>
        </div>
    </section>

    <!-- MENU SECTION -->
    <section id="menu" class="menu">
        <h2 class="section-title">Fresh Favorites</h2>
        <div class="product-grid">
            <!-- Product 1 -->
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1613478223719-2ab802602423?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Green Juice" class="product-img">
                <div class="product-info">
                    <h3>The Green Glow</h3>
                    <p>Kale, Spinach, Apple, Lemon, Ginger.</p>
                    <span class="price">₹299</span>
                </div>
            </div>
            <!-- Product 2 -->
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1621506289937-a8e4df240d0b?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Orange Juice" class="product-img">
                <div class="product-info">
                    <h3>Citrus Immunity</h3>
                    <p>Orange, Carrot, Turmeric, Black Pepper.</p>
                    <span class="price">₹199</span>
                </div>
            </div>
            <!-- Product 3 -->
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1620916297397-a4a5402a3c6c?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Beet Juice" class="product-img">
                <div class="product-info">
                    <h3>Root Reboot</h3>
                    <p>Beetroot, Apple, Lemon, Ginger.</p>
                    <span class="price">₹249</span>
                </div>
            </div>
        </div>
    </section>

    <!-- PAYMENT INFO SECTION -->
    <section class="payment-info">
        <p><strong>💳 We Accept:</strong> UPI, GPay, PhonePe, Paytm, Cash on Delivery</p>
        <p style="margin-top: 0.5rem;">
            UPI ID: <span class="upi-id">zestandflow@oksbi</span>
        </p>
        <p style="font-size: 0.9rem; margin-top: 1rem; color: #666;">
            🚚 Free delivery on orders above ₹499 in Bangalore
        </p>
    </section>

    <!-- ABOUT SECTION -->
    <section id="about" class="about">
        <div class="about-text">
            <h2 style="margin-bottom: 1rem;">Pressed with Purpose</h2>
            <p>At Zest & Flow, we believe that health comes from nature, not a lab. Founded in 2024 in Bangalore, our mission is to make healthy living accessible, delicious, and sustainable.</p>
            <br>
            <p>We never use HPP (High Pressure Processing), added sugars, or preservatives. Just fresh fruits and vegetables from local farms, pure and simple.</p>
            <br>
            <p><strong>📍 Serving:</strong> Indiranagar, Koramangala, MG Road, Whitefield & surrounding areas.</p>
        </div>
        <div class="about-image">
            <img src="https://images.unsplash.com/photo-1600353068866-565d4e6643ae?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Fresh juice preparation">
        </div>
    </section>

    <!-- FOOTER -->
    <footer id="contact">
        <h2>Ready to refresh?</h2>
        
        <div class="contact-info">
            <p>📍 Shop No. 12, MG Road, Bangalore, Karnataka 560001</p>
            <p>📧 hello@zestandflow.com</p>
            <p>📞 <a href="tel:+919789877899">+91 97898 77899</a></p>
            <p style="margin-top: 0.5rem; font-size: 0.95rem;">
                ⏰ <strong>Hours:</strong> Mon-Sun, 7:00 AM - 9:00 PM
            </p>
        </div>

        <div class="socials">
            <a href="https://instagram.com/md_shaheem" target="_blank" class="social-link">📸 Instagram: @md_shaheem</a>
            <a href="https://snapchat.com/add/Md_Shaheem" target="_blank" class="social-link">👻 Snapchat: Md_Shaheem</a>
        </div>

        <p style="font-size: 0.8rem; opacity: 0.7; margin-top: 2rem;">
            &copy; 2026 Zest & Flow Juicery, Bangalore. All rights reserved.
        </p>
    </footer>

    <!-- ✨ WhatsApp Floating Button -->
    <a href="https://wa.me/919789877899?text=Hi!%20I'd%20like%20to%20order%20juice%20from%20Zest%20%26%20Flow%20Juicery" 
       target="_blank" 
       class="whatsapp-float">
       💬 Order on WhatsApp
    </a>

    <script>
        // Smooth scroll for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth' });
                }
            });
        });

        // Optional: Add animation to WhatsApp button on scroll
        window.addEventListener('scroll', () => {
            const whatsappBtn = document.querySelector('.whatsapp-float');
            if (window.scrollY > 300) {
                whatsappBtn.style.opacity = '1';
            }
        });
    </script>
</body>
</html>
