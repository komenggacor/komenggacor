<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Premium - komenggacor</title>
    <style>
        /* Reset dan Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #0d1117;
            color: #c9d1d9;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        header {
            background: linear-gradient(135deg, #161b22 0%, #0d1117 100%);
            padding: 60px 0;
            border-bottom: 1px solid #21262d;
            position: relative;
            overflow: hidden;
        }

        header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(56,139,253,0.1) 0%, rgba(0,0,0,0) 70%);
            z-index: 0;
        }

        .header-content {
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            z-index: 1;
        }

        .profile {
            display: flex;
            align-items: center;
        }

        .avatar {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 4px solid #388bfd;
            margin-right: 30px;
            box-shadow: 0 0 20px rgba(56, 139, 253, 0.3);
        }

        .profile-info h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: #f0f6fc;
        }

        .profile-info p {
            font-size: 1.2rem;
            color: #8b949e;
            margin-bottom: 15px;
        }

        .tagline {
            font-size: 1.5rem;
            color: #388bfd;
            font-weight: 600;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-link {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: #21262d;
            color: #c9d1d9;
            text-decoration: none;
            transition: all 0.3s ease;
        }

        .social-link:hover {
            background-color: #388bfd;
            transform: translateY(-3px);
        }

        /* Section Styles */
        section {
            padding: 80px 0;
        }

        .section-title {
            font-size: 2rem;
            margin-bottom: 40px;
            color: #f0f6fc;
            position: relative;
            display: inline-block;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 60px;
            height: 3px;
            background-color: #388bfd;
        }

        /* About Section */
        .about-content {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .about-text p {
            margin-bottom: 20px;
            font-size: 1.1rem;
        }

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 20px;
        }

        .skill-tag {
            background-color: #21262d;
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            border: 1px solid #30363d;
        }

        .highlight {
            color: #388bfd;
        }

        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 30px;
        }

        .project-card {
            background-color: #161b22;
            border-radius: 10px;
            overflow: hidden;
            border: 1px solid #21262d;
            transition: all 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
            border-color: #388bfd;
        }

        .project-image {
            height: 200px;
            background-color: #0d1117;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #8b949e;
            font-size: 1.2rem;
        }

        .project-content {
            padding: 20px;
        }

        .project-title {
            font-size: 1.3rem;
            margin-bottom: 10px;
            color: #f0f6fc;
        }

        .project-description {
            color: #8b949e;
            margin-bottom: 15px;
        }

        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 15px;
        }

        .tech-tag {
            background-color: #13233a;
            color: #58a6ff;
            padding: 4px 10px;
            border-radius: 15px;
            font-size: 0.8rem;
        }

        .project-links {
            display: flex;
            gap: 15px;
        }

        .project-link {
            display: inline-flex;
            align-items: center;
            gap: 5px;
            color: #388bfd;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.2s ease;
        }

        .project-link:hover {
            color: #58a6ff;
        }

        /* Experience Section */
        .timeline {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }

        .timeline::before {
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            left: 30px;
            width: 2px;
            background-color: #21262d;
        }

        .timeline-item {
            position: relative;
            margin-bottom: 40px;
            padding-left: 80px;
        }

        .timeline-date {
            position: absolute;
            left: 0;
            top: 0;
            width: 60px;
            padding: 5px 10px;
            background-color: #388bfd;
            color: white;
            border-radius: 4px;
            font-size: 0.8rem;
            text-align: center;
        }

        .timeline-content {
            background-color: #161b22;
            padding: 20px;
            border-radius: 8px;
            border: 1px solid #21262d;
        }

        .timeline-title {
            font-size: 1.2rem;
            margin-bottom: 5px;
            color: #f0f6fc;
        }

        .timeline-subtitle {
            color: #8b949e;
            margin-bottom: 10px;
            font-size: 0.9rem;
        }

        /* Contact Section */
        .contact-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
        }

        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .contact-icon {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: #21262d;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #388bfd;
        }

        .contact-form {
            background-color: #161b22;
            padding: 30px;
            border-radius: 10px;
            border: 1px solid #21262d;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-label {
            display: block;
            margin-bottom: 8px;
            color: #f0f6fc;
        }

        .form-input, .form-textarea {
            width: 100%;
            padding: 12px 15px;
            background-color: #0d1117;
            border: 1px solid #30363d;
            border-radius: 6px;
            color: #c9d1d9;
            font-size: 1rem;
        }

        .form-input:focus, .form-textarea:focus {
            outline: none;
            border-color: #388bfd;
        }

        .form-textarea {
            min-height: 120px;
            resize: vertical;
        }

        .btn {
            display: inline-block;
            padding: 12px 25px;
            background-color: #388bfd;
            color: white;
            border: none;
            border-radius: 6px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .btn:hover {
            background-color: #58a6ff;
            transform: translateY(-2px);
        }

        /* Footer */
        footer {
            background-color: #161b22;
            padding: 40px 0;
            text-align: center;
            border-top: 1px solid #21262d;
        }

        .footer-text {
            color: #8b949e;
            margin-bottom: 20px;
        }

        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .fade-in {
            animation: fadeIn 0.8s ease forwards;
        }

        /* Responsive Design */
        @media (max-width: 992px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            .profile {
                flex-direction: column;
                margin-bottom: 30px;
            }
            
            .avatar {
                margin-right: 0;
                margin-bottom: 20px;
            }
            
            .about-content {
                grid-template-columns: 1fr;
            }
            
            .contact-content {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 768px) {
            .projects-grid {
                grid-template-columns: 1fr;
            }
            
            section {
                padding: 60px 0;
            }
        }
    </style>
</head>
<body>
    <!-- Header Section -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="profile">
                    <img src="https://avatars.githubusercontent.com/u/YOUR_USER_ID" alt="Profile Picture" class="avatar">
                    <div class="profile-info">
                        <h1>komenggacor</h1>
                        <p class="tagline">Full Stack Developer & Problem Solver</p>
                        <p>Membangun solusi digital yang inovatif dan efisien</p>
                        <div class="social-links">
                            <a href="https://github.com/komenggacor" class="social-link">G</a>
                            <a href="https://linkedin.com/in/komenggacor" class="social-link">L</a>
                            <a href="https://twitter.com/komenggacor" class="social-link">T</a>
                            <a href="mailto:komenggacor@example.com" class="social-link">M</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <!-- About Section -->
    <section id="about">
        <div class="container">
            <h2 class="section-title fade-in">Tentang Saya</h2>
            <div class="about-content fade-in">
                <div class="about-text">
                    <p>Halo! Saya seorang <span class="highlight">Full Stack Developer</span> dengan passion dalam menciptakan solusi teknologi yang efisien dan user-friendly. Dengan pengalaman lebih dari 3 tahun di industri, saya telah mengembangkan berbagai aplikasi web dan mobile untuk klien dari berbagai sektor.</p>
                    <p>Saya percaya bahwa kode yang baik tidak hanya berfungsi dengan benar, tetapi juga mudah dipahami, dikelola, dan dikembangkan. Saya selalu berusaha untuk menerapkan best practices dalam setiap proyek yang saya kerjakan.</p>
                    <div class="skills">
                        <span class="skill-tag">JavaScript</span>
                        <span class="skill-tag">TypeScript</span>
                        <span class="skill-tag">React</span>
                        <span class="skill-tag">Node.js</span>
                        <span class="skill-tag">Python</span>
                        <span class="skill-tag">PostgreSQL</span>
                        <span class="skill-tag">Docker</span>
                        <span class="skill-tag">AWS</span>
                    </div>
                </div>
                <div class="about-stats">
                    <h3>Statistik GitHub</h3>
                    <p>Berikut adalah beberapa statistik dari aktivitas GitHub saya:</p>
                    <!-- GitHub stats akan ditampilkan di sini -->
                    <div style="margin-top: 20px; text-align: center;">
                        <img src="https://github-readme-stats.vercel.app/api?username=komenggacor&show_icons=true&theme=radical" alt="GitHub Stats" style="max-width: 100%;">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <div class="container">
            <h2 class="section-title fade-in">Proyek Unggulan</h2>
            <div class="projects-grid">
                <div class="project-card fade-in">
                    <div class="project-image">
                        [Gambar Proyek 1]
                    </div>
                    <div class="project-content">
                        <h3 class="project-title">Sistem Manajemen E-Commerce</h3>
                        <p class="project-description">Platform e-commerce lengkap dengan dashboard admin, sistem pembayaran, dan manajemen inventaris.</p>
                        <div class="project-tech">
                            <span class="tech-tag">React</span>
                            <span class="tech-tag">Node.js</span>
                            <span class="tech-tag">MongoDB</span>
                            <span class="tech-tag">Stripe API</span>
                        </div>
                        <div class="project-links">
                            <a href="#" class="project-link">Lihat Demo</a>
                            <a href="#" class="project-link">Kode Sumber</a>
                        </div>
                    </div>
                </div>
                
                <div class="project-card fade-in">
                    <div class="project-image">
                        [Gambar Proyek 2]
                    </div>
                    <div class="project-content">
                        <h3 class="project-title">Aplikasi Mobile Task Management</h3>
                        <p class="project-description">Aplikasi produktivitas untuk mengelola tugas dengan fitur kolaborasi tim dan notifikasi real-time.</p>
                        <div class="project-tech">
                            <span class="tech-tag">React Native</span>
                            <span class="tech-tag">Firebase</span>
                            <span class="tech-tag">Redux</span>
                        </div>
                        <div class="project-links">
                            <a href="#" class="project-link">Lihat Demo</a>
                            <a href="#" class="project-link">Kode Sumber</a>
                        </div>
                    </div>
                </div>
                
                <div class="project-card fade-in">
                    <div class="project-image">
                        [Gambar Proyek 3]
                    </div>
                    <div class="project-content">
                        <h3 class="project-title">Platform Analisis Data</h3>
                        <p class="project-description">Tool visualisasi data dengan dashboard interaktif untuk analisis bisnis dan pelaporan.</p>
                        <div class="project-tech">
                            <span class="tech-tag">Python</span>
                            <span class="tech-tag">Django</span>
                            <span class="tech-tag">D3.js</span>
                            <span class="tech-tag">PostgreSQL</span>
                        </div>
                        <div class="project-links">
                            <a href="#" class="project-link">Lihat Demo</a>
                            <a href="#" class="project-link">Kode Sumber</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience">
        <div class="container">
            <h2 class="section-title fade-in">Pengalaman Kerja</h2>
            <div class="timeline">
                <div class="timeline-item fade-in">
                    <div class="timeline-date">2022 - Sekarang</div>
                    <div class="timeline-content">
                        <h3 class="timeline-title">Senior Full Stack Developer</h3>
                        <p class="timeline-subtitle">Tech Solutions Inc.</p>
                        <p>Memimpin pengembangan aplikasi web dan mobile untuk klien perusahaan. Bertanggung jawab atas arsitektur sistem, code review, dan mentoring developer junior.</p>
                    </div>
                </div>
                
                <div class="timeline-item fade-in">
                    <div class="timeline-date">2020 - 2022</div>
                    <div class="timeline-content">
                        <h3 class="timeline-title">Full Stack Developer</h3>
                        <p class="timeline-subtitle">Digital Creative Agency</p>
                        <p>Mengembangkan berbagai aplikasi web untuk klien dari berbagai industri. Berkolaborasi dengan tim desain untuk menciptakan pengalaman pengguna yang optimal.</p>
                    </div>
                </div>
                
                <div class="timeline-item fade-in">
                    <div class="timeline-date">2019 - 2020</div>
                    <div class="timeline-content">
                        <h3 class="timeline-title">Frontend Developer</h3>
                        <p class="timeline-subtitle">Startup XYZ</p>
                        <p>Mengembangkan antarmuka pengguna untuk aplikasi SaaS menggunakan React.js. Menerapkan responsive design dan optimasi performa.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <div class="container">
            <h2 class="section-title fade-in">Hubungi Saya</h2>
            <div class="contact-content">
                <div class="contact-info fade-in">
                    <div class="contact-item">
                        <div class="contact-icon">@</div>
                        <div>
                            <h3>Email</h3>
                            <p>komenggacor@example.com</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">L</div>
                        <div>
                            <h3>LinkedIn</h3>
                            <p>linkedin.com/in/komenggacor</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">G</div>
                        <div>
                            <h3>GitHub</h3>
                            <p>github.com/komenggacor</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">T</div>
                        <div>
                            <h3>Twitter</h3>
                            <p>twitter.com/komenggacor</p>
                        </div>
                    </div>
                </div>
                
                <div class="contact-form fade-in">
                    <form id="contactForm">
                        <div class="form-group">
                            <label for="name" class="form-label">Nama</label>
                            <input type="text" id="name" class="form-input" required>
                        </div>
                        
                        <div class="form-group">
                            <label for="email" class="form-label">Email</label>
                            <input type="email" id="email" class="form-input" required>
                        </div>
                        
                        <div class="form-group">
                            <label for="subject" class="form-label">Subjek</label>
                            <input type="text" id="subject" class="form-input" required>
                        </div>
                        
                        <div class="form-group">
                            <label for="message" class="form-label">Pesan</label>
                            <textarea id="message" class="form-textarea" required></textarea>
                        </div>
                        
                        <button type="submit" class="btn">Kirim Pesan</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p class="footer-text">&copy; 2023 komenggacor. All rights reserved.</p>
            <p class="footer-text">Dibuat dengan ❤️ dan banyak ☕</p>
        </div>
    </footer>

    <script>
        // Animasi scroll
        document.addEventListener('DOMContentLoaded', function() {
            const fadeElements = document.querySelectorAll('.fade-in');
            
            const fadeInOnScroll = function() {
                fadeElements.forEach(element => {
                    const elementTop = element.getBoundingClientRect().top;
                    const elementVisible = 150;
                    
                    if (elementTop < window.innerHeight - elementVisible) {
                        element.style.opacity = 1;
                        element.style.transform = 'translateY(0)';
                    }
                });
            };
            
            // Set initial state
            fadeElements.forEach(element => {
                element.style.opacity = 0;
                element.style.transform = 'translateY(20px)';
                element.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
            });
            
            window.addEventListener('scroll', fadeInOnScroll);
            fadeInOnScroll(); // Check on load
            
            // Form submission
            document.getElementById('contactForm').addEventListener('submit', function(e) {
                e.preventDefault();
                alert('Terima kasih! Pesan Anda telah dikirim. Saya akan membalasnya segera.');
                this.reset();
            });
        });
    </script>
</body>
</html>
