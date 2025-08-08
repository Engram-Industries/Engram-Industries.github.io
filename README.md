<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Engram Industries | Pioneering Memory Reconstruction Technology</title>
    <meta name="description" content="Engram Industries specializes in advanced memory reconstruction technology, mnemonic enhancement, and temporal cognition research.">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        :root {
            --primary-color: #0066CC;
            --text-dark: #333;
            --text-light: #666;
            --border-color: #e0e0e0;
            --bg-light: #f8f9fa;
            --warning-color: #ff6600;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Helvetica Neue', Arial, sans-serif;
            line-height: 1.6;
            color: var(--text-dark);
            background: white;
        }
        
        /* Header */
        header {
            background: white;
            border-bottom: 1px solid var(--border-color);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        nav {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 80px;
        }
        
        .logo {
            font-size: 24px;
            font-weight: 300;
            letter-spacing: 3px;
            color: var(--text-dark);
        }
        
        .logo-symbol {
            display: inline-block;
            width: 30px;
            height: 30px;
            margin-right: 15px;
            background: linear-gradient(135deg, #0066CC, #004499);
            border-radius: 50%;
            position: relative;
            vertical-align: middle;
        }
        
        .logo-symbol::after {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 15px;
            height: 15px;
            background: white;
            border-radius: 50%;
        }
        
        .nav-links {
            display: flex;
            gap: 40px;
            list-style: none;
        }
        
        .nav-links a {
            color: var(--text-light);
            text-decoration: none;
            font-size: 14px;
            letter-spacing: 0.5px;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--primary-color);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #f5f7fa 0%, #e9ecef 100%);
            padding: 120px 20px;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 48px;
            font-weight: 300;
            margin-bottom: 20px;
            letter-spacing: -1px;
        }
        
        .hero .subtitle {
            font-size: 20px;
            color: var(--text-light);
            margin-bottom: 40px;
        }
        
        .hero-stats {
            display: flex;
            justify-content: center;
            gap: 60px;
            margin-top: 60px;
        }
        
        .stat {
            text-align: center;
        }
        
        .stat-number {
            font-size: 36px;
            font-weight: 300;
            color: var(--primary-color);
        }
        
        .stat-label {
            font-size: 12px;
            text-transform: uppercase;
            letter-spacing: 1px;
            color: var(--text-light);
            margin-top: 5px;
        }
        
        /* Main Content */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 80px 20px;
        }
        
        section {
            margin-bottom: 100px;
        }
        
        h2 {
            font-size: 36px;
            font-weight: 300;
            margin-bottom: 20px;
            letter-spacing: -0.5px;
        }
        
        .section-subtitle {
            font-size: 18px;
            color: var(--text-light);
            margin-bottom: 40px;
        }
        
        /* Products Section */
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
            margin-top: 40px;
        }
        
        .product-card {
            background: var(--bg-light);
            padding: 40px;
            border-radius: 8px;
            transition: transform 0.3s;
        }
        
        .product-card:hover {
            transform: translateY(-5px);
        }
        
        .product-status {
            display: inline-block;
            padding: 4px 8px;
            background: var(--primary-color);
            color: white;
            font-size: 10px;
            text-transform: uppercase;
            letter-spacing: 1px;
            border-radius: 3px;
            margin-bottom: 15px;
        }
        
        .product-status.beta {
            background: var(--warning-color);
        }
        
        .product-card h3 {
            font-size: 24px;
            margin-bottom: 15px;
        }
        
        .product-card p {
            color: var(--text-light);
            margin-bottom: 20px;
            font-size: 14px;
            line-height: 1.8;
        }
        
        .product-link {
            color: var(--primary-color);
            text-decoration: none;
            font-size: 14px;
            font-weight: 500;
        }
        
        /* Research Section */
        .research-papers {
            display: grid;
            gap: 30px;
        }
        
        .paper {
            padding: 30px;
            border: 1px solid var(--border-color);
            border-radius: 8px;
            background: white;
        }
        
        .paper-title {
            font-size: 18px;
            font-weight: 500;
            margin-bottom: 10px;
            color: var(--text-dark);
        }
        
        .paper-authors {
            font-size: 14px;
            color: var(--text-light);
            margin-bottom: 15px;
        }
        
        .paper-abstract {
            font-size: 14px;
            color: var(--text-light);
            line-height: 1.8;
            margin-bottom: 15px;
        }
        
        .paper-status {
            display: inline-block;
            padding: 4px 8px;
            background: #28a745;
            color: white;
            font-size: 10px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            border-radius: 3px;
        }
        
        .paper-status.pending {
            background: #ffc107;
        }
        
        .paper-status.review {
            background: #6c757d;
        }
        
        /* Team Section */
        .team-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-top: 40px;
        }
        
        .team-member {
            text-align: center;
        }
        
        .member-photo {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            margin: 0 auto 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 48px;
            color: white;
            font-weight: 300;
        }
        
        .member-name {
            font-size: 18px;
            font-weight: 500;
            margin-bottom: 5px;
        }
        
        .member-title {
            font-size: 14px;
            color: var(--text-light);
            margin-bottom: 10px;
        }
        
        .member-credentials {
            font-size: 12px;
            color: #999;
        }
        
        /* Careers Section */
        .careers-list {
            display: grid;
            gap: 20px;
        }
        
        .job-posting {
            padding: 25px;
            border: 1px solid var(--border-color);
            border-radius: 8px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: border-color 0.3s;
        }
        
        .job-posting:hover {
            border-color: var(--primary-color);
        }
        
        .job-title {
            font-size: 16px;
            font-weight: 500;
            margin-bottom: 5px;
        }
        
        .job-department {
            font-size: 14px;
            color: var(--text-light);
        }
        
        .job-type {
            padding: 6px 12px;
            background: var(--bg-light);
            border-radius: 20px;
            font-size: 12px;
            color: var(--text-light);
        }
        
        /* Footer */
        footer {
            background: var(--bg-light);
            border-top: 1px solid var(--border-color);
            padding: 60px 20px 40px;
        }
        
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 2fr 1fr 1fr 1fr;
            gap: 60px;
        }
        
        .footer-section h4 {
            font-size: 14px;
            font-weight: 500;
            margin-bottom: 20px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        .footer-section p,
        .footer-section li {
            font-size: 14px;
            color: var(--text-light);
            line-height: 1.8;
        }
        
        .footer-section ul {
            list-style: none;
        }
        
        .footer-section li {
            margin-bottom: 10px;
        }
        
        .footer-section a {
            color: var(--text-light);
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-section a:hover {
            color: var(--primary-color);
        }
        
        .footer-bottom {
            max-width: 1200px;
            margin: 40px auto 0;
            padding-top: 40px;
            border-top: 1px solid var(--border-color);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .footer-bottom p {
            font-size: 12px;
            color: #999;
        }
        
        .disclaimer {
            background: #fff3cd;
            border: 1px solid #ffc107;
            border-radius: 8px;
            padding: 20px;
            margin-top: 40px;
            font-size: 12px;
            color: #856404;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .hero h1 {
                font-size: 32px;
            }
            
            .hero-stats {
                flex-direction: column;
                gap: 30px;
            }
            
            .footer-content {
                grid-template-columns: 1fr;
                gap: 40px;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">
                <span class="logo-symbol"></span>
                ENGRAM INDUSTRIES
            </div>
            <ul class="nav-links">
                <li><a href="#products">Products</a></li>
                <li><a href="#research">Research</a></li>
                <li><a href="#team">Team</a></li>
                <li><a href="#careers">Careers</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <h1>Pioneering Memory Reconstruction</h1>
        <p class="subtitle">Advanced mnemonic technologies for the preservation and enhancement of human memory</p>
        
        <div class="hero-stats">
            <div class="stat">
                <div class="stat-number">2.3M</div>
                <div class="stat-label">Memory Points Per Scan</div>
            </div>
            <div class="stat">
                <div class="stat-number">47s</div>
                <div class="stat-label">Average Processing Time</div>
            </div>
            <div class="stat">
                <div class="stat-number">87%</div>
                <div class="stat-label">Reconstruction Accuracy*</div>
            </div>
        </div>
    </section>

    <div class="container">
        <section id="about">
            <h2>About Engram Industries</h2>
            <p class="section-subtitle">
                Founded in 2024, Engram Industries emerged from stealth mode with breakthrough advances in memory reconstruction technology. 
                Our team of neuroscientists, engineers, and mnemonic specialists work at the intersection of consciousness and computation.
            </p>
            <p style="color: var(--text-light); line-height: 1.8;">
                Through our proprietary Hollowgram™ technology, we've achieved unprecedented fidelity in the extraction and reconstruction 
                of human memories from static visual inputs. Our research focuses on the preservation of temporal experiences, the enhancement 
                of recall accuracy, and the exploration of memory's malleable nature.
            </p>
        </section>

        <section id="products">
            <h2>Our Products</h2>
            <p class="section-subtitle">Cutting-edge applications of memory reconstruction technology</p>
            
            <div class="products-grid">
                <div class="product-card">
                    <span class="product-status">Available</span>
                    <h3>Relapsr™</h3>
                    <p>
                        Consumer-grade memory reconstruction platform enabling users to transform photographs into 
                        explorable three-dimensional memories. Features our patented Hollowgram™ rendering engine.
                    </p>
                    <a href="https://relapsr.com" class="product-link">Learn More →</a>
                </div>
                
                <div class="product-card">
                    <span class="product-status beta">Beta</span>
                    <h3>MnemonicOS™</h3>
                    <p>
                        Enterprise memory management system for organizations requiring long-term preservation of 
                        institutional knowledge. Currently in limited beta with select partners.
                    </p>
                    <a href="#" class="product-link">Request Access →</a>
                </div>
                
                <div class="product-card">
                    <span class="product-status beta">Research</span>
                    <h3>Temporal Anchor™</h3>
                    <p>
                        Experimental framework for maintaining cognitive stability during extended memory reconstruction 
                        sessions. In development at our San Francisco research facility.
                    </p>
                    <a href="#" class="product-link">View Research →</a>
                </div>
            </div>
        </section>

        <section id="research">
            <h2>Published Research</h2>
            <p class="section-subtitle">Peer-reviewed studies and ongoing investigations</p>
            
            <div class="research-papers">
                <div class="paper">
                    <h3 class="paper-title">Gaussian Distribution Patterns in Memory Point Cloud Reconstruction</h3>
                    <p class="paper-authors">Chen, S., Torres, M., Park, J. - Engram Industries Research Division</p>
                    <p class="paper-abstract">
                        We present a novel approach to memory reconstruction using 2.3 million Gaussian distributions to represent 
                        spatial-temporal memory data. Our method achieves 87% accuracy in blind studies, though subjects reported 
                        mild temporal displacement in 23% of cases...
                    </p>
                    <span class="paper-status">Published 2024</span>
                </div>
                
                <div class="paper">
                    <h3 class="paper-title">Hallucination Rate Optimization in Neural Memory Synthesis</h3>
                    <p class="paper-authors">Watson, E., Chen, S. - Engram Industries</p>
                    <p class="paper-abstract">
                        This study examines the relationship between reconstruction fidelity and hallucination rates in synthetic 
                        memory generation. We find that a 23-35% hallucination rate optimizes user engagement while maintaining 
                        cognitive coherence...
                    </p>
                    <span class="paper-status pending">Under Review</span>
                </div>
                
                <div class="paper">
                    <h3 class="paper-title">Long-term Effects of Repeated Exposure to Reconstructed Memories</h3>
                    <p class="paper-authors">Torres, M., et al. - Collaborative Study</p>
                    <p class="paper-abstract">
                        Longitudinal study tracking 500 subjects over 12 months of regular memory reconstruction sessions. 
                        Preliminary findings suggest altered recall patterns and enhanced vividness of reconstructed memories 
                        compared to organic memories. Full results pending...
                    </p>
                    <span class="paper-status review">In Progress</span>
                </div>
            </div>
        </section>

        <section id="team">
            <h2>Leadership Team</h2>
            <p class="section-subtitle">Pioneers in mnemonic science and reconstruction technology</p>
            
            <div class="team-grid">
                <div class="team-member">
                    <div class="member-photo">SC</div>
                    <h3 class="member-name">Dr. Sarah Chen</h3>
                    <p class="member-title">Chief Mnemonic Officer</p>
                    <p class="member-credentials">PhD Neuroscience, MIT</p>
                </div>
                
                <div class="team-member">
                    <div class="member-photo">MT</div>
                    <h3 class="member-name">Dr. Michael Torres</h3>
                    <p class="member-title">Head of Temporal Studies</p>
                    <p class="member-credentials">PhD Cognitive Science, Stanford</p>
                </div>
                
                <div class="team-member">
                    <div class="member-photo">EW</div>
                    <h3 class="member-name">Dr. Emily Watson</h3>
                    <p class="member-title">Director of Reconstruction</p>
                    <p class="member-credentials">PhD Computer Vision, CMU</p>
                </div>
                
                <div class="team-member">
                    <div class="member-photo">JP</div>
                    <h3 class="member-name">Dr. James Park</h3>
                    <p class="member-title">VP Hallucination Management</p>
                    <p class="member-credentials">MD/PhD, Johns Hopkins</p>
                </div>
            </div>
        </section>

        <section id="careers">
            <h2>Join Our Team</h2>
            <p class="section-subtitle">Help shape the future of human memory</p>
            
            <div class="careers-list">
                <div class="job-posting">
                    <div>
                        <h3 class="job-title">Senior Mnemonic Engineer</h3>
                        <p class="job-department">Research & Development</p>
                    </div>
                    <span class="job-type">Full-time</span>
                </div>
                
                <div class="job-posting">
                    <div>
                        <h3 class="job-title">Temporal Displacement Specialist</h3>
                        <p class="job-department">Safety & Compliance</p>
                    </div>
                    <span class="job-type">Full-time</span>
                </div>
                
                <div class="job-posting">
                    <div>
                        <h3 class="job-title">Memory Reconstruction Technician</h3>
                        <p class="job-department">Operations</p>
                    </div>
                    <span class="job-type">Contract</span>
                </div>
                
                <div class="job-posting">
                    <div>
                        <h3 class="job-title">Hallucination Rate Analyst</h3>
                        <p class="job-department">Quality Assurance</p>
                    </div>
                    <span class="job-type">Full-time</span>
                </div>
            </div>
        </section>

        <div class="disclaimer">
            <strong>Important Notice:</strong> Engram Industries' memory reconstruction technology is pending FDA approval for therapeutic use. 
            Current applications are limited to entertainment and research purposes. Side effects may include temporal displacement, 
            enhanced nostalgia, difficulty distinguishing reconstructed from organic memories, and mild dissociation. Users experiencing 
            memory loops lasting more than 4 hours should discontinue use and consult a mnemonic specialist.
        </div>
    </div>

    <footer>
        <div class="footer-content">
            <div class="footer-section">
                <h4>Engram Industries</h4>
                <p>
                    Pioneering the future of human memory through advanced reconstruction technology. 
                    Our mission is to preserve, enhance, and make accessible the full spectrum of human experience.
                </p>
                <p style="margin-top: 20px;">
                    <strong>Headquarters:</strong><br>
                    580 California Street<br>
                    San Francisco, CA 94104
                </p>
            </div>
            
            <div class="footer-section">
                <h4>Products</h4>
                <ul>
                    <li><a href="https://relapsr.com">Relapsr™</a></li>
                    <li><a href="#">MnemonicOS™</a></li>
                    <li><a href="#">Temporal Anchor™</a></li>
                    <li><a href="#">Hollowgram™ SDK</a></li>
                </ul>
            </div>
            
            <div class="footer-section">
                <h4>Company</h4>
                <ul>
                    <li><a href="#about">About</a></li>
                    <li><a href="#research">Research</a></li>
                    <li><a href="#careers">Careers</a></li>
                    <li><a href="#press">Press</a></li>
                    <li><a href="#investors">Investors</a></li>
                </ul>
            </div>
            
            <div class="footer-section">
                <h4>Legal</h4>
                <ul>
                    <li><a href="#privacy">Privacy Policy</a></li>
                    <li><a href="#terms">Terms of Service</a></li>
                    <li><a href="#compliance">Compliance</a></li>
                    <li><a href="#patents">Patents</a></li>
                    <li><a href="#warnings">Health Warnings</a></li>
                </ul>
            </div>
        </div>
        
        <div class="footer-bottom">
            <p>© 2024 Engram Industries. All rights reserved. Memory accuracy not guaranteed.</p>
            <p>Hollowgram™, Relapsr™, and Temporal Anchor™ are registered trademarks of Engram Industries.</p>
        </div>
    </footer>
</body>
</html>
