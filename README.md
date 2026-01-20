<!DOCTYPE html>
<html lang="en">
<head>
    <!-- 
    ================================================================
    PROJECT: THE GAME POINT (ULTIMATE GAMING PORTAL)
    VERSION: 4.0 (MASTER EDITION)
    FEATURES: AUTO-SLIDER, ZIG-ZAG BLOGS, NEON DESIGN, PRO FOOTER
    ================================================================
    -->
    <!-- Primary Meta Tags -->
    <title>The Game Point | Latest Gaming News, Pro Guides & Hardware Reviews</title>
    <meta name="title" content="The Game Point | Latest Gaming News, Pro Guides & Hardware Reviews">
    <meta name="description" content="The Game Point is your #1 source for latest gaming leaks, GTA 6 updates, BGMI pro tips, and unbiased PC hardware reviews. Level up your game today!">
    <meta name="keywords" content="gaming news, GTA 6 leaks, BGMI pro tips, PC hardware reviews, gaming portal, eSports updates, The Game Point, gaming guides India">
    <meta name="author" content="The Game Point Team">
    <meta name="robots" content="index, follow">
    
    <!-- Open Graph / Facebook (Jab aap link share karenge toh photo aur text dikhega) -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://yourusername.github.io/"> <!-- Yahan apna live link dalein -->
    <meta property="og:title" content="The Game Point | Ultimate Gaming Portal">
    <meta property="og:description" content="Get real-time gaming updates and professional walkthroughs.">
    <meta property="og:image" content="https://images.unsplash.com/photo-1542751371-adc38448a05e?w=800">
    
    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:url" content="https://yourusername.github.io/">
    <meta property="twitter:title" content="The Game Point | Ultimate Gaming Portal">
    <meta property="twitter:description" content="Get real-time gaming updates and professional walkthroughs.">
    <meta property="twitter:image" content="https://images.unsplash.com/photo-1542751371-adc38448a05e?w=800">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0"

    <!-- FONTS: Orbitron for Headers, Inter for Body -->
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
    
    <!-- ICONS: Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        /* --- CSS VARIABLES (Easy to change colors) --- */
        :root {
            --neon-blue: #00f2ff;
            --neon-purple: #bc13fe;
            --dark-bg: #050505;
            --card-bg: #111111;
            --header-gradient: linear-gradient(180deg, #1f2833 0%, #000 100%);
            --transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        /* --- RESET & GLOBAL STYLES --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--dark-bg);
            color: #e0e0e0;
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* --- STICKY NAVIGATION --- */
        nav.main-nav {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: rgba(0, 0, 0, 0.8);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid rgba(0, 242, 255, 0.2);
            padding: 15px 0;
        }

        .nav-container {
            max-width: 1300px;
            margin: 0 auto;
            display: flex;
            justify-content: center;
            gap: 40px;
        }

        .nav-container a {
            font-family: 'Orbitron', sans-serif;
            color: #fff;
            text-decoration: none;
            font-size: 0.9rem;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 2px;
            transition: var(--transition);
        }

        .nav-container a:hover {
            color: var(--neon-blue);
            text-shadow: 0 0 10px var(--neon-blue);
        }

        /* --- HEADER SECTION --- */
        header {
            background: var(--header-gradient);
            padding: 80px 20px;
            text-align: center;
            border-bottom: 5px solid var(--neon-blue);
            position: relative;
        }

        header::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 100%;
            height: 10px;
            background: var(--neon-blue);
            filter: blur(15px);
            opacity: 0.5;
        }

        header h1 {
            font-family: 'Orbitron', sans-serif;
            font-size: 6rem; /* Billion dollar bold italic heading */
            font-weight: 900;
            font-style: italic;
            margin: 0;
            color: var(--neon-blue);
            text-transform: uppercase;
            letter-spacing: 15px;
            text-shadow: 0 0 20px var(--neon-blue), 0 0 40px rgba(0, 242, 255, 0.5);
            animation: neonPulse 2s infinite alternate;
        }

        @keyframes neonPulse {
            from { text-shadow: 0 0 15px var(--neon-blue), 0 0 30px var(--neon-blue); transform: scale(1); }
            to { text-shadow: 0 0 25px var(--neon-blue), 0 0 50px var(--neon-blue), 0 0 70px var(--neon-blue); transform: scale(1.02); }
        }

        /* --- AUTO-SLIDING CAROUSEL --- */
        .slider-section {
            padding: 50px 0;
        }

        .slider-container {
            width: 95%;
            max-width: 1400px;
            margin: 0 auto;
            position: relative;
            overflow: hidden;
            border-radius: 40px;
            border: 2px solid #222;
            box-shadow: 0 20px 50px rgba(0,0,0,0.8);
        }

        .slider {
            display: flex;
            transition: transform 1s cubic-bezier(0.85, 0, 0.15, 1);
        }

        .slide {
            min-width: 100%;
            height: 600px;
            position: relative;
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: flex-end;
        }

        .slide-overlay {
            width: 100%;
            padding: 80px 50px;
            background: linear-gradient(to top, rgba(0,0,0,1) 10%, transparent);
            text-align: center;
        }

        .slide-overlay h2 {
            font-family: 'Orbitron', sans-serif;
            font-size: 2.2rem; /* Adjusted as per request */
            color: #fff;
            text-transform: uppercase;
            letter-spacing: 4px;
            margin-bottom: 15px;
            text-shadow: 2px 2px 10px #000;
        }

        .badge {
            background: var(--neon-blue);
            color: #000;
            padding: 5px 15px;
            font-family: 'Orbitron', sans-serif;
            font-weight: 900;
            font-size: 0.8rem;
            border-radius: 5px;
            margin-bottom: 20px;
            display: inline-block;
        }

        /* --- MAIN CONTENT & BLOG LIST --- */
        .container {
            max-width: 1300px;
            width: 95%;
            margin: 80px auto;
        }

        .section-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 3rem;
            color: #fff;
            text-align: center;
            margin-bottom: 60px;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 100px;
            height: 4px;
            background: var(--neon-blue);
            margin: 15px auto;
        }

        .blog-list {
            display: flex;
            flex-direction: column;
            gap: 80px;
        }

        /* ZIG-ZAG LAYOUT WITH CENTRED CONTENT */
        .card {
            display: flex;
            background-color: var(--card-bg);
            border-radius: 40px; /* Modern Rounded */
            overflow: hidden;
            border: 1px solid #222;
            transition: var(--transition);
            align-items: center;
        }

        .card:nth-child(even) {
            flex-direction: row-reverse;
        }

        .card:hover {
            border-color: var(--neon-blue);
            box-shadow: 0 0 40px rgba(0,242,255,0.2);
            transform: translateY(-10px);
        }

        .card-img {
            flex: 1.2;
            height: 500px;
            overflow: hidden;
            position: relative;
        }

        .card-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: 1s;
        }

        .card:hover .card-img img {
            transform: scale(1.1) rotate(2deg);
        }

        .card-content {
            flex: 1;
            padding: 60px;
            text-align: center; /* Content Centred */
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .card h3 {
            font-family: 'Orbitron', sans-serif;
            font-size: 2.5rem;
            color: var(--neon-blue);
            margin-bottom: 20px;
            text-transform: uppercase;
        }

        .card p {
            color: #aaa;
            font-size: 1.1rem;
            line-height: 1.8;
            margin-bottom: 30px;
            max-width: 85%;
        }

        .btn {
            background: var(--neon-blue);
            color: #000;
            border: none;
            padding: 18px 45px;
            font-family: 'Orbitron', sans-serif;
            font-weight: 900;
            cursor: pointer;
            text-transform: uppercase;
            border-radius: 12px;
            transition: var(--transition);
            font-size: 1rem;
            letter-spacing: 2px;
        }

        .btn:hover {
            box-shadow: 0 0 30px var(--neon-blue);
            transform: scale(1.1);
            background: #fff;
        }

        /* --- PROFESSIONAL FOOTER --- */
        footer {
            background-color: #000;
            padding: 100px 20px 40px 20px;
            border-top: 5px solid var(--neon-blue);
            margin-top: 100px;
            position: relative;
        }

        .footer-grid {
            max-width: 1300px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 50px;
        }

        .footer-box h4 {
            font-family: 'Orbitron', sans-serif;
            color: #fff;
            font-size: 1.6rem;
            margin-bottom: 30px;
            text-transform: uppercase;
            border-left: 5px solid var(--neon-blue);
            padding-left: 15px;
        }

        .footer-box p {
            color: #888;
            font-size: 1rem;
            margin-bottom: 20px;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 15px;
        }

        .footer-links a {
            color: #888;
            text-decoration: none;
            transition: 0.3s;
            font-weight: 600;
        }

        .footer-links a:hover {
            color: var(--neon-blue);
            padding-left: 10px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 20px;
            color: #bbb;
        }

        .contact-item i {
            color: var(--neon-blue);
            font-size: 1.2rem;
        }

        .social-media {
            display: flex;
            gap: 20px;
            margin-top: 30px;
        }

        .social-media a {
            width: 55px;
            height: 55px;
            background: #111;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 15px;
            color: #fff;
            font-size: 1.5rem;
            text-decoration: none;
            border: 1px solid #333;
            transition: var(--transition);
        }

        .social-media a:hover {
            background: var(--neon-blue);
            color: #000;
            transform: translateY(-10px) rotate(10deg);
            box-shadow: 0 10px 20px rgba(0, 242, 255, 0.4);
        }

        .newsletter input {
            width: 100%;
            padding: 15px;
            background: #111;
            border: 1px solid #333;
            color: #fff;
            border-radius: 8px;
            margin-bottom: 15px;
        }

        .copyright {
            text-align: center;
            margin-top: 80px;
            padding-top: 40px;
            border-top: 1px solid #222;
            font-family: 'Orbitron', sans-serif;
            font-size: 0.8rem;
            color: #555;
            letter-spacing: 2px;
        }

        /* --- MOBILE OPTIMIZATION --- */
        @media (max-width: 1024px) {
            header h1 { font-size: 4rem; letter-spacing: 10px; }
            .card { flex-direction: column !important; }
            .card-img { width: 100%; height: 350px; }
            .card-content { padding: 40px 20px; }
        }

        @media (max-width: 768px) {
            header h1 { font-size: 2.5rem; letter-spacing: 5px; }
            .slide { height: 400px; }
            .slide-overlay h2 { font-size: 1.4rem; }
            .nav-container { gap: 15px; }
            .nav-container a { font-size: 0.7rem; }
        }
    </style>
</head>
<body>

    <!-- STICKY NAV -->
    <nav class="main-nav">
        <div class="nav-container">
            <a href="#home">Home</a>
            <a href="#news">News</a>
            <a href="#guides">Guides</a>
            <a href="#hardware">Hardware</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>

    <!-- HEADER -->
    <header id="home">
        <h1>The Game Point</h1>
    </header>

    <!-- AUTO-SLIDING NEWS -->
    <section class="slider-section">
        <div class="slider-container">
            <div class="slider" id="mainSlider">
                <!-- Slides Generated by JS -->
            </div>
        </div>
    </section>

    <!-- MAIN BLOG SECTION -->
    <div class="container" id="news">
        <h2 class="section-title">Latest Gaming Feed</h2>
        <div class="blog-list" id="blogGrid">
            <!-- Blogs Generated by JS -->
        </div>
    </div>

    <!-- PRO FOOTER -->
    <footer id="contact">
        <div class="footer-grid">
            <!-- Box 1: Brand Info -->
            <div class="footer-box">
                <h4>The Game Point</h4>
                <p>Experience gaming news like never before. We bring you the latest leaks, pro strategies, and the most honest hardware reviews in the industry.</p>
                <div class="newsletter">
                    <input type="email" placeholder="Enter your email for updates...">
                    <button class="btn" style="padding: 10px 20px; font-size: 0.8rem;">Subscribe</button>
                </div>
            </div>

            <!-- Box 2: Quick Links -->
            <div class="footer-box">
                <h4>Navigation</h4>
                <ul class="footer-links">
                    <li><a href="#home">Home Base</a></li>
                    <li><a href="#news">Daily News</a></li>
                    <li><a href="#guides">Pro Walkthroughs</a></li>
                    <li><a href="#hardware">Gear Reviews</a></li>
                    <li><a href="#">Privacy Policy</a></li>
                </ul>
            </div>

            <!-- Box 3: Contact Details -->
            <div class="footer-box">
                <h4>Contact Info</h4>
                <div class="contact-item">
                    <i class="fas fa-envelope"></i>
                    <span>support@thegamepoint.com</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-phone-alt"></i>
                    <span>+91 88888 99999</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-map-marker-alt"></i>
                    <span>Cyber City, Gaming Zone, India</span>
                </div>
            </div>

            <!-- Box 4: Social Connectivity -->
            <div class="footer-box">
                <h4>Follow The Journey</h4>
                <p>Join our community of 1M+ gamers across social platforms.</p>
                <div class="social-media">
                    <a href="https://youtube.com" target="_blank"><i class="fab fa-youtube"></i></a>
                    <a href="https://instagram.com" target="_blank"><i class="fab fa-instagram"></i></a>
                    <a href="https://twitter.com" target="_blank"><i class="fab fa-x-twitter"></i></a>
                    <a href="#"><i class="fab fa-discord"></i></a>
                </div>
            </div>
        </div>

        <div class="copyright">
            &copy; 2024 THE GAME POINT PORTAL | ENGINE POWERED BY GAMING SPIRIT
        </div>
    </footer>

    <!-- JAVASCRIPT: Logic for Slider and Dynamic Blogs -->
    <script>
        // 1. DATA CENTER: Change your content here
        const sliderData = [
            { category: "TRENDING", title: "GTA 6: NEW MAP LEAKS CONFIRMED", img: "https://images.unsplash.com/photo-1544006659-f0b21f04cb1d?w=1400" },
            { category: "HARDWARE", title: "RTX 5090: THE FUTURE OF 8K GAMING", img: "https://images.unsplash.com/photo-1587202372775-e229f172b9d7?w=1400" },
            { category: "ESPORTS", title: "VALORANT CHAMPIONS 2024 FINALS", img: "https://images.unsplash.com/photo-1542751371-adc38448a05e?w=1400" },
            { category: "CONSOLES", title: "PS5 PRO: SPECS VS REALITY", img: "https://images.unsplash.com/photo-1606144042614-b2417e99c4e3?w=1400" }
        ];

        const blogData = [
            { 
                title: "Mastering Valorant Aim", 
                text: "Unlock your full potential with our comprehensive aim guide. We cover everything from mouse DPI settings to advanced flick-shot techniques used by the pros. Learn how to hold angles and clear sites with pixel-perfect precision.", 
                img: "https://images.unsplash.com/photo-1542751371-adc38448a05e?w=800" 
            },
            { 
                title: "Top 5 Gaming PCs 2024", 
                text: "Don't waste your money on overpriced pre-builds. We analyzed the top 5 gaming rigs that offer the best price-to-performance ratio for 4K ultra gaming. See which one fits your budget and dominates the leaderboards.", 
                img: "https://images.unsplash.com/photo-1591488320449-011701bb6704?w=800" 
            },
            { 
                title: "The Future of VR Gaming", 
                text: "Virtual Reality is evolving faster than ever. With haptic suits and 8K lenses, the boundary between reality and games is blurring. Discover the upcoming titles that will change the way you perceive the digital world.", 
                img: "https://images.unsplash.com/photo-1622979135225-d2ba269cf1ac?w=800" 
            },
            { 
                title: "BGMI: Pro Survival Tips", 
                text: "Survival is an art. In this guide, we reveal the top-secret drop locations and rotation strategies that will help you reach the final circle every single time. Conquer the battleground with elite tactical knowledge.", 
                img: "https://images.unsplash.com/photo-1509198397868-475647b2a1e5?w=800" 
            }
        ];

        // 2. RENDER SLIDER
        const sliderEl = document.getElementById('mainSlider');
        sliderData.forEach(slide => {
            sliderEl.innerHTML += `
                <div class="slide" style="background-image: url('${slide.img}')">
                    <div class="slide-overlay">
                        <span class="badge">${slide.category}</span>
                        <h2>${slide.title}</h2>
                        <button class="btn" style="padding: 10px 25px;">View News</button>
                    </div>
                </div>`;
        });

        // 3. RENDER BLOGS (Alternating Left-Right)
        const blogEl = document.getElementById('blogGrid');
        blogData.forEach(blog => {
            blogEl.innerHTML += `
                <div class="card">
                    <div class="card-img"><img src="${blog.img}" alt="Gaming News"></div>
                    <div class="card-content">
                        <h3>${blog.title}</h3>
                        <p>${blog.text}</p>
                        <button class="btn">Read Full Article</button>
                    </div>
                </div>`;
        });

        // 4. AUTO-SLIDE LOGIC
        let currentSlide = 0;
        function slideNext() {
            currentSlide = (currentSlide + 1) % sliderData.length;
            sliderEl.style.transform = `translateX(-${currentSlide * 100}%)`;
        }
        setInterval(slideNext, 5000); // Swaps every 5 seconds for better engagement

        // 5. SMOOTH REVEAL ANIMATION ON SCROLL
        const observerOptions = { threshold: 0.1 };
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if(entry.isIntersecting) {
                    entry.target.style.opacity = "1";
                    entry.target.style.transform = "translateY(0)";
                }
            });
        }, observerOptions);

        document.querySelectorAll('.card').forEach(card => {
            card.style.opacity = "0";
            card.style.transform = "translateY(50px)";
            card.style.transition = "all 0.8s ease-out";
            observer.observe(card);
        });

    </script>
</body>
</html>
