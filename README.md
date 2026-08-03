# my-firm-website
Welcome to Mega Footcare – your trusted destination for complete foot health and comfort. We specialize in advanced podiatry treatments, therapeutic footwear, and custom orthotics designed to keep you moving pain-free. Healthy feet, happy life.
!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MEGA FOOTCARE | Premium Footwear Wholesaler in Katihar, Bihar</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #1E3A8A;
            --primary-dark: #0F172A;
            --secondary: #D97706;
            --accent: #2563EB;
            --bg-light: #F8FAFC;
            --text-dark: #1E293B;
            --text-muted: #64748B;
            --white: #FFFFFF;
            --shadow: 0 10px 30px -10px rgba(30, 58, 138, 0.15);
            --radius: 12px;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.6;
        }

        /* Top Bar */
        .top-bar {
            background-color: var(--primary-dark);
            color: var(--white);
            padding: 8px 5%;
            font-size: 0.85rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .top-bar-info span {
            margin-right: 20px;
        }

        .top-bar-info i {
            color: var(--secondary);
            margin-right: 5px;
        }

        /* Header & Nav */
        header {
            background: var(--white);
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 18px 5%;
            max-width: 1280px;
            margin: 0 auto;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 800;
            color: var(--primary);
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo span {
            color: var(--secondary);
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 30px;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-dark);
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--accent);
        }

        .btn-contact {
            background: var(--primary);
            color: var(--white) !important;
            padding: 10px 22px;
            border-radius: 30px;
            font-weight: 600;
            transition: all 0.3s;
        }

        .btn-contact:hover {
            background: var(--accent);
            transform: translateY(-2px);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #1E3A8A 0%, #0F172A 100%);
            color: var(--white);
            padding: 80px 5%;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
        }

        .badge {
            background: rgba(217, 119, 6, 0.2);
            color: #FBBF24;
            border: 1px solid rgba(217, 119, 6, 0.4);
            padding: 6px 16px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1px;
            display: inline-block;
            margin-bottom: 20px;
        }

        .hero h1 {
            font-size: 2.8rem;
            font-weight: 800;
            margin-bottom: 20px;
            line-height: 1.2;
        }

        .hero p {
            font-size: 1.15rem;
            opacity: 0.9;
            margin-bottom: 35px;
            font-weight: 300;
        }

        .hero-btns {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn-main {
            background-color: var(--secondary);
            color: var(--white);
            padding: 14px 32px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1rem;
            box-shadow: 0 4px 15px rgba(217, 119, 6, 0.4);
            transition: all 0.3s;
        }

        .btn-main:hover {
            background-color: #B45309;
            transform: translateY(-3px);
        }

        .btn-outline {
            border: 2px solid var(--white);
            color: var(--white);
            padding: 14px 32px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1rem;
            transition: all 0.3s;
        }

        .btn-outline:hover {
            background: var(--white);
            color: var(--primary);
            transform: translateY(-3px);
        }

        /* Section Container */
        .section {
            padding: 70px 5%;
            max-width: 1280px;
            margin: 0 auto;
        }

        .section-header {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-header h2 {
            font-size: 2.2rem;
            color: var(--primary-dark);
            margin-bottom: 10px;
            font-weight: 700;
        }

        .section-header p {
            color: var(--text-muted);
            font-size: 1rem;
        }

        /* Features / Why Choose Us */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .feature-card {
            background: var(--white);
            padding: 30px;
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            text-align: center;
            transition: transform 0.3s;
        }

        .feature-card:hover {
            transform: translateY(-8px);
        }

        .feature-icon {
            width: 60px;
            height: 60px;
            background: rgba(37, 99, 235, 0.1);
            color: var(--accent);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            margin: 0 auto 20px;
        }

        .feature-card h3 {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: var(--primary-dark);
        }

        .feature-card p {
            color: var(--text-muted);
            font-size: 0.9rem;
        }

        /* Categories Section */
        .categories-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .category-card {
            background: var(--white);
            border-radius: var(--radius);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: transform 0.3s;
        }

        .category-card:hover {
            transform: translateY(-5px);
        }

        .category-img {
            height: 180px;
            background-color: #E2E8F0;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3.5rem;
            color: var(--primary);
        }

        .category-body {
            padding: 25px;
        }

        .category-body h3 {
            font-size: 1.3rem;
            margin-bottom: 8px;
            color: var(--primary-dark);
        }

        .category-body p {
            color: var(--text-muted);
            font-size: 0.9rem;
        }

        /* Brands Banner */
        .brands-section {
            background: var(--white);
            padding: 50px 5%;
            border-top: 1px solid #E2E8F0;
            border-bottom: 1px solid #E2E8F0;
        }

        .brands-flex {
            display: flex;
            justify-content: space-around;
            align-items: center;
            flex-wrap: wrap;
            gap: 30px;
            max-width: 1100px;
            margin: 0 auto;
        }

        .brand-item {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--text-muted);
            letter-spacing: 1px;
            text-transform: uppercase;
            padding: 10px 20px;
            border: 2px dashed #E2E8F0;
            border-radius: 8px;
        }

        /* Contact & Location Section */
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 40px;
            background: var(--white);
            padding: 40px;
            border-radius: var(--radius);
            box-shadow: var(--shadow);
        }

        .contact-info h3 {
            font-size: 1.5rem;
            color: var(--primary-dark);
            margin-bottom: 20px;
        }

        .info-item {
            display: flex;
            align-items: flex-start;
            margin-bottom: 20px;
            gap: 15px;
        }

        .info-item i {
            font-size: 1.2rem;
            color: var(--secondary);
            margin-top: 4px;
        }

        .info-item h4 {
            font-size: 1rem;
            color: var(--primary-dark);
        }

        .info-item p {
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        /* Footer */
        footer {
            background: var(--primary-dark);
            color: var(--white);
            text-align: center;
            padding: 25px 5%;
            font-size: 0.9rem;
            margin-top: 50px;
        }

        footer span {
            color: var(--secondary);
        }

        /* Floating WhatsApp Button */
        .whatsapp-float {
            position: fixed;
            bottom: 25px;
            right: 25px;
            background-color: #25D366;
            color: var(--white);
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 30px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            z-index: 1000;
            text-decoration: none;
            transition: transform 0.3s;
        }

        .whatsapp-float:hover {
            transform: scale(1.1);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .navbar {
                flex-direction: column;
                gap: 15px;
            }
            .hero h1 {
                font-size: 2.1rem;
            }
            .top-bar {
                text-align: center;
                justify-content: center;
                gap: 10px;
            }
        }
    </style>
</head>
<body>

    <!-- Top Info Bar -->
    <div class="top-bar">
        <div class="top-bar-info">
            <span><i class="fas fa-map-marker-alt"></i> Shiv Mandir Gali, Mangal Bazaar, Katihar - 854105</span>
            <span><i class="fas fa-certificate"></i> Premium Wholesale & Retail Footwear</span>
        </div>
    </div>

    <!-- Header / Navbar -->
    <header>
        <nav class="navbar">
            <a href="#" class="logo"><i class="fas fa-shoe-prints"></i> MEGA <span>FOOTCARE</span></a>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About Us</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#contact" class="btn-contact">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <span class="badge">Bihar's Leading Footwear Hub</span>
            <h1>Super Quality Footwear for Every Step</h1>
            <p>Deals in top brands & high-quality footwear across Bihar. Wholesale & bulk distribution with unmatched pricing and durability.</p>
            <div class="hero-btns">
                <a href="#products" class="btn-main">View Collections</a>
                <a href="https://wa.me/919000000000?text=Hello%20Mega%20Footcare,%20I%20have%20an%20inquiry" class="btn-outline" target="_blank"><i class="fab fa-whatsapp"></i> Inquiry on WhatsApp</a>
            </div>
        </div>
    </section>

    <!-- Why Choose Us -->
    <section class="section" id="about">
        <div class="section-header">
            <h2>Why Choose MEGA FOOTCARE?</h2>
            <p>Your trusted partner for wholesale and retail footwear solutions in Bihar</p>
        </div>
        <div class="features-grid">
            <div class="feature-card">
                <div class="feature-icon"><i class="fas fa-award"></i></div>
                <h3>Super Brands</h3>
                <p>Top-rated regional and national footwear brands under one roof with 100% genuine quality.</p>
            </div>
            <div class="feature-card">
                <div class="feature-icon"><i class="fas fa-tags"></i></div>
                <h3>Best Rates</h3>
                <p>Unbeatable wholesale rates for retailers and highly competitive prices for all customers.</p>
            </div>
            <div class="feature-card">
                <div class="feature-icon"><i class="fas fa-cubes"></i></div>
                <h3>Huge Variety</h3>
                <p>Wide selection ranging from daily casual wear, formal shoes, sports, and specialized footwear.</p>
            </div>
            <div class="feature-card">
                <div class="feature-icon"><i class="fas fa-truck-fast"></i></div>
                <h3>Reliable Supply</h3>
                <p>Timely order fulfillment and stock availability for business partners across Bihar.</p>
            </div>
        </div>
    </section>

    <!-- Product Categories -->
    <section class="section" id="products" style="background-color: #F1F5F9; border-radius: 20px;">
        <div class="section-header">
            <h2>Our Product Ranges</h2>
            <p>Explore our extensive footwear categories</p>
        </div>
        <div class="categories-grid">
            <div class="category-card">
                <div class="category-img"><i class="fas fa-shoe-prints"></i></div>
                <div class="category-body">
                    <h3>Casual Footwear</h3>
                    <p>Comfortable slippers, sandals, and daily wear footwear designed for durability.</p>
                </div>
            </div>
            <div class="category-card">
                <div class="category-img"><i class="fas fa-user-tie"></i></div>
                <div class="category-body">
                    <h3>Formal Shoes</h3>
                    <p>Premium leather and synthetic formal shoes for men and professionals.</p>
                </div>
            </div>
            <div class="category-card">
                <div class="category-img"><i class="fas fa-running"></i></div>
                <div class="category-body">
                    <h3>Sports & Sneakers</h3>
                    <p>Lightweight, trendy sports footwear for active daily lifestyle.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Brands Strip -->
    <div class="brands-section">
        <div class="section-header" style="margin-bottom: 30px;">
            <h2 style="font-size: 1.5rem;">Partnering with Top Brands</h2>
        </div>
        <div class="brands-flex">
            <div class="brand-item">SUPER BRANDS</div>
            <div class="brand-item">PREMIUM QUALITY</div>
            <div class="brand-item">WHOLESALE BIHAR</div>
            <div class="brand-item">MEGA COLLECTION</div>
        </div>
    </div>

    <!-- Contact & Address Section -->
    <section class="section" id="contact">
        <div class="section-header">
            <h2>Visit Our Store</h2>
            <p>Get in touch for orders, wholesale inquiries, or store visits</p>
        </div>
        <div class="contact-container">
            <div class="contact-info">
                <h3>Store Location & Info</h3>
                <div class="info-item">
                    <i class="fas fa-building"></i>
                    <div>
                        <h4>Store Name</h4>
                        <p>MEGA FOOTCARE</p>
                    </div>
                </div>
                <div class="info-item">
                    <i class="fas fa-map-marker-alt"></i>
                    <div>
                        <h4>Address</h4>
                        <p>Shiv Mandir Gali, Mangal Bazaar,<br>Katihar, Bihar - 854105</p>
                    </div>
                </div>
                <div class="info-item">
                    <i class="fas fa-store"></i>
                    <div>
                        <h4>Business Type</h4>
                        <p>Wholesale & Retail Footwear Distributor</p>
                    </div>
                </div>
            </div>
            <div class="contact-info">
                <h3>Quick Connect</h3>
                <div class="info-item">
                    <i class="fas fa-phone-alt"></i>
                    <div>
                        <h4>Call / WhatsApp</h4>
                        <p>+91 90000 00000 (Replace with your number)</p>
                    </div>
                </div>
                <div class="info-item">
                    <i class="fas fa-clock"></i>
                    <div>
                        <h4>Opening Hours</h4>
                        <p>Monday - Saturday: 10:00 AM - 8:00 PM</p>
                    </div>
                </div>
                <div style="margin-top: 20px;">
                    <a href="https://wa.me/919000000000?text=Hello%20Mega%20Footcare" class="btn-main" style="display: inline-block; text-align: center; width: 100%;" target="_blank">
                        <i class="fab fa-whatsapp"></i> Contact on WhatsApp Now
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 <span>MEGA FOOTCARE</span>. Shiv Mandir Gali, Mangal Bazaar, Katihar, Bihar - 854105. All Rights Reserved.</p>
    </footer>

    <!-- Floating WhatsApp Icon -->
    <a href="https://wa.me/919000000000?text=Hello%20Mega%20Footcare" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

</body>
</html>
