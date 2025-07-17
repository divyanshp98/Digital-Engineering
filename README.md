<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Simple Landing Page</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-white text-gray-800">
  <!-- Navbar -->
  <nav class="flex justify-between items-center px-6 py-4 shadow">
    <h1 class="text-xl font-bold">MySite</h1>
    <ul class="hidden md:flex gap-6">
      <li><a href="#" class="hover:text-blue-600">Home</a></li>
      <li><a href="#" class="hover:text-blue-600">About</a></li>
      <li><a href="#" class="hover:text-blue-600">Contact</a></li>
    </ul>
    <button class="md:hidden">☰</button>
  </nav>

  <!-- Hero Section -->
  <section class="text-center px-6 py-20 bg-blue-50">
    <h2 class="text-4xl font-bold mb-4">Welcome to MySite</h2>
    <p class="text-lg mb-6">A modern and minimal landing page built with Tailwind CSS.</p>
    <a href="#" class="bg-blue-600 text-white px-6 py-3 rounded hover:bg-blue-700">Get Started</a>
  </section>

  <!-- Features -->
  <section class="px-6 py-20">
    <div class="grid md:grid-cols-3 gap-8 text-center">
      <div>
        <h3 class="text-xl font-semibold mb-2">Fast</h3>
        <p>Lightning-fast performance for all devices.</p>
      </div>
      <div>
        <h3 class="text-xl font-semibold mb-2">Responsive</h3>
        <p>Perfectly adapts to any screen size.</p>
      </div>
      <div>
        <h3 class="text-xl font-semibold mb-2">Easy</h3>
        <p>Clean and easy-to-use layout for developers.</p>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="text-center py-6 bg-gray-100 text-sm">
    © 2025 MySite. All rights reserved.
  </footer>
</body>
</html>
