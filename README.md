<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Balai Desa Pondokjoyo | Profil Desa</title>

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link
        href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Poppins:wght@500;600;700;800&display=swap"
        rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">

    <style>
        :root {
            --green: #176b45;
            --green-dark: #0b422b;
            --green-light: #eaf7f0;
            --gold: #d7a62a;
            --dark: #10251b;
            --muted: #66756e;
            --white: #fff;
        }

        * {
            box-sizing: border-box;
            scroll-behavior: smooth
        }

        body {
            margin: 0;
            font-family: Inter, sans-serif;
            color: var(--dark);
            background: #fff;
        }

        h1,
        h2,
        h3,
        h4,
        .navbar-brand {
            font-family: Poppins, sans-serif
        }

        section {
            padding: 95px 0
        }

        .navbar {
            padding: 14px 0;
            background: rgba(255, 255, 255, .94) !important;
            backdrop-filter: blur(12px);
            box-shadow: 0 4px 25px rgba(0, 0, 0, .06);
        }

        .navbar-brand {
            font-weight: 800;
            color: var(--dark) !important
        }

        .brand-logo {
            width: 45px;
            height: 45px;
            object-fit: contain;
            border-radius: 12px;
            background: #fff;
        }

        .nav-link {
            font-weight: 600;
            color: #43534b !important;
            margin: 0 5px
        }

        .nav-link:hover,
        .nav-link.active {
            color: var(--green) !important
        }

        .btn-green {
            background: var(--green);
            color: #fff;
            border: 0;
            padding: 12px 22px;
            border-radius: 12px;
            font-weight: 700;
        }

        .btn-green:hover {
            background: var(--green-dark);
            color: #fff;
            transform: translateY(-2px)
        }

        .hero {
            min-height: 92vh;
            position: relative;
            display: flex;
            align-items: center;
            overflow: hidden;
            color: #fff;
            background:
                linear-gradient(90deg, rgba(5, 34, 21, .92) 0%, rgba(10, 61, 39, .78) 48%, rgba(8, 35, 24, .40) 100%),
                url("assets/foto-balai-desa.jpg") center/cover no-repeat;
        }

        .hero::after {
            content: "";
            position: absolute;
            inset: auto 0 0;
            height: 130px;
            background: linear-gradient(transparent, #fff);
        }

        .hero-content {
            position: relative;
            z-index: 2
        }

        .hero-logo {
            width: 92px;
            height: 92px;
            object-fit: contain;
            background: #fff;
            border-radius: 24px;
            padding: 10px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, .2);
            margin-bottom: 22px;
        }

        .badge-custom {
            display: inline-block;
            padding: 9px 14px;
            border-radius: 30px;
            background: rgba(255, 255, 255, .13);
            border: 1px solid rgba(255, 255, 255, .25);
            font-size: .78rem;
            font-weight: 800;
            letter-spacing: 1px;
        }

        .hero h1 {
            font-size: clamp(2.4rem, 5vw, 4.6rem);
            font-weight: 800;
            line-height: 1.08;
            margin: 18px 0
        }

        .hero p {
            max-width: 650px;
            font-size: 1.05rem;
            line-height: 1.8;
            color: #e9f5ef
        }

        .hero-buttons {
            display: flex;
            gap: 12px;
            flex-wrap: wrap
        }

        .btn-white {
            background: #fff;
            color: var(--green);
            padding: 13px 22px;
            border-radius: 12px;
            font-weight: 700;
            border: 0;
        }

        .btn-outline-white {
            color: #fff;
            border: 1px solid rgba(255, 255, 255, .6);
            padding: 13px 22px;
            border-radius: 12px;
            font-weight: 700;
        }

        .section-label {
            color: var(--green);
            font-size: .78rem;
            font-weight: 800;
            letter-spacing: 2px;
            text-transform: uppercase;
            margin-bottom: 10px;
        }

        .section-title {
            font-weight: 800;
            font-size: 2.25rem
        }

        .section-subtitle {
            color: var(--muted);
            line-height: 1.8;
            max-width: 700px
        }

        .info-card {
            border: 0;
            border-radius: 22px;
            padding: 30px;
            background: #fff;
            box-shadow: 0 12px 40px rgba(16, 37, 27, .08);
            height: 100%;
            transition: .3s;
        }

        .info-card:hover {
            transform: translateY(-7px);
            box-shadow: 0 18px 45px rgba(16, 37, 27, .13)
        }

        .icon-box {
            width: 58px;
            height: 58px;
            border-radius: 16px;
            background: var(--green-light);
            color: var(--green);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 25px;
            margin-bottom: 20px;
        }

        .about-image {
            width: 100%;
            height: 430px;
            object-fit: cover;
            border-radius: 28px;
            box-shadow: 0 20px 45px rgba(0, 0, 0, .12);
        }

        .feature-list {
            list-style: none;
            padding: 0;
            margin: 25px 0 0
        }

        .feature-list li {
            margin: 15px 0;
            color: #52635b
        }

        .feature-list i {
            color: var(--green);
            margin-right: 10px
        }

        .vision-box {
            background: linear-gradient(135deg, var(--green-dark), var(--green));
            color: #fff;
            border-radius: 28px;
            padding: 42px;
            height: 100%;
            position: relative;
            overflow: hidden;
        }

        .vision-box::before {
            content: "";
            width: 210px;
            height: 210px;
            border: 30px solid rgba(255, 255, 255, .06);
            border-radius: 50%;
            position: absolute;
            right: -60px;
            top: -70px;
        }

        .vision-box p {
            color: #e4f2eb;
            line-height: 1.8
        }

        .service-section {
            background: #f6faf8
        }

        .service-card {
            background: #fff;
            border: 1px solid #e4eee8;
            border-radius: 22px;
            padding: 32px;
            height: 100%;
            transition: .3s;
        }

        .service-card:hover {
            border-color: #a9d2bd;
            transform: translateY(-6px)
        }

        .number {
            font-size: .8rem;
            font-weight: 800;
            color: var(--gold)
        }

        .activity {
            border-radius: 22px;
            overflow: hidden;
            background: #fff;
            box-shadow: 0 10px 35px rgba(0, 0, 0, .07);
            height: 100%;
        }

        .activity img {
            width: 100%;
            height: 220px;
            object-fit: cover
        }

        .activity-body {
            padding: 24px
        }

        .contact-section {
            background: var(--dark);
            color: #fff
        }

        .contact-card {
            background: #163a2a;
            border: 1px solid rgba(255, 255, 255, .08);
            border-radius: 24px;
            padding: 32px;
            height: 100%;
        }

        .contact-item {
            display: flex;
            gap: 15px;
            margin: 22px 0
        }

        .contact-item i {
            font-size: 22px;
            color: #a9dfbf
        }

        .contact-item small {
            display: block;
            color: #9eb4a8;
            margin-bottom: 4px
        }

        .map {
            width: 100%;
            height: 100%;
            min-height: 410px;
            border: 0;
            border-radius: 24px;
        }

        footer {
            background: #08150f;
            color: #a9b9b0;
            padding: 28px 0
        }

        footer strong {
            color: #fff
        }

        .top {
            position: fixed;
            right: 22px;
            bottom: 22px;
            width: 46px;
            height: 46px;
            border: 0;
            border-radius: 50%;
            background: var(--green);
            color: #fff;
            box-shadow: 0 10px 25px rgba(0, 0, 0, .2);
            z-index: 99;
        }

        @media(max-width:768px) {
            section {
                padding: 70px 0
            }

            .hero {
                min-height: 88vh;
                background-position: center
            }

            .hero h1 {
                font-size: 2.55rem
            }

            .hero-logo {
                width: 75px;
                height: 75px
            }

            .about-image {
                height: 300px
            }

            .hero-buttons {
                justify-content: center
            }

            .hero-content {
                text-align: center
            }

            .hero p {
                margin-left: auto;
                margin-right: auto
            }
        }
    </style>
</head>

<body>

    <nav class="navbar navbar-expand-lg sticky-top">
        <div class="container">
            <a class="navbar-brand d-flex align-items-center gap-2" href="#home">
                <img src="assets/logo-desa.png" class="brand-logo" alt="Logo Desa Pondokjoyo">
                <span>Balai Desa Pondokjoyo</span>
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#nav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="nav">
                <ul class="navbar-nav ms-auto align-items-lg-center">
                    <li class="nav-item"><a class="nav-link active" href="#home">Beranda</a></li>
                    <li class="nav-item"><a class="nav-link" href="#about">Profil</a></li>
                    <li class="nav-item"><a class="nav-link" href="#services">Layanan</a></li>
                    <li class="nav-item"><a class="nav-link" href="#activities">Kegiatan</a></li>
                    <li class="nav-item"><a class="nav-link" href="#contact">Kontak</a></li>
                </ul>
                <a href="#contact" class="btn btn-green ms-lg-3 mt-3 mt-lg-0">Hubungi Kami</a>
            </div>
        </div>
    </nav>

    <section class="hero" id="home">
        <div class="container hero-content">
            <div class="row">
                <div class="col-lg-8">
                    <img src="assets/logo-desa.png" class="hero-logo" alt="Logo Desa Pondokjoyo">
                    <div><span class="badge-custom">PROFIL INSTANSI PKL • RPL</span></div>
                    <h1>Selamat Datang di<br>Balai Desa Pondokjoyo</h1>
                    <p>
                        Pusat pemerintahan dan pelayanan masyarakat Desa Pondokjoyo.
                        Website ini dibuat sebagai media informasi profil, layanan, kegiatan,
                        serta lokasi Balai Desa Pondokjoyo.
                    </p>
                    <div class="hero-buttons mt-4">
                        <a href="#about" class="btn btn-white">Kenali Desa <i class="bi bi-arrow-down ms-2"></i></a>
                        <a href="#contact" class="btn btn-outline-white">Lihat Lokasi</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="about">
        <div class="container">
            <div class="row align-items-center g-5">
                <div class="col-lg-6">
                    <img src="assets/foto-balai-desa.jpg" class="about-image" alt="Balai Desa Pondokjoyo">
                </div>
                <div class="col-lg-6">
                    <div class="section-label">Tentang Kami</div>
                    <h2 class="section-title mb-3">Mengenal Balai Desa Pondokjoyo</h2>
                    <p class="section-subtitle">
                        Balai Desa Pondokjoyo merupakan pusat pemerintahan desa yang berperan
                        dalam memberikan pelayanan kepada masyarakat serta mendukung pelaksanaan
                        program dan pembangunan desa.
                    </p>
                    <ul class="feature-list">
                        <li><i class="bi bi-check-circle-fill"></i>Pelayanan administrasi masyarakat</li>
                        <li><i class="bi bi-check-circle-fill"></i>Penyampaian informasi dan program desa</li>
                        <li><i class="bi bi-check-circle-fill"></i>Pendukung pembangunan dan pemberdayaan masyarakat
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <section class="service-section">
        <div class="container">
            <div class="text-center mb-5">
                <div class="section-label">Informasi Utama</div>
                <h2 class="section-title">Pelayanan untuk Masyarakat</h2>
                <p class="section-subtitle mx-auto">Beberapa fungsi utama Balai Desa Pondokjoyo dalam mendukung
                    kebutuhan masyarakat.</p>
            </div>
            <div class="row g-4">
                <div class="col-md-4">
                    <div class="info-card">
                        <div class="icon-box"><i class="bi bi-file-earmark-text"></i></div>
                        <h4>Administrasi Desa</h4>
                        <p class="text-secondary lh-lg">Mendukung kebutuhan administrasi dan surat-menyurat masyarakat
                            sesuai ketentuan yang berlaku.</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="info-card">
                        <div class="icon-box"><i class="bi bi-megaphone"></i></div>
                        <h4>Informasi Desa</h4>
                        <p class="text-secondary lh-lg">Menyediakan informasi mengenai kegiatan, program, dan pelayanan
                            yang berkaitan dengan masyarakat desa.</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="info-card">
                        <div class="icon-box"><i class="bi bi-people"></i></div>
                        <h4>Pemberdayaan Masyarakat</h4>
                        <p class="text-secondary lh-lg">Mendukung kegiatan kemasyarakatan, pembangunan, dan pemberdayaan
                            warga Desa Pondokjoyo.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section>
        <div class="container">
            <div class="row g-4">
                <div class="col-lg-6">
                    <div class="info-card">
                        <div class="section-label">Profil</div>
                        <h3 class="fw-bold mb-3">Sejarah Singkat</h3>
                        <p class="text-secondary lh-lg">
                            Balai Desa Pondokjoyo menjadi bagian penting dalam penyelenggaraan
                            pemerintahan dan pelayanan masyarakat di tingkat desa. Informasi sejarah
                            yang lebih spesifik dapat disesuaikan dengan data resmi Pemerintah Desa Pondokjoyo.
                        </p>
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="vision-box">
                        <div class="section-label text-white">Visi & Misi</div>
                        <h3 class="fw-bold">Melayani dengan baik, membangun bersama.</h3>
                        <p class="mt-3">Mewujudkan pemerintahan desa yang transparan, tertib, responsif, dan
                            berorientasi pada pelayanan masyarakat.</p>
                        <p class="mb-0"><strong>Misi:</strong> meningkatkan kualitas pelayanan, mendukung pembangunan
                            desa, keterbukaan informasi, dan partisipasi masyarakat.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="service-section" id="services">
        <div class="container">
            <div class="text-center mb-5">
                <div class="section-label">Layanan</div>
                <h2 class="section-title">Fungsi Utama Desa</h2>
            </div>
            <div class="row g-4">
                <div class="col-md-4">
                    <div class="service-card">
                        <div class="number">01</div>
                        <h4 class="mt-3">Pelayanan Administrasi</h4>
                        <p class="text-secondary lh-lg">Pelayanan berbagai kebutuhan administrasi dan dokumen
                            masyarakat.</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="service-card">
                        <div class="number">02</div>
                        <h4 class="mt-3">Pelayanan Informasi</h4>
                        <p class="text-secondary lh-lg">Memberikan informasi terkait program, kegiatan, dan pelayanan
                            desa.</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="service-card">
                        <div class="number">03</div>
                        <h4 class="mt-3">Pembangunan Desa</h4>
                        <p class="text-secondary lh-lg">Mendukung pembangunan serta kegiatan pemberdayaan masyarakat
                            desa.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="activities">
        <div class="container">
            <div class="text-center mb-5">
                <div class="section-label">Kegiatan</div>
                <h2 class="section-title">Kegiatan Desa</h2>
                <p class="section-subtitle mx-auto">Bagian ini dapat diisi dengan dokumentasi kegiatan Balai Desa
                    Pondokjoyo.</p>
            </div>
            <div class="row g-4">
                <div class="col-md-4">
                    <div class="activity">
                        <img src="assets/foto-kegiatan-1.jpg" onerror="this.src='assets/foto-balai-desa.jpg'"
                            alt="Kegiatan Desa">
                        <div class="activity-body">
                            <div class="number">KEGIATAN 01</div>
                            <h5 class="fw-bold mt-2">Kegiatan Masyarakat</h5>
                            <p class="text-secondary mb-0">Dokumentasi kegiatan masyarakat desa.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="activity">
                        <img src="assets/foto-kegiatan-2.jpg" onerror="this.src='assets/foto-balai-desa.jpg'"
                            alt="Kegiatan Desa">
                        <div class="activity-body">
                            <div class="number">KEGIATAN 02</div>
                            <h5 class="fw-bold mt-2">Pelayanan Desa</h5>
                            <p class="text-secondary mb-0">Dokumentasi pelayanan di Balai Desa.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="activity">
                        <img src="assets/foto-kegiatan-3.jpg" onerror="this.src='assets/foto-balai-desa.jpg'"
                            alt="Kegiatan Desa">
                        <div class="activity-body">
                            <div class="number">KEGIATAN 03</div>
                            <h5 class="fw-bold mt-2">Program Desa</h5>
                            <p class="text-secondary mb-0">Dokumentasi program dan kegiatan desa.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="contact-section" id="contact">
        <div class="container">
            <div class="row g-4">
                <div class="col-lg-5">
                    <div class="section-label text-white">Kontak & Lokasi</div>
                    <h2 class="section-title text-white mb-4">Temukan Balai Desa Pondokjoyo</h2>
                    <div class="contact-card">
                        <div class="contact-item"><i class="bi bi-geo-alt-fill"></i>
                            <div><small>Alamat</small>Jl.Jambesongo No.1.PondokJoyo</div>
                        </div>
                        <div class="contact-item"><i class="bi bi-telephone-fill"></i>
                            <div><small>Telepon</small>(0331)5102507</div>
                        </div>
                        <div class="contact-item"><i class="bi bi-envelope-fill"></i>
                            <div><small>Email</small>diskominfo@jemberkab.go.id</div>
                        </div>
                        <div class="contact-item mb-0"><i class="bi bi-globe2"></i>
                            <div><small>Website</small>Resmi Desa</div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-7">
                    <iframe class="map"
                        src="https://www.google.com/maps?q=Balai%20Desa%20Pondokjoyo%2C%20Jember&output=embed"
                        loading="lazy" allowfullscreen></iframe>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="container text-center">
            <p class="mb-1"><strong>Balai Desa Pondokjoyo</strong></p>
            <small>Website Company Profile • Tugas Pra-PKL RPL • 2026</small>
        </div>
    </footer>

    <a href="#home" class="top" aria-label="Kembali ke atas"><i class="bi bi-arrow-up"></i></a>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>

</html>
