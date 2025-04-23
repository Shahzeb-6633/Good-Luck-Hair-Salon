# Good-Luck-Hair-Salon
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Good Luck Hair Salon</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: 'Montserrat', sans-serif;
      background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      color: #fff;
    }

    header {
      background: #111;
      padding: 1rem;
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }

    nav h1 {
      font-size: 1.5rem;
      color: #fff;
      margin: 0;
    }

    .menu-toggle {
      display: none;
      font-size: 1.5rem;
      cursor: pointer;
      color: white;
    }

    nav ul {
      display: flex;
      gap: 1rem;
      list-style: none;
      padding-left: 0;
      margin: 0;
    }

    nav ul li a {
      color: #fff;
      text-decoration: none;
      font-weight: 700;
      transition: color 0.3s ease;
    }

    nav ul li a:hover {
      color: #ffdd57;
    }

    .tab-section {
      padding: 3rem 2rem;
      text-align: center;
      opacity: 0;
      transform: translateY(30px);
      animation: fadeInUp 1s forwards;
    }

    .tab-section:nth-child(2) { animation-delay: 0.3s; }
    .tab-section:nth-child(3) { animation-delay: 0.6s; }
    .tab-section:nth-child(4) { animation-delay: 0.9s; }
    .tab-section:nth-child(5) { animation-delay: 1.2s; }

    @keyframes fadeInUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .tab-section h2 {
      font-size: 2rem;
      margin-bottom: 1rem;
      color: #ffdd57;
    }

    .srk-img {
      width: 300px;
      height: auto;
      border-radius: 10px;
      margin: 1rem 0;
      box-shadow: 0 0 10px #000;
      animation: fadeIn 2s ease-in-out;
    }

    .tagline {
      font-size: 1.2rem;
      margin-bottom: 1rem;
    }

    .btn {
      display: inline-block;
      padding: 0.75rem 1.5rem;
      background: #ffdd57;
      color: #000;
      text-decoration: none;
      font-weight: bold;
      border-radius: 8px;
      transition: background 0.3s ease, transform 0.2s ease;
    }

    .btn:hover {
      background: #ffe784;
      transform: scale(1.05);
    }

    .services {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 2rem;
    }

    .service {
      background: #1f1f1f;
      padding: 1rem;
      border-radius: 10px;
      width: 220px;
      text-align: center;
      box-shadow: 0 0 10px #000;
      transition: transform 0.3s ease;
    }

    .service:hover {
      transform: translateY(-10px);
    }

    .service img {
      width: 100%;
      height: 150px;
      object-fit: cover;
      border-radius: 8px;
    }

    footer {
      background: #000;
      text-align: center;
      padding: 1rem;
      margin-top: 2rem;
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      .menu-toggle {
        display: block;
      }

      nav ul {
        flex-direction: column;
        width: 100%;
        display: none;
        margin-top: 1rem;
      }

      nav ul.show {
        display: flex;
      }

      nav ul li {
        margin-bottom: 0.5rem;
        text-align: center;
      }
    }
  </style>
</head>
<body>

  <header>
    <nav>
      <h1>Good Luck Hair Salon</h1>
      <div class="menu-toggle" onclick="toggleMenu()">☰</div>
      <ul id="menu">
        <li><a href="#home">Home</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#about">About Us</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home" class="tab-section">
    <h2>WELCOME TO GOOD LUCK HAIR SALON</h2>
    <img src="shah_rukh_khan_.jpeg" alt="Shahrukh Khan" class="srk-img">
    <p class="tagline">"Where Style Meets Royalty – Be the Star You Are!"</p>
    <a href="#contact" class="btn">BOOK YOUR APPOINTMENT</a>
  </section>

  <section id="services" class="tab-section">
    <h2>FEATURED SERVICES</h2>
    <div class="services">
      <div class="service">
        <img src="pexels-ryank-12304506.jpg" alt="Hair Cut for Men" />
        <h3>Hair Cut for Men</h3>
        <p>₹200</p>
      </div>
      <div class="service">
        <img src="MEN hair color.jpg" alt="Hair Colour for Men" />
        <h3>Hair Colour for Men</h3>
        <p>₹350</p>
      </div>
      <div class="service">
        <img src="pexels-thgusstavo-2881253.jpg" alt="Hair & Beard Styling for Men" />
        <h3>Hair and Beard Styling for Men</h3>
        <p>₹300</p>
      </div>
      <div class="service">
        <img src="pexels-n-voitkevich-8468039.jpg" alt="Hair Cut and Styling for Women" />
        <h3>Hair Cut and Styling for Women</h3>
        <p>₹400</p>
      </div>
      <div class="service">
        <img src="pexels-cottonbro-3993323.jpg" alt="Hair Colour for Women" />
        <h3>Hair Colour for Women</h3>
        <p>₹500</p>
      </div>
      <div class="service">
        <img src="pexels-cottonbro-4812649.jpg" alt="Skin Care for Men" />
        <h3>Skin Care for Men</h3>
        <p>₹250</p>
      </div>
      <div class="service">
        <img src="pexels-kerimeveyik-16100124.jpg" alt="Skin Care for Women" />
        <h3>Skin Care for Women</h3>
        <p>₹300</p>
      </div>
    </div>
  </section>

  <section id="about" class="tab-section">
    <h2>About Us</h2>
    <p>Welcome to GOOD LUCK HAIR SALON, where beauty is more than skin deep- it's an experience. From the moment you walk through our doors, you will be greeted with warmth and sophistication. We will give you absolutely the best. Whether you are preparing for a big event or indulging in a little self care. From precision haircuts and luxurious color treatments to facials and skin cares, every service is crafted with passion. Relax in our salon desingned to melt away the stress of the day and leave with glow that is both seen and felt.
    At GOOD LUCK HAIR SALON, we don't just enhance your beauty- we celebrate it. Come discover the difference a truly elevated salon experience can make. Contact us for booking.</p>
  </section>

  <section id="contact" class="tab-section">
    <h2>Contact Us</h2>
    <p><strong>Address:</strong> Shop-7, Ganpati Market, Sector-15, Rourkela - 769003, Odisha</p>
    <p><strong>Get Directions:</strong> <a href="https://maps.google.com" target="_blank">Google Maps</a></p>
    <p><strong>Phone:</strong> +91-9938646661</p>
  </section>

  <footer>
    <p>&copy; 2025 Good Luck Hair Salon. All rights reserved.</p>
  </footer>

  <script>
    function toggleMenu() {
      document.getElementById("menu").classList.toggle("show");
    }
  </script>
</body>
</html>
