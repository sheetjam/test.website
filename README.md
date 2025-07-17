
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>InSight Services</title>
  <style>
    
    /* ========= Base Styles ========= */

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      background: url("repeattest.jpg") center/cover repeat;
      font-family: Arial, sans-serif;
      color: #333;
      line-height: 1.6;
    }

    header {
      background: linear-gradient(
        90deg,
        rgba(0, 119, 204, 1) 0%,
        rgba(0, 139, 204, 0.87) 38%,
        rgba(0, 180, 204, 1) 100%
      );
      color: #fff;
      padding: .5em;
    }

    .header-top {
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
    }

    .logo-container {
      display: flex;
      align-items: center;
      gap: 1em;
    }

    .logo {
      width: 70px;
      height: auto;
      max-width: 100%;
    }

    /* ========= Navigation ========= */

    .hamburger {
      display: none;
      font-size: 2rem;
      cursor: pointer;
      color: #fff;
    }

    nav {
      background: #0077cc;
    }

    nav ul {
      display: flex;
      list-style: none;
      justify-content: center;
      gap: 2rem;
      padding: 1em;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
      padding: 0.5em;
      transition: background 0.3s;
    }

    nav a:hover {
      background: rgba(255, 255, 255, 0.2);
      border-radius: 5px;
    }

    /* ========= Main Layout ========= */

    main {
      display: flex;
      flex-wrap: wrap;
      gap: 1em;
      padding: 1em;
    }

    .content {
      flex: 3 1 60%;
      background: #ffffffe8;
      padding: 1em;
      border-radius: 5px;
      font-size: 15px;
    }

    .sidebar {
      flex: 1 1 30%;
      background: #d9edf7;
      padding: 1em;
      border-radius: 5px;
    }

    footer {
      background: #333;
      color: #fff;
      text-align: center;
      padding: 1em;
      margin-top: 1em;
    }

    /* ========= Listings ========= */

    .listings-section {
      padding: 1em;
    }

    .listings-top {
      font-size: 1rem;
      text-align: center;
      color: #000;
      background-color: #ffffffe5;
      border-radius: 5px;
      padding: 0.5em;
      margin-bottom: 1em;
    }

    .listing-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 1em;
      justify-content: center;
    }

    .listing-card {
      flex: 1 1 20%;
      max-width: 350px;
      max-height: fit-content;
      background: white;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease;
    }

    .listing-card:hover {
      transform: scale(1.01);
    }

    .image-gallery {
      width: 100%;
      height: 300px;
      overflow: hidden;
    }

    .image-gallery .main-image {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .details {
      padding: 1rem;
    }

    .details h2 {
      margin: 0;
      font-size: 2rem;
      color: #2c3e50;
    }

    .location {
      color: #888;
      font-size: 0.95rem;
      margin-bottom: 1rem;
    }

    .description {
      margin-bottom: 1.5rem;
      color: #333;
    }

    .features {
      list-style: none;
      padding: 0;
      margin: 0 0 1.5rem 0;
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
    }

    .features li {
      background: #eaf1f8;
      padding: 0.2rem .25rem;
      border-radius: 5px;
      font-size: 0.95rem;
    }

    .btn {
      display: inline-block;
      background: #3498db;
      color: white;
      padding: 0.75rem 1.5rem;
      border-radius: 5px;
      text-decoration: none;
      transition: background 0.3s;
    }

    .btn:hover {
      background: #2980b9;
    }

    /* ========= Responsive ========= */

    @media (max-width: 768px) {
      .hamburger {
        display: block;
        order: 2;
      }

      nav {
        display: none;
      }

      nav.show {
        display: block;
      }

      nav ul {
        flex-direction: column;
        align-items: flex-start;
        gap: 0;
        padding: 0;
      }

      nav li {
        width: 100%;
      }

      nav a {
        display: block;
        width: 100%;
        padding: 1em;
        border-bottom: 1px solid rgba(255, 255, 255, 0.2);
      }

      .logo-container {
        flex: 1;
        order: 1;
      }

      .listing-card {
        flex: 1 1 100%;
      }
    }

  </style>
</head>
<body>
  <header>
    <div class="header-top">
      <div class="logo-container">
        <img src="emblem3.png" alt="InSight Services Logo" class="logo" />
        <h3>Where your dream home becomes reality</h3>
      </div>
      <div class="hamburger" onclick="toggleNav()">
        &#9776;
      </div>
    </div>

    <nav id="myLinks">
      <ul>
        <li><a href="#"></a></li>
        <li><a href="#">Placeholder</a></li>
        <li><a href="#">Locations</a></li>
        <li><a href="contact.htm">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section class="content">
      <h2>About Us</h2>
      <p>
        Thank you for visiting InSight Services. We are a privately owned company
        specializing in the purchasing and selling of properties. For the last
        30 years, we have been serving the people of Northeast Florida. We look
        forward to helping you in your home-buying journey.
      </p>
      <p>
        Additional text can be added here as needed. This is placeholder
        content.
      </p>
      <p>
        We are available 7 days a week. Please call or text us at
        <a href="tel:1234567890">123-456-7890</a> or email us at
        <a href="mailto:thisisatest@gmail.com">thisisatest@gmail.com</a>.
      </p>
    </section>
  </main>

  <section class="listings-section">
    <p class="listings-top">Here are some recently listed homes</p>
    <div class="listing-grid">
      <div class="listing-card">
        <div class="image-gallery">
          <img src="testlisting.jpg" alt="Exterior view of the home at 1234 Elm Street" class="main-image" loading="lazy" />
        </div>
        <div class="details">
          <h2>$599,000</h2>
          <p class="location">1234 Elm Street, Springfield, IL</p>
          <p class="description">Beautiful 4-bedroom family home...</p>
          <ul class="features">
            <li>🛏️ 4 Beds</li>
            <li>🛁 3 Baths</li>
            <li>📐 2,400 sqft</li>
            <li>🌳 Large backyard</li>
            <li>🚗 2-car garage</li>
          </ul>
          <a href="#" class="btn">Schedule a Tour</a>
        </div>
      </div>

      <div class="listing-card">
        <div class="image-gallery">
          <img src="testlisting.jpg" alt="Exterior view of the home at 1234 Elm Street" class="main-image" loading="lazy" />
        </div>
        <div class="details">
          <h2>$599,000</h2>
          <p class="location">1234 Elm Street, Springfield, IL</p>
          <p class="description">Beautiful 4-bedroom family home...</p>
          <ul class="features">
            <li>🛏️ 4 Beds</li>
            <li>🛁 3 Baths</li>
            <li>📐 2,400 sqft</li>
            <li>🌳 Large backyard</li>
            <li>🚗 2-car garage</li>
          </ul>
          <a href="#" class="btn">Schedule a Tour</a>
        </div>
      </div>
      <div class="listing-card">
        <div class="image-gallery">
          <img src="testlisting.jpg" alt="Exterior view of the home at 1234 Elm Street" class="main-image" loading="lazy" />
        </div>
        <div class="details">
          <h2>$599,000</h2>
          <p class="location">1234 Elm Street, Springfield, IL</p>
          <p class="description">Beautiful 4-bedroom family home...</p>
          <ul class="features">
            <li>🛏️ 4 Beds</li>
            <li>🛁 3 Baths</li>
            <li>📐 2,400 sqft</li>
            <li>🌳 Large backyard</li>
            <li>🚗 2-car garage</li>
          </ul>
          <a href="#" class="btn">Schedule a Tour</a>
        </div>
      </div>
    </div>
  </section>

  <section class="listings-section">
    <div class="listing-grid">
      <div class="listing-card">
        <div class="image-gallery">
          <img src="testlisting.jpg" alt="Exterior view of the home at 1234 Elm Street" class="main-image" loading="lazy" />
        </div>
        <div class="details">
          <h2>$599,000</h2>
          <p class="location">1234 Elm Street, Springfield, IL</p>
          <p class="description">Beautiful 4-bedroom family home...</p>
          <ul class="features">
            <li>🛏️ 4 Beds</li>
            <li>🛁 3 Baths</li>
            <li>📐 2,400 sqft</li>
            <li>🌳 Large backyard</li>
            <li>🚗 2-car garage</li>
          </ul>
          <a href="#" class="btn">Schedule a Tour</a>
        </div>
      </div>

      <div class="listing-card">
        <div class="image-gallery">
          <img src="testlisting.jpg" alt="Exterior view of the home at 1234 Elm Street" class="main-image" loading="lazy" />
        </div>
        <div class="details">
          <h2>$599,000</h2>
          <p class="location">1234 Elm Street, Springfield, IL</p>
          <p class="description">Beautiful 4-bedroom family home...</p>
          <ul class="features">
            <li>🛏️ 4 Beds</li>
            <li>🛁 3 Baths</li>
            <li>📐 2,400 sqft</li>
            <li>🌳 Large backyard</li>
            <li>🚗 2-car garage</li>
          </ul>
          <a href="#" class="btn">Schedule a Tour</a>
        </div>
      </div>
      <div class="listing-card">
        <div class="image-gallery">
          <img src="testlisting.jpg" alt="Exterior view of the home at 1234 Elm Street" class="main-image" loading="lazy" />
        </div>
        <div class="details">
          <h2>$599,000</h2>
          <p class="location">1234 Elm Street, Springfield, IL</p>
          <p class="description">Beautiful 4-bedroom family home...</p>
          <ul class="features">
            <li>🛏️ 4 Beds</li>
            <li>🛁 3 Baths</li>
            <li>📐 2,400 sqft</li>
            <li>🌳 Large backyard</li>
            <li>🚗 2-car garage</li>
          </ul>
          <a href="#" class="btn">Schedule a Tour</a>
        </div>
      </div>
    </div>
    <p class="listings-top" >Click here to view all listings
    </p>
  </section>

  <footer>
    <p>&copy; InSight Services Inc.</p>
  </footer>

  <script>
    function toggleNav() {
      var nav = document.getElementById("myLinks");
      nav.classList.toggle("show");
    }
  </script>
</body>
</html>
