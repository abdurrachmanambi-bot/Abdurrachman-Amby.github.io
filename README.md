# Abdurrachman-Amby.github.io
```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio | Abdurrachman Amby</title>

    <style>
        *{
            margin:0;
            padding:0;
            box-sizing:border-box;
            font-family:'Segoe UI', sans-serif;
        }

        body{
            background:#f5f7fa;
            color:#333;
        }

        /* NAVBAR */
        header{
            background:#0d1b2a;
            color:white;
            padding:15px 8%;
            display:flex;
            justify-content:space-between;
            align-items:center;
            position:sticky;
            top:0;
            z-index:1000;
        }

        .logo{
            display:flex;
            align-items:center;
            gap:12px;
        }

        .logo img{
            width:50px;
            height:50px;
        }

        .logo h2{
            font-size:20px;
        }

        nav ul{
            list-style:none;
            display:flex;
            gap:30px;
            align-items:center;
        }

        nav ul li{
            position:relative;
        }

        nav ul li a{
            color:white;
            text-decoration:none;
            font-weight:500;
        }

        nav ul li a:hover{
            color:#00b4d8;
        }

        /* Dropdown */
        .dropdown{
            display:none;
            position:absolute;
            top:35px;
            left:0;
            background:white;
            min-width:200px;
            border-radius:10px;
            overflow:hidden;
            box-shadow:0 5px 15px rgba(0,0,0,0.2);
        }

        .dropdown a{
            display:block;
            color:#333;
            padding:12px 15px;
        }

        .dropdown a:hover{
            background:#f0f0f0;
        }

        nav ul li:hover .dropdown{
            display:block;
        }

        /* HERO */
        .hero{
            min-height:90vh;
            display:flex;
            align-items:center;
            justify-content:center;
            gap:60px;
            padding:60px 8%;
            flex-wrap:wrap;
        }

        .hero-text{
            flex:1;
            min-width:300px;
        }

        .hero-text h1{
            font-size:48px;
            color:#0d1b2a;
        }

        .hero-text h3{
            margin-top:10px;
            color:#0077b6;
        }

        .hero-text p{
            margin-top:20px;
            line-height:1.8;
            text-align:justify;
        }

        .btn{
            display:inline-block;
            margin-top:25px;
            padding:12px 25px;
            background:#0077b6;
            color:white;
            text-decoration:none;
            border-radius:8px;
        }

        .btn:hover{
            background:#023e8a;
        }

        .hero-image{
            flex:1;
            text-align:center;
            min-width:300px;
        }

        .hero-image img{
            width:320px;
            height:320px;
            object-fit:cover;
            border-radius:50%;
            border:8px solid #0077b6;
        }

        /* BIODATA */
        .section{
            padding:80px 8%;
        }

        .title{
            text-align:center;
            margin-bottom:40px;
            color:#0d1b2a;
        }

        .biodata{
            display:grid;
            grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
            gap:20px;
        }

        .card{
            background:white;
            padding:25px;
            border-radius:15px;
            box-shadow:0 5px 15px rgba(0,0,0,0.1);
        }

        .card h4{
            margin-bottom:10px;
            color:#0077b6;
        }

        /* PROJECT */
        .project-grid{
            display:grid;
            grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
            gap:25px;
        }

        .project-card{
            background:white;
            padding:25px;
            border-radius:15px;
            box-shadow:0 5px 15px rgba(0,0,0,0.1);
        }

        /* GALERY */
        .gallery{
            display:grid;
            grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
            gap:20px;
        }

        .gallery img{
            width:100%;
            height:250px;
            object-fit:cover;
            border-radius:15px;
        }

        /* CONTACT */
        .contact{
            text-align:center;
        }

        .contact p{
            margin:10px 0;
            font-size:18px;
        }

        footer{
            background:#0d1b2a;
            color:white;
            text-align:center;
            padding:20px;
        }

        @media(max-width:768px){
            .hero-text h1{
                font-size:36px;
            }

            nav ul{
                gap:15px;
            }
        }
    </style>
</head>

<body>

<header>
    <div class="logo">
        <img src="logo-ekonomi-informasi.png" alt="Logo">
        <h2>Ekonomi Informasi</h2>
    </div>

    <nav>
        <ul>
            <li><a href="#home">Home</a></li>

            <li>
                <a href="#">Project ▼</a>
                <div class="dropdown">
                    <a href="#team">Project Team</a>
                    <a href="#individu">Project Individu</a>
                </div>
            </li>

            <li><a href="#gallery">Gallery Foto</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>

<!-- HOME -->
<section class="hero" id="home">

    <div class="hero-text">
        <h1>Abdurrachman Amby</h1>
        <h3>Mahasiswa Sistem Informasi</h3>

        <p>
            Selamat datang di website portofolio pribadi saya.
            Website ini berisi informasi profil, pengalaman,
            proyek akademik, penelitian, serta dokumentasi kegiatan
            yang telah saya kerjakan selama menempuh pendidikan
            di bidang Sistem Informasi.
        </p>

        <a href="#contact" class="btn">
            Hubungi Saya
        </a>
    </div>

    <div class="hero-image">
        <img src="foto-abdurrachman.jpg" alt="Foto Mahasiswa">
    </div>

</section>

<!-- BIODATA -->
<section class="section">
    <h2 class="title">Biodata Mahasiswa</h2>

    <div class="biodata">

        <div class="card">
            <h4>Nama Lengkap</h4>
            <p>Abdurrachman Amby</p>
        </div>

        <div class="card">
            <h4>NIM</h4>
            <p>Isi NIM Anda</p>
        </div>

        <div class="card">
            <h4>Program Studi</h4>
            <p>Sistem Informasi</p>
        </div>

        <div class="card">
            <h4>Universitas</h4>
            <p>Universitas Bakrie</p>
        </div>

        <div class="card">
            <h4>Email</h4>
            <p>emailanda@gmail.com</p>
        </div>

        <div class="card">
            <h4>Keahlian</h4>
            <p>
                Data Analytics, UI/UX,
                Business Analysis, Web Development,
                Data Mining, Machine Learning
            </p>
        </div>

    </div>
</section>

<!-- PROJECT TEAM -->
<section class="section" id="team">

    <h2 class="title">Project Team</h2>

    <div class="project-grid">

        <div class="project-card">
            <h3>AFATO</h3>
            <p>
                Platform digital layanan otomotif
                berbasis teknologi untuk meningkatkan
                efisiensi layanan kendaraan.
            </p>
        </div>

        <div class="project-card">
            <h3>Data Mining Export Batik</h3>
            <p>
                Analisis clustering ekspor batik
                menggunakan metode K-Means.
            </p>
        </div>

    </div>

</section>

<!-- PROJECT INDIVIDU -->
<section class="section" id="individu">

    <h2 class="title">Project Individu</h2>

    <div class="project-grid">

        <div class="project-card">
            <h3>Skripsi Sistem Informasi</h3>
            <p>
                Penelitian terkait implementasi
                teknologi informasi dalam bisnis digital.
            </p>
        </div>

        <div class="project-card">
            <h3>Dashboard Analytics</h3>
            <p>
                Dashboard interaktif menggunakan
                Python dan Streamlit.
            </p>
        </div>

    </div>

</section>

<!-- GALERY -->
<section class="section" id="gallery">

    <h2 class="title">Gallery Foto</h2>

    <div class="gallery">

        <img src="foto1.jpg" alt="">
        <img src="foto2.jpg" alt="">
        <img src="foto3.jpg" alt="">
        <img src="foto4.jpg" alt="">

    </div>

</section>

<!-- CONTACT -->
<section class="section contact" id="contact">

    <h2 class="title">Contact</h2>

    <p><strong>Email :</strong> emailanda@gmail.com</p>
    <p><strong>WhatsApp :</strong> +62xxxxxxxxxx</p>
    <p><strong>LinkedIn :</strong> linkedin.com/in/abdurrachmanamby</p>
    <p><strong>GitHub :</strong> github.com/abdurrachmanamby</p>

</section>

<footer>
    © 2026 Portfolio Mahasiswa - Abdurrachman Amby
</footer>

</body>
</html>
```
