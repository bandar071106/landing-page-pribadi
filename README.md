<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Landing Page Pribadi - Dark Mode</title>

    <!-- CSS eksternal -->
    <link rel="stylesheet" href="style.css">

    <!-- CSS internal -->
    <style>
        /* Warna highlight elemen tertentu */
        .highlight {
            color: #ffd54d;
        }
    </style>
</head>
<body>

    <!-- HEADER -->
    <header class="hero">
        <h1 class="highlight">Halo, Saya Muhammad Bandar</h1>
        <p>Web Developer | UI Designer | Freelancer</p>
        <a href="#profil" class="btn">Lihat Profil</a>
    </header>

    <!-- NAVIGATION -->
    <nav>
        <ul>
            <li><a href="#">Beranda</a></li>
            <li><a href="#profil">Tentang</a></li>
            <li><a href="#proyek">Proyek</a></li>
            <li><a href="#hobi">Hobi</a></li>
            <li><a href="#sosmed">Sosial Media</a></li>
        </ul>
    </nav>

    <!-- MAIN -->
    <main class="container">

        <!-- PROFIL -->
        <section id="profil" class="box">
            <h2>Tentang Saya</h2>
            <p>
                Saya adalah seorang web developer yang sedang belajar membangun website
                modern, responsif, dan enak dilihat. Saya tertarik mempelajari teknologi
                baru serta mendesain UI yang simple dan estetik.
            </p>
        </section>

        <!-- PROYEK -->
        <section id="proyek" class="box">
            <h2>Proyek Saya</h2>
            <ul>
                <li>Aplikasi To-Do List</li>
                <li>Website Portofolio</li>
                <li>UI/UX E-Commerce</li>
            </ul>
        </section>

        <!-- HOBI -->
        <section id="hobi" class="box">
            <h2>Hobi</h2>
            <ul>
                <li>Skateboard</li>
                <li>Fotografi</li>
                <li>Ngoding</li>
            </ul>
        </section>

        <!-- SOSIAL MEDIA -->
        <section id="sosmed" class="box">
            <h2>Sosial Media</h2>
            <ul>
                <li><a href="#" target="_blank">
                Instagram</a></li>
                <li><a href="#" target="_blank">Github</a></li>
                <li><a href="#" target="_blank">LinkedIn</a></li>
            </ul>
        </section>
    </main>

    <!-- FOOTER -->
    <footer>
        <p>Email : muhammadbandarsudarman@gmail.com</p>
    </footer>

</body>
</html>


/* ===== GLOBAL ===== */
body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    background: #0d0d0d;
    color: #e8e8e8;
}

/* ===== HEADER ===== */
.hero {
    text-align: center;
    padding: 90px 20px;
    background: linear-gradient(180deg, #111, #1b1b1b);
    border-bottom: 2px solid #ffd54d;
    margin-bottom: 30px;
}

.btn {
    display: inline-block;
    padding: 10px 20px;
    background: #ffd54d;
    color: #000;
    border-radius: 6px;
    text-decoration: none;
    font-weight: bold;
    transition: 0.3s;
}

/* Hover tombol */
.btn:hover {
    transform: scale(1.05);
    background: #fff;
}

/* ===== NAVBAR ===== */
nav {
    display: flex;
    justify-content: center;
    padding: 12px;
    background: #111;
    margin-bottom: 20px;
}

nav ul {
    list-style: none;
    display: flex; /* Flexbox */
    gap: 25px;
    padding: 0;
}

nav a {
    color: #ffd54d;
    text-decoration: none;
    font-weight: bold;
    padding: 6px 12px;
    transition: 0.3s;
}

/* Hover navbar */
nav a:hover {
    background: #ffd54d;
    color: #000;
    border-radius: 4px;
}

/* ===== MAIN ===== */
.container {
    display: flex; /* Flexbox */
    flex-wrap: wrap;
    gap: 20px;
    padding: 20px;
}

/* BOX */
.box {
    flex: 1;
    min-width: 250px;
    background: #1a1a1a;
    border: 1px solid #ffd54d; /* box model */
    padding: 20px;            /* box model */
    border-radius: 12px;
    margin-bottom: 20px;      /* box model */
    transition: 0.3s;
}

.box:hover {
    transform: translateY(-5px);
    background: #242424;
}

/* ===== FOOTER ===== */
footer {
    text-align: center;
    padding: 15px;
    background: #111;
    border-top: 1px solid #ffd54d;
    margin-top: 20px;
}

/*
=====================================================
KOMENTAR WAJIB
- Flexbox digunakan pada nav & container
- Margin, padding, border: diterapkan minimal pada .box, footer, hero
- Hover: tombol & nav link & box
=====================================================
*/
