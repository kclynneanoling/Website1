<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfolio Page</title>
  <style>
    /* General Styles */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f9f9f9;
      scroll-behavior: smooth; /* Enables smooth scrolling */
    }

    /* Header Section */
    .header {
      text-align: center;
      padding: 50px 20px;
      background-color: #afaaad;
    }

    .header h1 {
      font-size: 28px;
      color: #333;
      margin-bottom: 20px;
    }

    .discover-btn {
      background-color: #007BFF;
      color: white;
      border: none;
      padding: 10px 20px;
      font-size: 16px;
      border-radius: 5px;
      cursor: pointer;
    }

    .discover-btn:hover {
      background-color: #0056b3;
    }

    /* Navigation Bar */
    .navbar {
      background-color: #333;
      padding: 10px 0;
    }

    .navbar ul {
      list-style: none;
      display: flex;
      justify-content: center;
      margin: 0;
      padding: 0;
    }

    .navbar ul li {
      margin: 0 15px;
    }

    .navbar ul li a {
      color: white;
      text-decoration: none;
      font-size: 16px;
    }

    .navbar ul li a:hover {
      text-decoration: underline;
    }

    /* Section Styles */
    .about-section, .favorites-section, .contact-section {
      text-align: center;
      padding: 40px 20px;
    }

    /* Apply Bold, Italic, and Blue Color to Section Headings */
    .about-section h2, .favorites-section h2, .contact-section h2 {
      font-size: 24px;
      margin-bottom: 20px;
      color: blue;
      font-weight: bold;
      font-style: italic;
    }

    /* Favorites Section */
    .favorites {
      display: flex;
      justify-content: center;
      gap: 20px;
    }

    .favorite-item {
      background-color: #e0e0e0;
      width: 120px;
      height: 120px;
      border-radius: 10px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 10px;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .favorite-item:hover {
      transform: scale(1.2); /* Zoom-in effect */
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2); /* Add shadow for emphasis */
    }

    .favorite-item p {
      margin-top: 10px;
      font-size: 14px;
      color: #333;
      font-weight: bold; /* Make the text bold */
    }

    /* Back to Home Button */
    .back-button {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #007BFF;
      color: white;
      text-decoration: none;
      font-size: 14px;
      padding: 10px 20px;
      border-radius: 5px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      cursor: pointer;
      display: none; /* Hidden initially */
      text-align: center;
    }

    .back-button:hover {
      background-color: #0056b3;
    }

    /* Footer */
    .footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 10px 0;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <div class="header">
    <h1>Hello, I'm Kc Lynne</h1>
    <a href="#about"><button class="discover-btn">Discover More</button></a>
  </div>

  <nav class="navbar">
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#favorites">My Favorites</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <section id="about" class="about-section">
    <h2>About Me</h2>
    <p>Hi, I'm Kc Lynne, a passionate individual with a love for creativity and new experiences.<br> Whether it's exploring different hobbies, learning new skills,<br> or connecting with others, I'm always excited to grow<br> and discover more about the world around me.</p>
  </section>

  <section id="favorites" class="favorites-section">
    <h2>My Favorites</h2>
    <div class="favorites">
      <div class="favorite-item">
        <p>Playing Games</p>
        <p>Mobile Legends</p>
        <p>CodM</p>
        <p>Block Blast</p>
      </div>
      <div class="favorite-item">
        <p>Cooking</p>
        <p>Viand</p>
        <p>Snack</p>
      </div>
      <div class="favorite-item">
        <p>Watching</p>
        <p>Anime</p>
        <p>Kdrama</p>
      </div>
    </div>
  </section>

  <section id="contact" class="contact-section">
    <h2>Contact Me</h2>
    <p>Facebook: Kc Lynne Anoling</p>
    <p>09457200898</p>
    <p>Email: kclynneanoling@gmail.com</p>
  </section>

  <footer class="footer">
    <p>@2024 All Rights Reserved</p>
  </footer>

  <!-- Back to Home Button -->
  <a href="lab5.html" class="back-button">Back to Home</a>

  <script>
    // Show Back to Home button when scrolling down
    window.onscroll = function() {
      const backButton = document.querySelector('.back-button');
      if (document.body.scrollTop > 100 || document.documentElement.scrollTop > 100) {
        backButton.style.display = 'block';
      } else {
        backButton.style.display = 'none';
      }
    };
  </script>
</body>
</html>
