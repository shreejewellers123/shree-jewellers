<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>श्री Jewellers — Mandvi, Kutch</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;1,400&family=Jost:wght@300;400;500;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        html {
            scroll-behavior: smooth;
        }
        body {
            background: #171310;
            color: #f2e9da;
            font-family: 'Jost', sans-serif;
            font-weight: 300;
            overflow-x: hidden;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 24px;
        }
        h1, h2, h3 {
            font-family: 'Cormorant Garamond', serif;
            font-weight: 500;
            letter-spacing: 0.02em;
        }
        .eyebrow {
            font-family: 'Jost', sans-serif;
            font-size: 0.72rem;
            letter-spacing: 0.3em;
            text-transform: uppercase;
            color: #c8a15a;
        }
        a {
            color: inherit;
            text-decoration: none;
        }
        img {
            max-width: 100%;
            display: block;
        }

        /* HEADER */
        header {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 50;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 18px 5vw;
            background: rgba(23, 19, 16, 0.92);
            backdrop-filter: blur(6px);
            border-bottom: 1px solid rgba(200, 161, 90, 0.15);
        }
        .logo {
            font-family: 'Cormorant Garamond', serif;
            font-size: 1.6rem;
            letter-spacing: 0.08em;
        }
        .logo span {
            color: #c8a15a;
        }
        nav {
            display: flex;
            gap: 32px;
        }
        nav a {
            font-size: 0.75rem;
            letter-spacing: 0.15em;
            text-transform: uppercase;
            color: #c9bfae;
            transition: 0.3s;
        }
        nav a:hover {
            color: #e6c98a;
        }

        /* HERO */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 120px 24px 80px;
            background: radial-gradient(ellipse at 50% 0%, rgba(200, 161, 90, 0.12), transparent 60%),
                        linear-gradient(180deg, #171310 0%, #1c1712 100%);
            border-bottom: 1px solid rgba(200, 161, 90, 0.1);
        }
        .hero .container {
            max-width: 820px;
        }
        .hero h1 {
            font-size: clamp(2.8rem, 7vw, 5rem);
            line-height: 1.05;
        }
        .hero h1 em {
            font-style: italic;
            color: #e6c98a;
        }
        .hero p {
            margin-top: 24px;
            color: #c9bfae;
            font-size: 1.05rem;
            line-height: 1.7;
        }
        .btn-group {
            margin-top: 40px;
            display: flex;
            gap: 16px;
            flex-wrap: wrap;
            justify-content: center;
        }
        .btn {
            display: inline-block;
            padding: 14px 32px;
            font-size: 0.75rem;
            letter-spacing: 0.2em;
            text-transform: uppercase;
            border: 1px solid #c8a15a;
            color: #e6c98a;
            transition: 0.3s;
            background: transparent;
            cursor: pointer;
        }
        .btn:hover {
            background: #c8a15a;
            color: #171310;
        }
        .btn-primary {
            background: #c8a15a;
            color: #171310;
        }
        .btn-primary:hover {
            background: #e6c98a;
            color: #171310;
        }

        /* PRICE BAR */
        .price-bar {
            background: #211b16;
            padding: 20px 0;
            border-top: 1px solid rgba(200, 161, 90, 0.15);
            border-bottom: 1px solid rgba(200, 161, 90, 0.15);
            text-align: center;
        }
        .price-bar .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 24px 48px;
        }
        .price-bar .item {
            font-size: 0.95rem;
            letter-spacing: 0.05em;
        }
        .price-bar .item span {
            color: #e6c98a;
            font-weight: 600;
            font-size: 1.1rem;
        }

        /* ABOUT */
        .about {
            background: #211b16;
            padding: 80px 0;
        }
        .about .container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }
        .about .frame {
            aspect-ratio: 4/5;
            border: 1px solid rgba(200, 161, 90, 0.2);
            padding: 12px;
        }
        .about .frame .inner {
            height: 100%;
            width: 100%;
            background: url('https://i.ibb.co/7JVwXs0j/IMG-20260709-WA0006.jpg') center/cover no-repeat;
        }
        .about .copy h2 {
            font-size: clamp(1.8rem, 3vw, 2.6rem);
            margin-top: 8px;
            margin-bottom: 20px;
        }
        .about .copy p {
            color: #c9bfae;
            line-height: 1.8;
            margin-bottom: 16px;
        }
        .stats {
            display: flex;
            gap: 40px;
            margin-top: 30px;
            flex-wrap: wrap;
        }
        .stats h3 {
            color: #e6c98a;
            font-size: 1.8rem;
        }
        .stats span {
            font-size: 0.7rem;
            letter-spacing: 0.1em;
            text-transform: uppercase;
            color: #c9bfae;
        }

        /* GALLERY */
        #gallery {
            background: #1a1613;
            padding: 80px 0;
        }
        .section-head {
            text-align: center;
            max-width: 600px;
            margin: 0 auto 48px;
        }
        .section-head h2 {
            font-size: clamp(2rem, 4vw, 2.8rem);
            margin-top: 10px;
        }
        .section-head p {
            color: #c9bfae;
            margin-top: 14px;
            line-height: 1.7;
        }
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 24px;
        }
        .card {
            border: 1px solid rgba(200, 161, 90, 0.15);
            background: rgba(200, 161, 90, 0.03);
            transition: 0.3s;
        }
        .card:hover {
            transform: translateY(-4px);
            border-color: rgba(200, 161, 90, 0.4);
        }
        .card .thumb {
            aspect-ratio: 1/1;
            overflow: hidden;
            background: #211b16;
            border-bottom: 1px solid rgba(200, 161, 90, 0.1);
        }
        .card .thumb img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .card .info {
            padding: 20px 20px 24px;
        }
        .card .info .eyebrow {
            font-size: 0.6rem;
        }
        .card .info h3 {
            font-size: 1.3rem;
            margin-top: 6px;
        }
        .card .info .price {
            color: #e6c98a;
            margin-top: 8px;
            font-size: 0.95rem;
        }
        .card .info .enquire {
            display: inline-block;
            margin-top: 14px;
            font-size: 0.7rem;
            letter-spacing: 0.15em;
            text-transform: uppercase;
            color: #c8a15a;
            border-bottom: 1px solid rgba(200, 161, 90, 0.3);
            padding-bottom: 4px;
        }
        .card .info .enquire:hover {
            color: #e6c98a;
        }

        /* CONTACT */
        .contact {
            background: #211b16;
            padding: 80px 0;
            text-align: center;
        }
        .contact .container {
            max-width: 600px;
        }
        .contact .info p {
            margin: 14px 0;
            font-size: 1rem;
            color: #c9bfae;
        }
        .contact .info i {
            color: #c8a15a;
            margin-right: 10px;
            width: 22px;
        }
        .social-links {
            display: flex;
            justify-content: center;
            gap: 16px;
            margin: 28px 0;
        }
        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            border: 1px solid #c8a15a;
            color: #e6c98a;
            font-size: 1.3rem;
            transition: 0.3s;
        }
        .social-links a:hover {
            background: #c8a15a;
            color: #171310;
        }
        .whatsapp-btn, .insta-btn {
            display: inline-block;
            padding: 12px 30px;
            border-radius: 50px;
            font-weight: 600;
            margin: 6px;
            transition: 0.3s;
        }
        .whatsapp-btn {
            background: #25D366;
            color: #fff;
        }
        .whatsapp-btn:hover {
            background: #1ebc5a;
            transform: translateY(-2px);
        }
        .insta-btn {
            background: #d62976;
            color: #fff;
        }
        .insta-btn:hover {
            background: #c01e65;
            transform: translateY(-2px);
        }
        .map-container {
            margin-top: 30px;
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid rgba(200, 161, 90, 0.15);
        }
        .map-container iframe {
            width: 100%;
            height: 260px;
            border: 0;
            display: block;
        }

        /* FOOTER */
        footer {
            background: #171310;
            padding: 60px 0 30px;
            border-top: 1px solid rgba(200, 161, 90, 0.1);
        }
        footer .container {
            display: grid;
            grid-template-columns: 1.4fr 1fr 1fr;
            gap: 40px;
        }
        footer .logo {
            font-size: 1.4rem;
        }
        footer p {
            color: #c9bfae;
            font-size: 0.9rem;
            line-height: 1.7;
            margin-top: 10px;
        }
        footer h4 {
            font-size: 0.7rem;
            letter-spacing: 0.2em;
            text-transform: uppercase;
            color: #c8a15a;
            margin-bottom: 16px;
            font-weight: 400;
        }
        footer a {
            display: block;
            color: #c9bfae;
            font-size: 0.9rem;
            margin-bottom: 8px;
        }
        footer a:hover {
            color: #e6c98a;
        }
        .footer-bottom {
            text-align: center;
            margin-top: 50px;
            padding-top: 20px;
            border-top: 1px solid rgba(200, 161, 90, 0.08);
            font-size: 0.75rem;
            color: #8a7a6a;
            grid-column: 1 / -1;
        }

        /* RESPONSIVE */
        @media (max-width: 820px) {
            nav {
                display: none;
            }
            .about .container {
                grid-template-columns: 1fr;
                gap: 40px;
            }
            footer .container {
                grid-template-columns: 1fr;
                gap: 30px;
            }
            .gallery-grid {
                grid-template-columns: 1fr 1fr;
            }
            .price-bar .container {
                gap: 12px 20px;
            }
        }
        @media (max-width: 480px) {
            .gallery-grid {
                grid-template-columns: 1fr;
            }
            .container {
                padding: 0 16px;
            }
            .hero {
                padding: 100px 16px 60px;
            }
            .btn {
                padding: 12px 24px;
                font-size: 0.7rem;
            }
            .price-bar .item {
                font-size: 0.8rem;
            }
        }
    </style>
</head>
<body>

<header>
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
        <div class="btn-group">
            <a href="#gallery" class="btn btn-primary">View Collection</a>
            <a href="#contact" class="btn">Book a Visit</a>
        </div>
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
            <div class="stats">
                <div><h3>BIS</h3><span>Hallmarked Gold</span></div>
                <div><h3>100%</h3><span>Handcrafted</span></div>
                <div><h3>Direct</h3><span>Karigar Pricing</span></div>
            </div>
        </div>
    </div>
</section>

<!-- GALLERY -->
<section id="gallery">
    <div class="container">
        <div class="section-head">
            <div class="eyebrow">Our Collection</div>
            <h2>Handcrafted for every occasion</h2>
            <p>Each piece is unique — crafted with care and precision by our master artisans.</p>
        </div>
        <div class="gallery-grid">
            <!-- Card 1 -->
            <div class="card">
                <div class="thumb"><img src="https://i.ibb.co/0jmq2M9S/motion-photo-1551257267689762343.jpg" alt="Gold Jewellery"></div>
                <div class="info">
                    <div class="eyebrow">Gold Jewellery</div>
                    <h3>Gold Jewellery</h3>
                    <div class="price">₹ 85,000 – 1,20,000</div>
                    <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery." target="_blank" class="enquire">Enquire →</a>
                </div>
            </div>
            <!-- Card 2 -->
            <div class="card">
                <div class="thumb"><img src="https://i.ibb.co/nNHvbTkR/IMG-20260709-WA0008.jpg" alt="Gold Jewellery"></div>
                <div class="info">
                    <div class="eyebrow">Gold Jewellery</div>
                    <h3>Gold Jewellery</h3>
                    <div class="price">₹ 1,40,000 – 2,10,000</div>
                    <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery." target="_blank" class="enquire">Enquire →</a>
                </div>
            </div>
            <!-- Card 3 -->
            <div class="card">
                <div class="thumb"><img src="https://i.ibb.co/rKBR6VKp/IMG-20260709-WA0007.jpg" alt="Gold Jewellery"></div>
                <div class="info">
                    <div class="eyebrow">Gold Jewellery</div>
                    <h3>Gold Jewellery</h3>
                    <div class="price">₹ 22,000 – 38,000</div>
                    <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery." target="_blank" class="enquire">Enquire →</a>
                </div>
            </div>
            <!-- Card 4 -->
            <div class="card">
                <div class="thumb"><img src="https://i.ibb.co/KjZ3NDFG/IMG-20260709-WA0011.jpg" alt="Gold Jewellery"></div>
                <div class="info">
                    <div class="eyebrow">Gold Jewellery</div>
                    <h3>Gold Jewellery</h3>
                    <div class="price">₹ 40,000 – 60,000</div>
                    <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery." target="_blank" class="enquire">Enquire →</a>
                </div>
            </div>
            <!-- Card 5 -->
            <div class="card">
                <div class="thumb"><img src="https://i.ibb.co/V0smJjkH/IMG-20260709-WA0013.jpg" alt="Gold Jewellery"></div>
                <div class="info">
                    <div class="eyebrow">Gold Jewellery</div>
                    <h3>Gold Jewellery</h3>
                    <div class="price">₹ 65,000 – 95,000</div>
                    <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery." target="_blank" class="enquire">Enquire →</a>
                </div>
            </div>
            <!-- Card 6 -->
            <div class="card">
                <div class="thumb"><img src="https://i.ibb.co/S7yqQ8Tw/IMG-20260709-WA0012.jpg" alt="Gold Jewellery"></div>
                <div class="info">
                    <div class="eyebrow">Gold Jewellery</div>
                    <h3>Gold Jewellery</h3>
                    <div class="price">₹ 48,000 – 70,000</div>
                    <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery." target="_blank" class="enquire">Enquire →</a>
                </div>
            </div>
            <!-- Card 7 -->
            <div class="card">
                <div class="thumb"><img src="https://i.ibb.co/KjHXPPxW/IMG-20260709-WA0018.jpg" alt="Gold Jewellery"></div>
                <div class="info">
                    <div class="eyebrow">Gold Jewellery</div>
                    <h3>Gold Jewellery</h3>
                    <div class="price">₹ 30,000 – 55,000</div>
                    <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery." target="_blank" class="enquire">Enquire →</a>
                </div>
            </div>
            <!-- Card 8 -->
            <div class="card">
                <div class="thumb"><img src="https://i.ibb.co/hFDST0rg/IMG-20260709-WA0016.jpg" alt="Gold Jewellery"></div>
                <div class="info">
                    <div class="eyebrow">Gold Jewellery</div>
                    <h3>Gold Jewellery</h3>
                    <div class="price">₹ 26,000 – 42,000</div>
                    <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery." target="_blank" class="enquire">Enquire →</a>
                </div>
            </div>
            <!-- Card 9 -->
            <div class="card">
                <div class="thumb"><img src="https://i.ibb.co/XZvkjfW2/IMG-20260709-WA0017.jpg" alt="Gold Jewellery"></div>
                <div class="info">
                    <div class="eyebrow">Gold Jewellery</div>
                    <h3>Gold Jewellery</h3>
                    <div class="price">₹ 52,000 – 80,000</div>
                    <a href="https://wa.me/916358158073?text=Hi%20Shree%20Jewellers%2C%20I%27m%20interested%20in%20this%20gold%20jewellery." target="_blank" class="enquire">Enquire →</a>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- CONTACT -->
<section class="contact" id="contact">
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
        </div>
        <div class="social-links">
            <a href="https://www.instagram.com/shree_jewellers_mandvikutch" target="_blank" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
            <a href="https://www.instagram.com/shree.jewellers.mandvi" target="_blank" aria-label="Instagram 2"><i class="fab fa-instagram"></i></a>
            <a href="https://wa.me/916358158073" target="_blank" aria-label="WhatsApp"><i class="fab fa-whatsapp"></i></a>
        </div>
        <div>
            <a href="https://wa.me/916358158073" class="whatsapp-btn"><i class="fab fa-whatsapp"></i> Chat on WhatsApp</a>
            <a href="https://www.instagram.com/shree_jewellers_mandvikutch" target="_blank" class="insta-btn"><i class="fab fa-instagram"></i> Follow on Instagram</a>
        </div>
        <div class="map-container">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d235.88568395856213!2d69.35228715356528!3d22.831034565714705!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zMjLCsDQ5JzUxLjciTiA2OcKwMjEnMDguNSJF!5e0!3m2!1sen!2sin!4v1741600000000" allowfullscreen loading="lazy"></iframe>
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
        <div class="footer-bottom">
            © 2026 श्री Jewellers. All rights reserved. Crafted with love in Kutch.
        </div>
    </div>
</footer>

</body>
</html>
