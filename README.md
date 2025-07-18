<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Full Page Website</title>
  <style>
    /* Reset and Variables */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    :root {
      --primary-color: #3498db;
      --bg-color: #ffffff;
      --text-color: #333333;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--bg-color);
      color: var(--text-color);
      transition: all 0.3s ease;
    }

    header {
      background-color: var(--primary-color);
      color: white;
      padding: 1rem 2rem;
    }

    header h1 {
      margin: 0;
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      background-color: #f2f2f2;
    }

    nav a {
      margin: 0 1rem;
      text-decoration: none;
      color: var(--text-color);
      font-weight: bold;
    }

    .hero {
      background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://picsum.photos/1600/600') no-repeat center/cover;
      color: white;
      text-align: center;
      padding: 100px 20px;
    }

    .hero h2 {
      font-size: 3rem;
      margin-bottom: 1rem;
    }

    .section {
      padding: 3rem 2rem;
      max-width: 1000px;
      margin: auto;
    }

    .section h3 {
      font-size: 2rem;
      margin-bottom: 1rem;
    }

    .section p {
      font-size: 1.1rem;
      line-height: 1.6;
    }

    form {
      display: flex;
      flex-direction: column;
    }

    form input,
    form textarea {
      margin-bottom: 1rem;
      padding: 10px;
      font-size: 1rem;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    form button {
      background-color: var(--primary-color);
      color: white;
      padding: 10px;
      font-size: 1rem;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    .toggle-button {
      margin: 1rem 2rem;
      text-align: right;
    }

    .toggle-button button {
      padding: 8px 16px;
      font-size: 0.9rem;
      background-color: #444;
      color: white;
      border: none;
      border-radius: 5px;
    }

    footer {
      background-color: #f2f2f2;
      text-align: center;
      padding: 1rem;
      font-size: 0.9rem;
    }

    /* Dark Mode */
    .dark-mode {
      --bg-color: #1e1e1e;
      --text-color: #f5f5f5;
    }

    .dark-mode nav {
      background-color: #333;
    }

    .dark-mode nav a {
      color: #f5f5f5;
    }

    .dark-mode header,
    .dark-mode footer {
      background-color: #2c2c2c;
      color: white;
    }

    @media (max-width: 600px) {
      nav {
        flex-direction: column;
      }

      .hero h2 {
        font-size: 2rem;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>My Full Website</h1>
  </header>

  <div class="toggle-button">
    <button onclick="toggleDarkMode()">Toggle Dark Mode</button>
  </div>

  <nav>
    <a href="#hero">Home</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>

  <section class="hero" id="hero">
    <h2>Welcome to My Website</h2>
    <p>Explore. Learn. Connect.</p>
  </section>

  <section class="section" id="about">
    <h3>About Me</h3>
    <p>
      I'm a passionate web developer who loves building beautiful and interactive websites. This site demonstrates a full single-page design using HTML, CSS, and JavaScript.
    </p>
  </section>

  <section class="section" id="contact">
    <h3>Contact Me</h3>
    <form>
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    &copy; 2025 My Full Website. All rights reserved.
  </footer>

  <script>
    // Toggle Dark Mode
    function toggleDarkMode() {
      document.body.classList.toggle('dark-mode');
    }
  </script>
</body>
</html>

