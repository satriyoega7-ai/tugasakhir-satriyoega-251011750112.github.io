# tugasakhir-satriyoega-251011750112.github.io
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ElectroDesign - Desain Instalasi Listrik Rumah</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;
        }

        html {
            scroll-behavior: smooth;
        }

      body {
    background: linear-gradient(180deg,
        #1a0933 0%,
        #4b1d5a 25%,
        #ff6b6b 60%,
        #ff9a56 85%,
        #ffd56b 100%);
}

        /* HERO */
        .hero {
            width: 100%;
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 120px 8% 50px;
            background:
                linear-gradient(90deg,
                    rgba(2, 10, 20, 0.95) 0%,
                    rgba(2, 10, 20, 0.85) 50%,
                    rgba(2, 10, 20, 0.4) 100%),
                url('background-rumah.jpg');

            background-size: cover;
            background-position: center;
        }

        .hero-left {
            width: 50%;
        }

        .logo h2 {
            color: white;
            font-size: 40px;
        }

        .logo span {
            color: #ffc107;
        }

        .logo p {
            color: #ddd;
            margin-top: 5px;
            margin-bottom: 40px;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 40px;
        }

        .logo img {
            width: 80px;
            height: auto;
        }

        .logo-text h2 {
            color: white;
            font-size: 40px;
            margin: 0;
        }

        .logo-text span {
            color: #ffc107;
        }

        .logo-text p {
            color: #ddd;
            margin-top: 5px;
        }

        .hero-left h1 {
            color: white;
            font-size: 70px;
            line-height: 1.1;
            text-transform: uppercase;
        }

        .highlight {
            color: #ffc107;
        }

        .desc {
            color: #ddd;
            font-size: 22px;
            margin-top: 25px;
            margin-bottom: 35px;
        }

        .btn {
            display: inline-block;
            padding: 15px 35px;
            background: #ffc107;
            color: black;
            text-decoration: none;
            border-radius: 8px;
            font-weight: bold;
            transition: .3s;
        }

        .btn:hover {
            background: #ffcf33;
        }

        .hero-right {
            width: 50%;
            text-align: right;
        }

        .hero-right img {
            width: 100%;
            max-width: 800px;
        }

        /* KONSULTASI */
        .konsultasi {
            padding: 80px 10%;
            background: #0b1b2b;
            color: white;
        }

        .judul-konsultasi {
            text-align: center;
            margin-bottom: 40px;
        }

        .judul-konsultasi h2 {
            font-size: 42px;
            color: #ffc107;
            margin-bottom: 10px;
        }

        .judul-konsultasi p {
            color: #ddd;
        }

        .form-konsultasi {
            max-width: 800px;
            margin: auto;
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .form-konsultasi input,
        .form-konsultasi select,
        .form-konsultasi textarea {
            padding: 15px;
            border: none;
            border-radius: 8px;
            font-size: 16px;
        }

        .form-konsultasi textarea {
            resize: none;
        }

        .form-konsultasi button {
            padding: 15px;
            background: #ffc107;
            border: none;
            border-radius: 8px;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            transition: .3s;
        }

        .form-konsultasi button:hover {
            background: #ffcf33;
        }

        /* FOOTER */
        footer {
            background: #06111d;
            color: white;
            text-align: center;
            padding: 20px;
        }

        /* RESPONSIVE */
        @media screen and (max-width:992px) {

            .hero {
                flex-direction: column;
                justify-content: center;
                text-align: center;
                padding: 40px 20px;
            }

            .hero-left,
            .hero-right {
                width: 100%;
            }

            .hero-left h1 {
                font-size: 42px;
            }

            .logo h2 {
                font-size: 32px;
            }

            .desc {
                font-size: 18px;
            }

            .hero-right {
                width: 100%;
                margin-top: 30px;
                min-height: 300px;
            }

            .hero-right img {
                max-width: 100%;
            }

            .form-konsultasi {
                width: 100%;
            }

        }

        /* TENTANG KAMI */
        .tentang-container {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 40px;
            flex-wrap: wrap;
        }

        .tentang-gambar {
            flex: 1;
            text-align: center;
        }

        .tentang-gambar img {
            width: 100%;
            max-width: 350px;
            /* Perkecil gambar */
            height: auto;
            border-radius: 12px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }

        .tentang-text {
            flex: 2;
            color: #ddd;
            line-height: 1.8;
            text-align: justify;
        }

        @media screen and (max-width:576px) {

            .hero {
                padding: 20px;
            }

            .logo h2 {
                font-size: 24px;
            }

            .logo p {
                font-size: 14px;
            }

            .hero-left h1 {
                font-size: 30px;
            }

            .desc {
                font-size: 16px;
            }

            .btn {
                width: 100%;
                text-align: center;
            }

            .hero-right {
                width: 100%;
                min-height: 250px;
            }

            .konsultasi {
                padding: 50px 20px;
            }

            .form-konsultasi input,
            .form-konsultasi select,
            .form-konsultasi textarea,
            .form-konsultasi button {
                width: 100%;
            }

            .navbar {
                flex-direction: column;
                gap: 10px;
            }

            .menu {
                gap: 15px;
            }

        }

        .hero-right {
            position: relative;
            width: 50%;
            min-height: 350px;
            overflow: hidden;
        }

        .slide {
            position: absolute;
            inset: 0;
            width: 100%;
            height: 100%;
            object-fit: contain;
            opacity: 0;
            transition: opacity 1s;
        }

        .slide.active {
            opacity: 1;
        }

        .hero-right img {
            display: block;
        }

        @media screen and (max-width:576px) {

            .hero-right {
                min-height: 300px;
            }

            .slide {
                object-fit: contain;
            }

        }

        /* NAVBAR */

        .navbar {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            padding: 18px 8%;
            background: rgba(7, 19, 33, .95);
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 1000;
        }

        .logo-nav h2 {
            color: white;
            font-size: 28px;
        }

        .logo-nav span {
            color: #ffc107;
        }

        .logo-nav {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .logo-nav img {
            width: 55px;
            height: auto;
        }

        .menu {
            display: flex;
            gap: 30px;
            list-style: none;
        }

        .menu a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            transition: .3s;
        }

        .menu a:hover {
            color: #ffc107;
        }
    </style>
</head>

<body>

    <!-- NAVBAR -->
    <nav class="navbar">
        <div class="logo-nav">
            <img src="gambar5.png" alt="Logo">

            <h2>ELECTRO<span>DESIGN</span></h2>
        </div>

        <ul class="menu">
            <li><a href="#home">Home</a></li>
            <li><a href="#tentang">Tentang</a></li>
            <li><a href="#kontak">Kontak</a></li>
        </ul>
    </nav>

    <!-- HERO -->
    <section id="home" class="hero">

        <div class="hero-left">

            <div class="logo">
                <img src="gambar5.png" alt="Logo ElectroDesign">

                <div class="logo-text">
                    <h2>ELECTRO<span>DESIGN</span></h2>
                    <p>DESAIN INSTALASI LISTRIK RUMAH</p>
                </div>
            </div>

            <h1>
                JASA PEMBUATAN <br>
                DESAIN INSTALASI <br>
                <span class="highlight">LISTRIK RUMAH</span>
            </h1>

            <p class="desc">
                Desain tepat, instalasi aman, rumah nyaman dan hemat energi.
            </p>

            <a href="#kontak" class="btn">
                Konsultasi Gratis
            </a>

        </div>

        <div class="hero-right">
            <img class="slide active" src="gambar1.png" alt="gambar 1">

            <img class="slide" src="gambar2.png" alt="gambar 2">

            <img class="slide" src="gambar4.png" alt="gambar 3">

        </div>


    </section>

    <!-- TENTANG -->
    <section id="tentang" class="konsultasi">

        <div class="judul-konsultasi">
            <h2>Tentang Kami</h2>
        </div>

        <div class="tentang-container">

            <div class="tentang-gambar">
                <img src="gambar3.png" alt="Desain Instalasi Listrik">
            </div>

            <div class="tentang-text">
                <p>
                    ElectroDesign adalah jasa pembuatan desain instalasi listrik rumah
                    yang berfokus pada keamanan, efisiensi, dan kenyamanan setiap hunian.
                    Kami membantu merancang sistem kelistrikan mulai dari jalur instalasi,
                    penempatan titik lampu, stop kontak, saklar, hingga perhitungan kebutuhan
                    daya listrik sesuai kebutuhan rumah Anda.
                </p>

                <br>

                <p>
                    Setiap desain dibuat secara rapi, terstruktur, dan mengikuti standar
                    kelistrikan yang berlaku sehingga proses pemasangan menjadi lebih mudah,
                    aman, serta mengurangi risiko gangguan listrik di masa mendatang.
                    Dengan tenaga yang berpengalaman, ElectroDesign siap memberikan solusi
                    terbaik untuk kebutuhan instalasi listrik rumah Anda.
                </p>

            </div>

        </div>

    </section>

    <!-- KONSULTASI -->
    <section id="kontak" class="konsultasi">


        <div class="judul-konsultasi">
            <h2>Konsultasi Gratis</h2>
            <p>
                Isi formulir berikut dan kami akan segera menghubungi Anda.
            </p>
        </div>

        <form class="form-konsultasi" action="https://formsubmit.co/satriyoega7@gmail.com" method="POST">

            <input type="hidden" name="_subject" value="Konsultasi Baru ElectroDesign">

            <input type="hidden" name="_captcha" value="false">
            <input type="hidden" name="_template" value="table">

            <input type="hidden" name="_next" value="https://satriyoidebisnis.netlify.app/#kontak"> <input type="text"
                id="nama" name="nama" placeholder="Nama Lengkap" autocomplete="name" required>

            <input type="tel" id="wa" name="whatsapp" placeholder="Nomor WhatsApp" autocomplete="tel" required>

            <input type="email" id="email" name="email" placeholder="Alamat Email" autocomplete="email">

            <select name="layanan" required>
                <option value="">Pilih Layanan</option>
                <option>Desain Instalasi Rumah</option>
                <option>Perhitungan Kebutuhan Daya</option>
                <option>Gambar Kerja Instalasi</option>
                <option>Paket Lengkap Desain Instalasi</option>
            </select>

            <textarea id="pesan" name="pesan" rows="5" placeholder="Jelaskan kebutuhan proyek Anda..."
                required></textarea>

            <button type="submit" id="kirim">Kirim Konsultasi</button>

        </form>

    </section>

    <footer>
        © 2026 ElectroDesign | Desain Instalasi Listrik Rumah
    </footer>


    <script>
        const slides = document.querySelectorAll(".slide");
        let currentSlide = 0;

        setInterval(() => {

            slides[currentSlide].classList.remove("active");

            currentSlide++;

            if (currentSlide >= slides.length) {
                currentSlide = 0;
            }

            slides[currentSlide].classList.add("active");

        }, 3000);

    </script>

    <script>
        document.querySelector(".form-konsultasi").addEventListener("submit", function (e) {
            e.preventDefault(); // WAJIB: stop form reload

            const nama = document.getElementById("nama").value;
            const wa = document.getElementById("wa").value;
            const email = document.getElementById("email").value;
            const pesan = document.getElementById("pesan").value;

            const text = `Halo Admin ElectroDesign

Nama: ${nama}
WA: ${wa}
Email: ${email}
Pesan: ${pesan}`;

            const url = "https://wa.me/6283841315902?text=" + encodeURIComponent(text);

            // buka WA dulu
            window.open(url, "_blank");

            // baru kirim ke formsubmit
            setTimeout(() => {
                e.target.submit();
            }, 500);
        });
    </script>

</body>

</html>
