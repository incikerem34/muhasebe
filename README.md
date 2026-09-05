<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hamza Öztayoğlu | Mali Müşavir & Finansal Danışman</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --primary-color: #0f2a4a;
            --secondary-color: #1d4ed8;
            --accent-color: #f59e0b;
            --bg-light: #f8fafc;
            --text-dark: #1e293b;
            --text-muted: #64748b;
            --white: #ffffff;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.6;
        }

        /* Header & Nav */
        header {
            background: var(--primary-color);
            color: var(--white);
            padding: 1rem 5%;
            position: sticky;
            top: 0;
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--white);
            text-decoration: none;
        }

        .logo span { color: var(--accent-color); }

        nav a {
            color: var(--white);
            text-decoration: none;
            margin-left: 20px;
            font-size: 0.95rem;
            transition: color 0.3s;
        }

        nav a:hover { color: var(--accent-color); }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--primary-color), #1e3a8a);
            color: var(--white);
            padding: 80px 5%;
            text-align: center;
        }

        .hero h1 { font-size: 2.8rem; margin-bottom: 10px; }
        .hero p { font-size: 1.2rem; color: #93c5fd; max-width: 600px; margin: 0 auto 30px; }

        .btn {
            background-color: var(--accent-color);
            color: var(--primary-color);
            padding: 12px 28px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
            transition: transform 0.2s, background 0.3s;
        }

        .btn:hover {
            transform: translateY(-2px);
            background-color: #d97706;
        }

        /* Containers & Titles */
        .container { padding: 60px 5%; max-width: 1200px; margin: 0 auto; }
        
        .section-title {
            text-align: center;
            font-size: 2rem;
            color: var(--primary-color);
            margin-bottom: 40px;
            position: relative;
        }

        .section-title::after {
            content: '';
            width: 50px;
            height: 3px;
            background: var(--accent-color);
            display: block;
            margin: 10px auto 0;
        }

        /* Cards Grid */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .card {
            background: var(--white);
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            border: 1px solid #e2e8f0;
            transition: transform 0.3s;
        }

        .card:hover { transform: translateY(-5px); }
        .card i { font-size: 2.5rem; color: var(--secondary-color); margin-bottom: 15px; }
        .card h3 { margin-bottom: 10px; color: var(--primary-color); }

        /* Skills Tags */
        .skills-container { display: flex; flex-wrap: wrap; gap: 10px; justify-content: center; }
        .skill-tag {
            background: #e0e7ff;
            color: var(--secondary-color);
            padding: 8px 16px;
            border-radius: 20px;
            font-weight: 600;
            font-size: 0.9rem;
        }

        /* Contact & Footer */
        .contact-info { text-align: center; font-size: 1.1rem; }
        .contact-info p { margin: 15px 0; }
        .contact-info i { color: var(--secondary-color); margin-right: 10px; }

        footer {
            background: var(--primary-color);
            color: var(--white);
            text-align: center;
            padding: 20px;
            margin-top: 40px;
            font-size: 0.9rem;
        }

        @media (max-width: 768px) {
            header { flex-direction: column; text-align: center; }
            nav { margin-top: 15px; }
            nav a { margin: 0 8px; }
            .hero h1 { font-size: 2rem; }
        }
    </style>
</head>
<body>

    <header>
        <a href="#" class="logo">DİA&Akınsoft <span>| SMMM</span></a>
        <nav>
            <a href="#hizmetler">Hizmetler</a>
            <a href="#yazilimlar">Sistemler</a>
            <a href="#hakkimda">Hakkımda</a>
            <a href="#iletisim">İletişim</a>
        </nav>
    </header>

    <section class="hero">
        <h1>Mali Müşavirlik & Finansal Danışmanlık</h1>
        <p>Şirketiniz için vergi yönetimi, e-Dönüşüm süreçleri ve güvenilir finansal raporlama çözümleri.</p>
        <a href="#iletisim" class="btn">İletişime Geçin</a>
    </section>

    <section id="hizmetler" class="container">
        <h2 class="section-title">Uzmanlık Alanları</h2>
        <div class="grid">
            <div class="card">
                <i class="fa-solid fa-calculator"></i>
                <h3>Genel Muhasebe & Vergi</h3>
                <p>Beyanname süreçlerinin takibi, vergi planlaması ve mevzuata tam uyumluluk danışmanlığı.</p>
            </div>
            <div class="card">
                <i class="fa-solid fa-file-invoice-dollar"></i>
                <h3>e-Dönüşüm Danışmanlığı</h3>
                <p>e-Fatura, e-Arşiv ve e-Defter geçiş süreçlerinin sorunsuz kurulumu ve yönetimi.</p>
            </div>
            <div class="card">
                <i class="fa-solid fa-chart-line"></i>
                <h3>Finansal Raporlama</h3>
                <p>Nakit akış analizleri, bütçe planlama ve yönetim içi kararlar için finansal tablolar.</p>
            </div>
        </div>
    </section>

    <section id="yazilimlar" class="container" style="background: #eff6ff; border-radius: 10px;">
        <h2 class="section-title">Kullandığım Yazılımlar & Sistemler</h2>
        <div class="skills-container">
            
            <span class="skill-tag">Akınsoft Wolvox</span>
            <span class="skill-tag">GİB e-Portallar</span>
            <span class="skill-tag">DİA</span>
            <span class="skill-tag">İleri Düzey Excel</span>
        </div>
    </section>

    <section id="iletisim" class="container">
        <h2 class="section-title">İletişim</h2>
        <div class="contact-info">
            <p><i class="fa-solid fa-envelope"></i> hamza.öztayoğlu@muhasebe.com</p>
            <p><i class="fa-solid fa-phone"></i> +90 (542) 660 69 16</p>
            <p><i class="fa-solid fa-location-dot"></i> Sultanbeyli
 / İstanbul</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 Hamza öztayoğlu - Tüm Hakları Saklıdır.</p>
    </footer>

</body>
</html>
