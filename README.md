
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Paws & Beaks Pet Clinic | Pakistan</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&family=Roboto:wght@300;400;500&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #FF7D29;
            --secondary: #2A9D8F;
            --accent: #E76F51;
            --light: #F8F9FA;
            --dark: #264653;
            --success: #2A9D8F;
            --warning: #E9C46A;
            --danger: #E76F51;
            --rounded: 16px;
            --shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', sans-serif;
            color: #333;
            background-color: #f9f9f9;
            line-height: 1.6;
        }

        h1, h2, h3, h4, h5 {
            font-family: 'Poppins', sans-serif;
            font-weight: 600;
            color: var(--dark);
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo img {
            height: 50px;
            width: auto;
        }

        .logo h1 {
            color: white;
            font-size: 1.8rem;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 25px;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            padding: 5px 10px;
            border-radius: 20px;
        }

        nav a:hover {
            background-color: rgba(255, 255, 255, 0.2);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(42, 157, 143, 0.9), rgba(42, 157, 143, 0.8)), url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100"><rect width="100" height="100" fill="%232A9D8F"/><path d="M0 0L100 100" stroke="%23228E80" stroke-width="2"/><path d="M100 0L0 100" stroke="%23228E80" stroke-width="2"/></svg>');
            padding: 80px 0;
            text-align: center;
            color: white;
            border-radius: 0 0 var(--rounded) var(--rounded);
            margin-bottom: 40px;
        }

        .hero h2 {
            font-size: 2.8rem;
            margin-bottom: 20px;
            color: white;
            animation: fadeInDown 1s ease;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
            animation: fadeInUp 1s ease;
        }

        .btn {
            display: inline-block;
            background-color: var(--primary);
            color: white;
            padding: 12px 28px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 1.1rem;
            box-shadow: var(--shadow);
        }

        .btn:hover {
            background-color: var(--accent);
            transform: translateY(-3px);
            box-shadow: 0 12px 20px rgba(0, 0, 0, 0.15);
        }

        /* Section Styles */
        section {
            padding: 60px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }

        .section-title h2 {
            font-size: 2.2rem;
            display: inline-block;
            padding-bottom: 10px;
            position: relative;
        }

        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: var(--primary);
            border-radius: 2px;
        }

        /* Services Section */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .service-card {
            background: white;
            border-radius: var(--rounded);
            padding: 30px;
            text-align: center;
            box-shadow: var(--shadow);
            transition: all 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }

        .service-icon {
            font-size: 3.5rem;
            margin-bottom: 20px;
            color: var(--primary);
        }

        .service-card h3 {
            margin-bottom: 15px;
            font-size: 1.5rem;
        }

        /* Adoption Section */
        .adoption {
            background-color: var(--light);
        }

        .pet-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .pet-card {
            background: white;
            border-radius: var(--rounded);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: all 0.3s ease;
        }

        .pet-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 25px rgba(0, 0, 0, 0.15);
        }

        .pet-image {
            height: 200px;
            background-color: var(--secondary);
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            font-size: 4rem;
        }

        .pet-info {
            padding: 20px;
        }

        .pet-info h3 {
            margin-bottom: 10px;
            color: var(--dark);
        }

        /* Emergency Section */
        .emergency {
            text-align: center;
            background: linear-gradient(135deg, var(--secondary) 0%, var(--primary) 100%);
            color: white;
            border-radius: var(--rounded);
            padding: 60px 20px;
            margin: 40px 0;
        }

        .emergency h2 {
            color: white;
            margin-bottom: 20px;
        }

        .emergency p {
            max-width: 700px;
            margin: 0 auto 30px;
            font-size: 1.2rem;
        }

        .emergency-btn {
            background-color: white;
            color: var(--primary);
            font-size: 1.3rem;
            padding: 15px 35px;
        }

        .emergency-btn:hover {
            background-color: var(--light);
            color: var(--accent);
        }

        /* Tips Section */
        .tips-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .tip-card {
            background: white;
            border-radius: var(--rounded);
            padding: 25px;
            box-shadow: var(--shadow);
            transition: all 0.3s ease;
        }

        .tip-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 25px rgba(0, 0, 0, 0.15);
        }

        .tip-card h3 {
            color: var(--secondary);
            margin-bottom: 15px;
            font-size: 1.4rem;
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 60px 0 30px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-column h3 {
            color: white;
            margin-bottom: 20px;
            font-size: 1.4rem;
        }

        .footer-column p, .footer-column a {
            color: rgba(255, 255, 255, 0.8);
            margin-bottom: 10px;
            display: block;
            text-decoration: none;
            transition: all 0.3s ease;
        }

        .footer-column a:hover {
            color: var(--primary);
        }

        .social-icons {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-icons a {
            display: inline-flex;
            justify-content: center;
            align-items: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            transition: all 0.3s ease;
        }

        .social-icons a:hover {
            background-color: var(--primary);
            transform: translateY(-3px);
        }

        .whatsapp-btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background-color: #25D366;
            color: white;
            padding: 12px 25px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            margin-top: 15px;
        }

        .whatsapp-btn:hover {
            background-color: #128C7E;
            transform: translateY(-3px);
        }

        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: rgba(255, 255, 255, 0.6);
            font-size: 0.9rem;
        }

        /* Animations */
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                gap: 15px;
            }

            nav ul {
                gap: 15px;
                flex-wrap: wrap;
                justify-content: center;
            }

            .hero h2 {
                font-size: 2.2rem;
            }

            .hero p {
                font-size: 1rem;
            }

            .section-title h2 {
                font-size: 1.8rem;
            }
        }

        @media (max-width: 480px) {
            .logo h1 {
                font-size: 1.5rem;
            }

            nav ul {
                gap: 10px;
            }

            nav a {
                font-size: 0.9rem;
            }

            .hero h2 {
                font-size: 1.8rem;
            }

            .btn {
                padding: 10px 20px;
                font-size: 1rem;
            }

            .service-icon {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <div class="logo">
                <i class="fas fa-paw" style="color: white; font-size: 2rem;"></i>
                <h1>Paws & Beaks</h1>
            </div>
            <nav>
                <ul>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#adoption">Adoption</a></li>
                    <li><a href="#emergency">Emergency</a></li>
                    <li><a href="#tips">Pet Care Tips</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h2>Your Pet's Health is Our Priority</h2>
            <p>At Paws & Beaks, we provide compassionate and comprehensive veterinary care for your furry, feathery, and scaly family members across Pakistan.</p>
            <a href="#contact" class="btn">Book an Appointment</a>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services">
        <div class="container">
            <div class="section-title">
                <h2>Our Services</h2>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-stethoscope"></i>
                    </div>
                    <h3>Health Checkups</h3>
                    <p>Regular wellness exams to keep your pet in optimal health and catch potential issues early.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-syringe"></i>
                    </div>
                    <h3>Vaccinations</h3>
                    <p>Complete vaccination protocols for dogs, cats, and birds to protect against common diseases.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-cut"></i>
                    </div>
                    <h3>Grooming</h3>
                    <p>Professional grooming services to keep your pet looking and feeling their best.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-bone"></i>
                    </div>
                    <h3>Dental Care</h3>
                    <p>Comprehensive dental services including cleaning, extractions, and oral health education.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Adoption Section -->
    <section id="adoption" class="adoption">
        <div class="container">
            <div class="section-title">
                <h2>Pets for Adoption</h2>
            </div>
            <div class="pet-cards">
                <div class="pet-card">
                    <div class="pet-image">
                        <i class="fas fa-dog"></i>
                    </div>
                    <div class="pet-info">
                        <h3>Max</h3>
                        <p>2 years old • Friendly • House-trained</p>
                        <p>Max is a playful Labrador mix looking for his forever home.</p>
                        <a href="#" class="btn" style="margin-top: 15px;">Adopt Me</a>
                    </div>
                </div>
                <div class="pet-card">
                    <div class="pet-image">
                        <i class="fas fa-cat"></i>
                    </div>
                    <div class="pet-info">
                        <h3>Luna</h3>
                        <p>1 year old • Calm • Loves attention</p>
                        <p>Luna is a beautiful tabby cat who gets along with other pets.</p>
                        <a href="#" class="btn" style="margin-top: 15px;">Adopt Me</a>
                    </div>
                </div>
                <div class="pet-card">
                    <div class="pet-image">
                        <i class="fas fa-dove"></i>
                    </div>
                    <div class="pet-info">
                        <h3>Kiwi</h3>
                        <p>6 months old • Colorful • Sociable</p>
                        <p>Kiwi is a friendly parrot looking for a loving aviary home.</p>
                        <a href="#" class="btn" style="margin-top: 15px;">Adopt Me</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Emergency Section -->
    <section id="emergency">
        <div class="container">
            <div class="emergency">
                <h2>Emergency Services Available 24/7</h2>
                <p>If your pet is experiencing a medical emergency, don't wait. Contact our emergency hotline immediately for assistance.</p>
                <a href="tel:+92123456789" class="btn emergency-btn"><i class="fas fa-phone"></i> Call Now: +92 123 456789</a>
            </div>
        </div>
    </section>

    <!-- Tips Section -->
    <section id="tips">
        <div class="container">
            <div class="section-title">
                <h2>Pet Care Tips</h2>
            </div>
            <div class="tips-grid">
                <div class="tip-card">
                    <h3>Regular Exercise</h3>
                    <p>Ensure your pet gets daily exercise appropriate for their breed and age. This helps maintain a healthy weight and prevents behavioral issues.</p>
                </div>
                <div class="tip-card">
                    <h3>Balanced Diet</h3>
                    <p>Feed your pet high-quality food that meets their nutritional needs. Avoid feeding them human food that might be harmful.</p>
                </div>
                <div class="tip-card">
                    <h3>Veterinary Visits</h3>
                    <p>Schedule regular check-ups with your veterinarian to monitor your pet's health and catch potential issues early.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer id="contact">
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Paws & Beaks</h3>
                    <p>Your trusted partner in pet care across Pakistan. We provide comprehensive veterinary services with compassion and expertise.</p>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="footer-column">
                    <h3>Contact Info</h3>
                    <p><i class="fas fa-map-marker-alt"></i> 123 Pet Street, Karachi, Pakistan</p>
                    <p><i class="fas fa-phone"></i> +92 123 456789</p>
                    <p><i class="fas fa-envelope"></i> info@pawsandbeaks.com</p>
                    <a href="https://wa.me/92123456789" class="whatsapp-btn"><i class="fab fa-whatsapp"></i> Book via WhatsApp</a>
                </div>
                <div class="footer-column">
                    <h3>Business Hours</h3>
                    <p>Monday - Friday: 9:00 AM - 6:00 PM</p>
                    <p>Saturday: 10:00 AM - 4:00 PM</p>
                    <p>Sunday: Emergency only</p>
                    <p>24/7 Emergency services available</p>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 Paws & Beaks Pet Clinic. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Simple animation for elements when they come into view
        document.addEventListener('DOMContentLoaded', function() {
            const animatedElements = document.querySelectorAll('.service-card, .pet-card, .tip-card');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = 1;
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, {
                threshold: 0.1
            });
            
            animatedElements.forEach(element => {
                element.style.opacity = 0;
                element.style.transform = 'translateY(20px)';
                element.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                observer.observe(element);
            });
        });
    </script>
