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
            background-color: #fcfcfc;
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

        /* HERO SECTION - Updated with your Image and Fixed Blurriness */
        .hero {
            height: 60vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            /* Your specific image link added below */
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://i.ibb.co/HTCNknK1/7.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed; /* This makes it look sharper/smoother */
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 3rem auto;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .image-box {
            width: 100%;
            height: 220px;
            overflow: hidden;
            border-radius: 12px;
            cursor: pointer;
            border: 2px solid #eee;
            transition: transform 0.3s, box-shadow 0.3s;
            background-color: #ddd;
        }

        .image-box:hover {
            transform: scale(1.03);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }

        .image-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

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
            cursor: zoom-out;
        }

        .lightbox img {
            max-width: 90%;
            max-height: 85%;
            border: 4px solid white;
            border-radius: 8px;
        }

        .close-btn {
            position: absolute;
            top: 20px;
            right: 30px;
            color: white;
            font-size: 45px;
            cursor: pointer;
            font-weight: bold;
        }

        .contact-section {
            background: #ecf0f1;
            padding: 4rem 5%;
            text-align: center;
        }

        .contact-flex {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
        }

        .contact-card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            min-width: 300px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            border-top: 5px solid #f1c40f;
        }

        /* NEW: Call Now Button Style */
        .call-btn {
            display: inline-block;
            margin-top: 20px;
            background: #27ae60;
            color: white;
            padding: 12px 25px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            transition: background 0.3s;
        }

        .call-btn:hover {
            background: #2ecc71;
        }

        footer {
            background: #2c3e50;
            color: white;
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
        <a href="tel:9664782852" class="call-btn">📞 Book Now</a>
    </section>

    <section class="container" id="gallery">
        <h2 style="text-align: center; font-size: 2rem; margin-bottom: 30px;">Our Fleet &amp; Gallery</h2>
        <div class="grid">
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/Q30hCpJm/1.jpg')"><img src="https://i.ibb.co/Q30hCpJm/1.jpg" alt="Rajveer Car 1"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/C3mGSQhG/2.jpg')"><img src="https://i.ibb.co/C3mGSQhG/2.jpg" alt="Rajveer Car 2"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/Swv773mb/3.jpg')"><img src="https://i.ibb.co/Swv773mb/3.jpg" alt="Rajveer Car 3"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/KcvW0qDc/4.jpg')"><img src="https://i.ibb.co/KcvW0qDc/4.jpg" alt="Rajveer Car 4"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/1GRLfwwW/5.jpg')"><img src="https://i.ibb.co/1GRLfwwW/5.jpg" alt="Rajveer Car 5"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/n880Npgc/6.jpg')"><img src="https://i.ibb.co/n880Npgc/6.jpg" alt="Rajveer Car 6"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/HTCNknK1/7.jpg')"><img src="https://i.ibb.co/HTCNknK1/7.jpg" alt="Rajveer Car 7"></div>
            <div class="image-box" onclick="openLightbox('https://i.ibb.co/B5TwY94p/8.jpg')"><img src="https://i.ibb.co/B5TwY94p/8.jpg" alt="Rajveer Car 8"></div>
        </div>
    </section>

    <div id="lightboxOverlay" class="lightbox" onclick="closeLightbox()">
        <span class="close-btn">&times;</span>
        <img id="lightboxImg" src="" alt="Full View">
    </div>

    <section class="contact-section" id="contact">
        <h2 style="margin-bottom: 40px;">Contact Our Experts</h2>
        <div class="contact-flex">
            <div class="contact-card">
                <h3>BHIKHUBHA SODHA</h3>
                <p>📞 9664782852</p>
                <p>📞 9586574902</p>
            </div>
            <div class="contact-card">
                <h3>NARPALSINH JADEJA</h3>
                <p>📞 9687213791</p>
                <p>📞 9723697117</p>
                <p>✉️ <a href="mailto:Narpalsinhjadeja86@gmail.com">Narpalsinhjadeja86@gmail.com</a></p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 Rajveer Tours and Travels. All rights reserved.</p>
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
