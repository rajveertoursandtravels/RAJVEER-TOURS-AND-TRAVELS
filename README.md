<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rajveer Tours and Travels</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            line-height: 1.6;
            color: #333;
            scroll-behavior: smooth;
            background-color: #f4f4f4;
        }

        header {
            background: #2c3e50;
            color: #fff;
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #f1c40f;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            margin-left: 20px;
            font-weight: 500;
        }

        /* WORLD SECTION - Updated with your requested image */
        .hero {
            height: 75vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://i.ibb.co/JWWj2rrk/1.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed; 
            background-repeat: no-repeat;
        }

        .hero h1 {
            font-size: clamp(2.5rem, 6vw, 4rem);
            margin: 0;
            text-shadow: 3px 3px 15px rgba(0,0,0,1);
        }

        .hero p {
            font-size: 1.3rem;
            margin-top: 10px;
            text-shadow: 2px 2px 10px rgba(0,0,0,0.8);
        }

        .container {
            width: 95%;
            max-width: 1200px;
            margin: -50px auto 3rem; 
            background: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.2);
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .image-box {
            width: 100%;
            height: 350px; 
            overflow: hidden;
            border-radius: 15px;
            cursor: pointer;
            border: 1px solid #eee;
            background-color: #ffffff;
            transition: 0.3s ease;
        }

        .image-box:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 25px rgba(0,0,0,0.2);
        }

        .image-box img {
            width: 100%;
            height: 100%;
            object-fit: contain; 
            image-rendering: -webkit-optimize-contrast; 
            background: #fff;
        }

        /* LIGHTBOX POPUP */
        .lightbox {
            display: none;
            position: fixed;
            z-index: 2000;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.9);
            justify-content: center;
            align-items: center;
        }

        .lightbox img {
            max-width: 95%;
            max-height: 90%;
            border: 3px solid #f1c40f;
        }

        .close-btn {
            position: absolute;
            top: 20px;
            right: 40px;
            color: #f1c40f;
            font-size: 60px;
            cursor: pointer;
        }

        /* CONTACT SECTION */
        .contact-section {
            background: #2c3e50;
            color: white;
            padding: 5rem 5%;
            text-align: center;
        }

        .contact-flex {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 40px;
            margin-top: 30px;
        }

        .contact-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 40px;
            border-radius: 20px;
            width: 320px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(10px);
        }

        .call-btn {
            display: inline-block;
            margin-top: 20px;
            background: #f1c40f;
            color: #2c3e50;
            padding: 15px 40px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
        }

        footer {
            background: #1a252f;
            color: #bdc3c7;
            text-align: center;
            padding: 2rem;
        }
    </style>
</head>

<body>

    <header>
        <div class="logo">RAJVEER TOURS AND TRAVELS</div>
        <nav>
            <a href="#home">Home</a>
            <a href="#gallery">Gallery</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="hero" id="home">
        <h1>Explore The World With Us</h1>
        <p>Premium AC &amp; Non-AC Car Rentals</p>
    </section>

    <section class="container" id="gallery">
        <h2 style="text-align: center; font-size: 2.2rem; margin-bottom: 40px; color: #2c3e50;">Our Professional Fleet</h2>
        <div class="grid">
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/67TcsmTY/89.jpg')"><img src="https://i.ibb.co/67TcsmTY/89.jpg" alt="Car 89"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/840fyYPk/7.jpg')"><img src="https://i.ibb.co/840fyYPk/7.jpg" alt="Car 7"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/fzFnBtNZ/6.jpg')"><img src="https://i.ibb.co/fzFnBtNZ/6.jpg" alt="Car 6"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/m5XDDCGd/5.jpg')"><img src="https://i.ibb.co/m5XDDCGd/5.jpg" alt="Car 5"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/1GxNNqmS/4.jpg')"><img src="https://i.ibb.co/1GxNNqmS/4.jpg" alt="Car 4"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/DPSNJC3S/3.jpg')"><img src="https://i.ibb.co/DPSNJC3S/3.jpg" alt="Car 3"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/yFFYCN9g/2.jpg')"><img src="https://i.ibb.co/yFFYCN9g/2.jpg" alt="Car 2"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/JWWj2rrk/1.jpg')"><img src="https://i.ibb.co/JWWj2rrk/1.jpg" alt="Car 1"></div>
        </div>
    </section>

    <div id="lightboxOverlay" class="lightbox" onclick="closeLightbox()">
        <span class="close-btn">&times;</span>
        <img id="lightboxImg" src="" alt="View">
    </div>

    <section class="contact-section" id="contact">
        <h2>Contact Our Experts</h2>
        <div class="contact-flex">
            <div class="contact-card">
                <h3>BHIKHUBHA SODHA</h3>
                <p>📞 9664782852</p>
                <p>📞 9586574902</p>
                <a href="tel:9664782852" class="call-btn">Call Now</a>
            </div>
            <div class="contact-card">
                <h3>NARPALSINH JADEJA</h3>
                <p>📞 9687213791</p>
                <p>📞 9723697117</p>
                <a href="tel:9687213791" class="call-btn">Call Now</a>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 Rajveer Tours and Travels.</p>
    </footer>

    <script>
        function openLightbox(imageSrc) {
            const overlay = document.getElementById('lightboxOverlay');
            const bigImg = document.getElementById('lightboxImg');
            bigImg.src = imageSrc;
            overlay.style.display = 'flex';
            document.body.style.overflow = 'hidden';
        }

        function closeLightbox() {
            document.getElementById('lightboxOverlay').style.display = 'none';
            document.body.style.overflow = 'auto';
        }
    </script>

</body>
</html>
