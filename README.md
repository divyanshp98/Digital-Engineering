<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>My Full Website</title>
  <style>
    :root {
      --primary: #4f46e5;
      --bg-light: #ffffff;
      --bg-dark: #1f2937;
      --text-light: #f9fafb;
      --text-dark: #1a202c;
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--bg-light);
      color: var(--text-dark);
      transition: all 0.3s ease;
    }

    header {
      background-color: var(--primary);
      color: white;
      padding: 1rem 2rem;
      text-align: center;
    }

    nav {
      display: flex;
      justify-content: center;
      gap: 20px;
      background-color: #f3f4f6;
      padding: 1rem;
    }

    nav a {
      text-decoration: none;
      color: var(--text-dark);
      font-weight: 600;
    }

    .dark-mode nav {
      background-color: #111827;
    }

    .dark-mode nav a {
      color: var(--text-light);
    }

    .hero {
      background: linear-gradient(to right, #4f46e5, #6366f1);
      color: white;
      padding: 100px 20px;
      text-align: center;
    }

    .section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }

    .section h2 {
      font-size: 2.5rem;
      margin-bottom: 20px;
      text-align: center;
    }

    .section p {
      font-size: 1.1rem;
      line-height: 1.6;
      text-align: center;
    }

    .services {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      gap: 20px;
      margin-top: 40px;
    }

    .card {
      background: #f9fafb;
      padding: 20px;
      border-radius: 10px;
      flex: 1 1 300px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.05);
      text-align: center;
    }

    .dark-mode {
      background-color: var(--bg-dark);
      color: var(--text-light);
    }

    .dark-mode .card {
      background-color: #374151;
      color: var(--text-light);
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
      margin-top: 30px;
    }

    input, textarea {
      padding: 10px;
      font-size: 1rem;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    button {
      padding: 12px;
      background-color: var(--primary);
      color: white;
      border: none;
      font-size: 1rem;
      border-radius: 5px;
      cursor: pointer;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #f3f4f6;
    }

    .dark-mode footer {
      background-color: #111827;
    }

    .toggle-mode {
      position: fixed;
      top: 20px;
      right: 20px;
    }

    @media (max-width: 768px) {
      .services {
        flex-direction: column;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>My Awesome Website</h1>
  </header>

  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#services">Services</a>
    <a href="#contact">Contact</a>
  </nav>

  <div class="toggle-mode">
    <button onclick="toggleDarkMode()">🌙 Toggle Dark Mode</button>
  </div>

  <section class="hero" id="home">
    <h2>Welcome to My Website</h2>
    <p>We create modern and responsive websites with love and passion.</p>
  </section>

  <section class="section" id="about">
    <h2>About Us</h2>
    <p>We are a small team of developers and designers focused on building clean and functional digital products for everyone.</p>
  </section>

  <section class="section" id="services">
    <h2>Our Services</h2>
    <div class="services">
      <div class="card">
        <h3>Web Design</h3>
        <p>Beautiful, user-friendly, and accessible designs for modern web applications.</p>
      </div>
      <div class="card">
        <h3>Development</h3>
        <p>Clean and scalable code using modern technologies like HTML, CSS, JS, and more.</p>
      </div>
      <div class="card">
        <h3>Consulting</h3>
        <p>Need help getting started? We offer expert advice for your next big idea.</p>
      </div>
    </div>
  </section>

  <section class="section" id="contact">
    <h2>Contact Us</h2>
    <form onsubmit="return handleSubmit(event)">
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    &copy; 2025 My Awesome Website. All rights reserved.
  </footer>

  <script>
    function toggleDarkMode() {
      document.body.classList.toggle('dark-mode');
    }

    function handleSubmit(event) {
      event.preventDefault();
      alert("Thanks for your message! We'll get back to you soon.");
      event.target.reset();
      return false;
    }
  </script>
</body>
</html>
