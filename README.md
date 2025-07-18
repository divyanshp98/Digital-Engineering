
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Simple Website</title>
  <style>
    /* CSS Styles */
    :root {
      --bg-color: #ffffff;
      --text-color: #333333;
      --primary-color: #007bff;
    }

    body {
      font-family: Arial, sans-serif;
      background-color: var(--bg-color);
      color: var(--text-color);
      margin: 0;
      padding: 0;
      transition: background-color 0.3s, color 0.3s;
    }

    header {
      background-color: var(--primary-color);
      color: white;
      padding: 1rem;
      text-align: center;
    }

    nav {
      background: #f4f4f4;
      padding: 0.5rem;
      text-align: center;
    }

    nav a {
      margin: 0 15px;
      text-decoration: none;
      color: var(--text-color);
      font-weight: bold;
    }

    .container {
      padding: 2rem;
      text-align: center;
    }

    button {
      padding: 10px 20px;
      font-size: 1rem;
      cursor: pointer;
      background-color: var(--primary-color);
      color: white;
      border: none;
      border-radius: 5px;
    }

    footer {
      background-color: #eee;
      padding: 1rem;
      text-align: center;
      font-size: 0.9rem;
    }

    /* Dark mode styles */
    .dark-mode {
      --bg-color: #1e1e1e;
      --text-color: #f5f5f5;
    }
  </style>
</head>
<body>

  <header>
    <h1>Welcome to My Website</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </nav>

  <div class="container">
    <h2>Hello, World!</h2>
    <p>This is a simple, interactive website using HTML, CSS, and JavaScript.</p>
    <button onclick="toggleDarkMode()">Toggle Dark Mode</button>
  </div>

  <footer>
    &copy; 2025 My Website. All rights reserved.
  </footer>

  <script>
    // JavaScript Function
    function toggleDarkMode() {
      document.body.classList.toggle('dark-mode');
    }
  </script>
</body>
</html>
