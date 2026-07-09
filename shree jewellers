<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>श्री Jewellers — Mandvi, Kutch</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;1,400&family=Jost:wght@300;400;500;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        :root {
            --ink: #171310;
            --ink-2: #211b16;
            --gold: #c8a15a;
            --gold-bright: #e6c98a;
            --gold-dim: #8a6f3d;
            --ivory: #f2e9da;
            --ivory-dim: #c9bfae;
            --line: rgba(200, 161, 90, 0.25);
        }
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        html { scroll-behavior: smooth; }
        body {
            background: var(--ink);
            color: var(--ivory);
            font-family: 'Jost', sans-serif;
            font-weight: 300;
            overflow-x: hidden;
        }
        h1, h2, h3, .serif {
            font-family: 'Cormorant Garamond', serif;
            font-weight: 500;
            letter-spacing: 0.02em;
        }
        .eyebrow {
            font-family: 'Jost', sans-serif;
            font-size: 0.72rem;
            letter-spacing: 0.35em;
            text-transform: uppercase;
            color: var(--gold);
        }
        a { color: inherit; text-decoration: none; }
        img { max-width: 100%; display: block; }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .motif {
            width: 64px; height: 64px;
            margin: 0 auto;
            opacity: 0.9;
        }
        .motif path {
            fill: none;
            stroke: var(--gold);
            stroke-width: 1.1;
        }

        /* Header */
        header {
            position: fixed; top: 0; left: 0; right: 0; z-index: 50;
            display: flex; align-items: center; justify-content: space-between;
            padding: 22px 6vw;
            background: linear-gradient(180deg, rgba(23, 19, 16, 0.95), rgba(23, 19, 16, 0));
            transition: background 0.4s ease;
        }
        header.scrolled { background: rgba(23, 19, 16, 0.92); backdrop-filter: blur(6px); border-bottom: 1px solid var(--line); }
        .logo {
            font-family: 'Cormorant Garamond', serif;
            font-size: 1.8rem;
            letter-spacing: 0.08em;
        }
        .logo span { color: var(--gold); }
        nav { display: flex; gap: 38px; }
        nav a {
            font-size: 0.78rem;
            letter-spacing: 0.18em;
            text-transform: uppercase;
            color: var(--ivory-dim);
            position: relative;
            padding-bottom: 4px;
        }
        nav a:hover { color: var(--gold-bright); }

        /* Hero */
        .hero {
            min-height: 100svh;
            display: flex; flex-direction: column; align-items: center; justify-content: center;
            text-align: center;
            padding: 140px 6vw 80px;
            position: relative;
            background:
                radial-gradient(ellipse at 50% 0%, rgba(200, 161, 90, 0.15), transparent 60%),
                linear-gradient(180deg, var(--ink) 0%, #1c1712 100%);
        }
        .hero::before {
            content: "";
            position: absolute; inset: 14px;
            border: 1px solid var(--line);
            pointer-events: none;
        }
        .hero .container {
            max-width: 800px;
        }
        .hero h1 {
            font-size: clamp(2.6rem, 6.5vw, 5.2rem);
            line-height: 1.05;
        }
        .hero h1 em {
            font-style: italic;
            color: var(--gold-bright);
        }
        .hero p {
            margin-top: 26px;
            color: var(--ivory-dim);
            font-size: 1.05rem;
            line-height: 1.7;
        }
        .cta-row {
            margin-top: 44px;
            display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;
        }
        .btn {
            display: inline-block;
            padding: 15px 34px;
            font-size: 0.78rem;
            letter-spacing: 0.2em;
            text-transform: uppercase;
            border: 1px solid var(--gold);
            color: var(--gold-bright);
            transition: all 0.3s ease;
            background: transparent;
            cursor: pointer;
        }
        .btn:hover { background: var(--gold); color: var(--ink); }
        .btn.solid { background: var(--gold); color: var(--ink); }
        .btn.solid:hover { background: var(--gold-bright); }

        .hero .motif { margin-top: 56px; }

        /* Price Bar */
        .price-bar {
            background: var(--ink-2);
            padding: 25px 0;
            border-top: 1px solid var(--line);
            border-bottom: 1px solid var(--line);
            text-align: center;
        }
        .price-bar .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px 50px;
        }
        .price-bar .item {
            font-size: 1rem;
            letter-spacing: 0.05em;
        }
        .price-bar .item span {
            color: var(--gold-bright);
            font-weight: 600;
            font-size: 1.2rem;
        }

        /* Sections */
        section { padding: 110px 0; }
        .section-head { text-align: center; max-width: 640px; margin: 0 auto 64px; }
        .section-head h2 { font-size: clamp(2rem, 4vw, 3rem); margin-top: 16px; }
        .section-head p { color: var(--ivory-dim); margin-top: 18px; line-height: 1.7; }

        /* About */
        .about {
            background: var(--ink-2);
        }
        .about .container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 70px;
            align-items: center;
        }
        .about .frame {
            aspect-ratio: 4/5;
            border: 1px solid var(--line);
            padding: 14px;
        }
        .about .frame .inner {
            height: 100%; width: 100%;
            background: url('https://i.ibb.co/7JVwXs0j/IMG-20260709-WA0006.jpg') center/cover no-repeat;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--ivory-dim);
            font-size: 0.8rem;
            letter-spacing: 0.1em;
            text-transform: uppercase;
            text-align: center;
            padding: 20px;
        }
        .about .copy .eyebrow { margin-bottom: 18px; }
        .about .copy h2 { font-size: clamp(1.8rem, 3vw, 2.6rem); margin-bottom: 22px; }
        .about .copy p { color: var(--ivory-dim); line-height: 1.8; margin-bottom: 16px; }
        .stat-row { display: flex; gap: 44px; margin-top: 34px; flex-wrap: wrap; }
        .stat h3 { color: var(--gold-bright); font-size: 2rem; }
        .stat span { font-size: 0.7rem; letter-spacing: 0.14em; text-transform: uppercase; color: var(--ivory-dim); }

        /* Gallery */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            margin-top: 40px;
            max-width: 1200px;
            margin-left: auto;
            margin-right: auto;
            padding: 0 20px;
        }
        .card {
            border: 1px solid var(--line);
            background: linear-gradient(180deg, rgba(200, 161, 90, 0.04), transparent);
            transition: transform 0.35s ease, border-color 0.35s ease;
            max-width: 100%;
        }
        .card:hover { transform: translateY(-6px); border-color: var(--gold-dim); }
        .card .thumb {
            aspect-ratio: 1/1;
            display: flex;
            align-items: center;
            justify-content: center;
            background:
                radial-gradient(circle at 30% 20%, rgba(230, 201, 138, 0.18), transparent 55%),
                linear-gradient(135deg, #2a2219, #171310);
            border-bottom: 1px solid var(--line);
            position: relative;
            overflow: hidden;
        }
        .card .thumb img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .card .thumb .swap-label {
            position: absolute; bottom: 10px; left: 10px; right: 10px;
            font-size: 0.62rem; letter-spacing: 0.1em; text-transform: uppercase;
            color: var(--ivory-dim); opacity: 0.55;
        }
        .card .info { padding: 24px 22px 28px; }
        .card .info .eyebrow { font-size: 0.62rem; }
        .card .info h3 { font-size: 1.4rem; margin-top: 8px; }
        .card .info .price { color: var(--gold-bright); margin-top: 10px; font-size: 0.95rem; letter-spacing: 0.03em; }
        .card .info .enquire {
            display: inline-block; margin-top: 18px;
            font-size: 0.7rem; letter-spacing: 0.16em; text-transform: uppercase;
            color: var(--gold); border-bottom: 1px solid var(--gold-dim); padding-bottom: 3px;
            cursor: pointer;
        }
        .card .info .enquire:hover { color: var(--gold-bright); border-color: var(--gold-bright); }

        /* Contact */
        .contact-section {
            background: var(--ink-2);
            text-align: center;
        }
        .contact-section .container {
            max-width: 600px;
        }
        .contact-section .info p {
            margin: 15px 0;
            font-size: 1.1rem;
            color: var(--ivory-dim);
        }
        .contact-section .info i {
            color: var(--gold);
            margin-right: 10px;
            width: 24px;
        }
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 30px 0;
        }
        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 56px;
            height: 56px;
            border-radius: 50%;
            border: 1px solid var(--gold);
            color: var(--gold-bright);
            font-size: 1.5rem;
            transition: all 0.3s ease;
        }
        .social-links a:hover {
            background: var(--gold);
            color: var(--ink);
            transform: translateY(-3px);
        }
        .whatsapp-btn {
            display: inline-block;
            background: #25D366;
            color: white;
            padding: 14px 35px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 700;
            margin-top: 20px;
            box-shadow: 0 8px 30px rgba(37, 211, 102, 0.3);
            transition: 0.3s;
        }
        .whatsapp-btn:hover { transform: translateY(-3px); background: #1ebc5a; }
        .insta-btn {
            display: inline-block;
            background: #d62976;
            color: white;
            padding: 14px 35px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 700;
            margin: 10px 10px;
            box-shadow: 0 8px 30px rgba(214, 41, 118, 0.3);
            transition: 0.3s;
        }
        .insta-btn:hover { transform: translateY(-3px); background: #c01e65; }
        .map-container {
            border: 1px solid var(--line);
            border-radius: 15px;
            overflow: hidden;
            margin-top: 30px;
        }
        iframe { display: block; width: 100%; height: 300px; border: 0; }

        /* Footer */
        footer {
            padding: 70px 0 40px;
            border-top: 1px solid var(--line);
        }
        footer .container {
            display: grid;
            grid-template-columns: 1.4fr 1fr 1fr;
            gap: 50px;
        }
        footer .logo { margin-bottom: 16px; }
        footer p { color: var(--ivory-dim); font-size: 0.9rem; line-height: 1.8; }
        footer h4 {
            font-size: 0.72rem;
            letter-spacing: 0.2em;
            text-transform: uppercase;
            color: var(--gold);
            margin-bottom: 18px;
            font-weight: 400;
            font-family: 'Jost', sans-serif;
        }
        footer a { display: block; color: var(--ivory-dim); font-size: 0.9rem; margin-bottom: 10px; }
        footer a:hover { color: var(--gold-bright); }
        .foot-bottom {
            text-align: center;
            margin-top: 60px;
            padding-top: 26px;
            border-top: 1px solid var(--line);
            font-size: 0.75rem;
            color: var(--ivory-dim);
            grid-column: 1 / -1;
        }

        @media (max-width: 820px) {
            nav { display: none; }
            .about .container { grid-template-columns: 1fr; gap: 40px; }
            footer .container { grid-template-columns: 1fr; gap: 30px; }
            .gallery-grid { grid-template-columns: 1fr 1fr; padding: 0 10px; }
            .social-links { flex-wrap: wrap; }
            .price-bar .container { gap: 15px 25px; }
            .price-bar .item { font-size: 0.9rem; }
            .container { padding: 0 15px; }
        }
        @media (max-width: 480px) {
            .gallery-grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

<header id="site-header">
    <div class="logo">श्री <span>Jewellers</span></div>
    <nav>
        <a href="#about">Our Story</a>
        <a href="#gallery">Gallery</a>
        <a href="#contact">Visit Us</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<!-- HERO -->
<section class="hero">
    <div class="container">
        <h1>Jewellery carried<br><em>through generations</em></h1>
        <p>Each piece at Shree Jewellers is shaped by hand, in gold and stone, following techniques passed down across generations of our karigars.</p>
        <div class="cta-row">
            <a href="#gallery" class="btn solid">View Collection</a>
            <a href="#contact" class="btn">Book a Visit</a>
        </div>
        <svg class="motif" viewBox="0 0 64 64">
            <path d="M32 4 C 40 16, 40 24, 32 32 C 24 24, 24 16, 32 4 Z"/>
            <path d="M32 32 C 40 40, 40 48, 32 60 C 24 48, 24 40, 32 32 Z"/>
            <circle cx="32" cy="32" r="3"/>
            <path d="M8 32 C 18 28, 26 30, 32 32 C 26 34, 18 36, 8 32 Z"/>
            <path d="M56 32 C 46 28, 38 30, 32 32 C 38 34, 46 36, 56 32 Z"/>
        </svg>
    </div>
</section>

<!-- PRICE BAR -->
<div class="price-bar">
    <div class="container">
        <div class="item">18K Gold: <span>₹5,200</span> / 1g</div>
        <div class="item">22K Gold: <span>₹6,300</span> / 1g</div>
        <div class="item">24K Gold: <span>₹6,900</span> / 1g</div>
        <div class="item">Silver: <span>₹95,000</span> / 1kg</div>
    </div>
</div>

<!-- ABOUT -->
<section class="about" id="about">
    <div class="container">
        <div class="frame">
            <div class="inner"></div>
        </div>
        <div class="copy">
            <div class="eyebrow">Our Story</div>
            <h2>Rooted in Mandvi, built on trust</h2>
            <p>Shree Jewellers began as a small family counter and has grown into a name families in Kutch return to for weddings, festivals, and everyday adornment.</p>
            <p>We work directly with skilled karigars who hand-set every stone and finish every chain — no two pieces leave our counter looking machine-made.</p>
            <div class="stat-row">
                <div class="stat"><h3>BIS</h3><span>Hallmarked Gold</span></div>
                <div class="stat"><h3>100%</h3><span>Handcrafted</span></div>
                <div class="stat"><h3>Direct</h3><span>Karigar Pricing</span></div>
            </div>
        </div>
    </div>
</section>

<!-- GALLERY -->
<section id="gallery" style="background: var(--ink-2);">
    <div class="container">
        <div class="section-head">
            <div class="eyebrow">Our Collection</div>
            <h2>Handcrafted for every occasion</h2>
            <p>Each piece is unique — crafted with care and precision by our master artisans.</p>
        </div>
    </div>
    <div class="gallery-grid">
        <!-- Card 1 -->
        <div class="card">
            <div class="thumb">
                <img src="https://i.ibb.co/0jmq2M9S/motion-photo-1551257267689762343.jpg" alt="Gold Jewellery">
                <div class="swap-label">Replace with product photo</div>
            </div>
            <div class="info">
                <div class="eyebrow">Gold Jewellery</div>
                <h3>Gold Jewellery</h3>
                <div class="price">₹ 85,000 – 1,20,000</div>
                <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery.%20Please%20share%20more%20details." target="_blank" class="enquire">Enquire →</a>
            </div>
        </div>
        <!-- Card 2 -->
        <div class="card">
            <div class="thumb">
                <img src="https://i.ibb.co/nNHvbTkR/IMG-20260709-WA0008.jpg" alt="Gold Jewellery">
                <div class="swap-label">Replace with product photo</div>
            </div>
            <div class="info">
                <div class="eyebrow">Gold Jewellery</div>
                <h3>Gold Jewellery</h3>
                <div class="price">₹ 1,40,000 – 2,10,000</div>
                <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery.%20Please%20share%20more%20details." target="_blank" class="enquire">Enquire →</a>
            </div>
        </div>
        <!-- Card 3 -->
        <div class="card">
            <div class="thumb">
                <img src="https://i.ibb.co/rKBR6VKp/IMG-20260709-WA0007.jpg" alt="Gold Jewellery">
                <div class="swap-label">Replace with product photo</div>
            </div>
            <div class="info">
                <div class="eyebrow">Gold Jewellery</div>
                <h3>Gold Jewellery</h3>
                <div class="price">₹ 22,000 – 38,000</div>
                <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery.%20Please%20share%20more%20details." target="_blank" class="enquire">Enquire →</a>
            </div>
        </div>
        <!-- Card 4 -->
        <div class="card">
            <div class="thumb">
                <img src="https://i.ibb.co/KjZ3NDFG/IMG-20260709-WA0011.jpg" alt="Gold Jewellery">
                <div class="swap-label">Replace with product photo</div>
            </div>
            <div class="info">
                <div class="eyebrow">Gold Jewellery</div>
                <h3>Gold Jewellery</h3>
                <div class="price">₹ 40,000 – 60,000</div>
                <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery.%20Please%20share%20more%20details." target="_blank" class="enquire">Enquire →</a>
            </div>
        </div>
        <!-- Card 5 -->
        <div class="card">
            <div class="thumb">
                <img src="https://i.ibb.co/V0smJjkH/IMG-20260709-WA0013.jpg" alt="Gold Jewellery">
                <div class="swap-label">Replace with product photo</div>
            </div>
            <div class="info">
                <div class="eyebrow">Gold Jewellery</div>
                <h3>Gold Jewellery</h3>
                <div class="price">₹ 65,000 – 95,000</div>
                <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery.%20Please%20share%20more%20details." target="_blank" class="enquire">Enquire →</a>
            </div>
        </div>
        <!-- Card 6 -->
        <div class="card">
            <div class="thumb">
                <img src="https://i.ibb.co/S7yqQ8Tw/IMG-20260709-WA0012.jpg" alt="Gold Jewellery">
                <div class="swap-label">Replace with product photo</div>
            </div>
            <div class="info">
                <div class="eyebrow">Gold Jewellery</div>
                <h3>Gold Jewellery</h3>
                <div class="price">₹ 48,000 – 70,000</div>
                <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery.%20Please%20share%20more%20details." target="_blank" class="enquire">Enquire →</a>
            </div>
        </div>
        <!-- Card 7 -->
        <div class="card">
            <div class="thumb">
                <img src="https://i.ibb.co/KjHXPPxW/IMG-20260709-WA0018.jpg" alt="Gold Jewellery">
                <div class="swap-label">Replace with product photo</div>
            </div>
            <div class="info">
                <div class="eyebrow">Gold Jewellery</div>
                <h3>Gold Jewellery</h3>
                <div class="price">₹ 30,000 – 55,000</div>
                <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery.%20Please%20share%20more%20details." target="_blank" class="enquire">Enquire →</a>
            </div>
        </div>
        <!-- Card 8 -->
        <div class="card">
            <div class="thumb">
                <img src="https://i.ibb.co/hFDST0rg/IMG-20260709-WA0016.jpg" alt="Gold Jewellery">
                <div class="swap-label">Replace with product photo</div>
            </div>
            <div class="info">
                <div class="eyebrow">Gold Jewellery</div>
                <h3>Gold Jewellery</h3>
                <div class="price">₹ 26,000 – 42,000</div>
                <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery.%20Please%20share%20more%20details." target="_blank" class="enquire">Enquire →</a>
            </div>
        </div>
        <!-- Card 9 -->
        <div class="card">
            <div class="thumb">
                <img src="https://i.ibb.co/XZvkjfW2/IMG-20260709-WA0017.jpg" alt="Gold Jewellery">
                <div class="swap-label">Replace with product photo</div>
            </div>
            <div class="info">
                <div class="eyebrow">Gold Jewellery</div>
                <h3>Gold Jewellery</h3>
                <div class="price">₹ 52,000 – 80,000</div>
                <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery.%20Please%20share%20more%20details." target="_blank" class="enquire">Enquire →</a>
            </div>
        </div>
    </div>
</section>

<!-- CONTACT -->
<section class="contact-section" id="contact">
    <div class="container">
        <div class="section-head">
            <div class="eyebrow">Visit Us</div>
            <h2>We'd love to meet you</h2>
            <p>Visit our store in Mandvi or reach out to us online — we're here to help you find the perfect piece.</p>
        </div>
        <div class="info">
            <p><i class="fas fa-store"></i> K.T. Shah Road, near Chapra Vari Sheri, Rameshwar Colony, Mandvi, Gujarat 370465</p>
            <p><i class="fas fa-phone-alt"></i> <a href="tel:+916358158073">+91 63581 58073</a></p>
            <p><i class="fas fa-envelope"></i> <a href="mailto:shreejewellersmandvi@gmail.com">shreejewellersmandvi@gmail.com</a></p>
            <div class="social-links">
                <a href="https://www.instagram.com/shree_jewellers_mandvikutch" target="_blank" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
                <a href="https://www.instagram.com/shree.jewellers.mandvi" target="_blank" aria-label="Instagram 2"><i class="fab fa-instagram"></i></a>
                <a href="https://wa.me/916358158073" target="_blank" aria-label="WhatsApp"><i class="fab fa-whatsapp"></i></a>
            </div>
            <a href="https://wa.me/916358158073" class="whatsapp-btn"><i class="fab fa-whatsapp"></i> Chat on WhatsApp</a>
            <a href="https://www.instagram.com/shree_jewellers_mandvikutch" target="_blank" class="insta-btn"><i class="fab fa-instagram"></i> Follow on Instagram</a>

            <div class="map-container">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d235.88568395856213!2d69.35228715356528!3d22.831034565714705!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zMjLCsDQ5JzUxLjciTiA2OcKwMjEnMDguNSJF!5e0!3m2!1sen!2sin!4v1741600000000" allowfullscreen="" loading="lazy"></iframe>
            </div>
        </div>
    </div>
</section>

<!-- FOOTER -->
<footer>
    <div class="container">
        <div>
            <div class="logo">श्री <span>Jewellers</span></div>
            <p>Fine handcrafted gold and stone jewellery, made in Mandvi, Kutch for weddings, festivals, and everyday moments.</p>
        </div>
        <div>
            <h4>Visit</h4>
            <a href="#">K.T. Shah Road, Mandvi, Gujarat</a>
            <a href="#">Mon – Sat · 10:30 AM – 8:30 PM</a>
            <a href="#">Closed Sundays</a>
        </div>
        <div>
            <h4>Connect</h4>
            <a href="https://www.instagram.com/shree_jewellers_mandvikutch" target="_blank">Instagram</a>
            <a href="https://wa.me/916358158073">WhatsApp</a>
            <a href="tel:+916358158073">Call the Shop</a>
        </div>
        <div class="foot-bottom">
            © 2026 श्री Jewellers. All rights reserved. Crafted with love in Kutch.
        </div>
    </div>
</footer>

<script>
    const header = document.getElementById('site-header');
    window.addEventListener('scroll', () => {
        header.classList.toggle('scrolled', window.scrollY > 40);
    });
</script>

</body>
</html>
