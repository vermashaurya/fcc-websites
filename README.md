<html>
<head>
    <style>
      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: Inter, system-ui, sans-serif;
      }

      :root {
        --bg: #0a0a0a;
        --card: #111111;
        --text: #e5e5e5;
        --muted: #888;
        --accent: #4f9cff;
      }

      .light {
        --bg: #f5f5f5;
        --card: #ffffff;
        --text: #111;
        --muted: #555;
      }

      body {
        background: var(--bg);
        color: var(--text);
        padding: 20px;
      }

      .navbar {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 30px;
      }

      .logo {
        font-weight: bold;
        font-size: 1.2rem;
      }

      .nav-right {
        display: flex;
        gap: 20px;
        align-items: center;
      }

      .nav-right a {
        text-decoration: none;
        color: var(--text);
        font-size: 0.9rem;
      }

      #themeToggle {
        border: none;
        background: var(--card);
        color: var(--text);
        padding: 6px 10px;
        cursor: pointer;
        border-radius: 6px;
      }

      .hero {
        text-align: center;
        margin-bottom: 30px;
      }

      .hero h1 {
        font-size: 2rem;
        margin-bottom: 8px;
      }

      .hero p {
        color: var(--muted);
      }

      .container {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 16px;
        max-width: 900px;
        margin: auto;
      }

      .card {
        background: var(--card);
        padding: 16px;
        border-radius: 10px;
        transition: 0.25s ease;
        border: 1px solid #1f1f1f;
      }

      .card:hover {
        transform: translateY(-4px);
        border-color: var(--accent);
      }

      .card h3 {
        margin-bottom: 6px;
        font-size: 1rem;
      }

      .card p {
        font-size: 0.8rem;
        color: var(--muted);
        margin-bottom: 10px;
      }

      .card a {
        text-decoration: none;
        font-size: 0.85rem;
        color: var(--accent);
      }

      .highlight {
        border-color: var(--accent);
      }

      footer {
        margin-top: 40px;
        text-align: center;
        font-size: 0.8rem;
        color: var(--muted);
      }

      footer a {
        display: block;
        margin-top: 8px;
        color: var(--accent);
        text-decoration: none;
      }

      @media (max-width: 600px) {
        .container {
          grid-template-columns: 1fr;
        }
      }
    </style>

    <script>
      document.addEventListener("DOMContentLoaded", function () {
        const toggle = document.getElementById("themeToggle");
        toggle.addEventListener("click", () => {
          document.body.classList.toggle("light");
          toggle.textContent =
            document.body.classList.contains("light") ? "🌙" : "☀️";
        });
      });
    </script>
  </head>

<body>

<nav class="navbar">
  <div class="logo">fcc-websites</div>
  <div class="nav-right">
    <a href="https://vermashaurya.github.io/fcc-websites/" target="_blank">Open Catalogue</a>
    <button id="themeToggle">☀️</button>
  </div>
</nav>

<section class="hero">
  <h1>freeCodeCamp Web Projects</h1>
  <p>A collection of frontend experiments and learning work</p>
</section>

<div class="container">

  <div class="card">
    <h3>Cat Photo App</h3>
    <p>Basic HTML structure with forms</p>
    <a href="https://vermashaurya.github.io/fcc-websites/CatPhotoApp/catphotoapp.html">View Project</a>
  </div>

  <div class="card">
    <h3>Cafe Menu</h3>
    <p>Styled layout using CSS</p>
    <a href="https://vermashaurya.github.io/fcc-websites/CafeMenu/cafemenu.html">View Project</a>
  </div>

  <div class="card">
    <h3>Color Markers</h3>
    <p>CSS experimentation with colors</p>
    <a href="https://vermashaurya.github.io/fcc-websites/ColorMarker/colormarker.html">View Project</a>
  </div>

  <div class="card highlight">
    <h3>Registration Form</h3>
    <p>Forms, inputs & SEO practices</p>
    <a href="https://vermashaurya.github.io/fcc-websites/RegistrationForm/registrationform.html">View Project</a>
  </div>

  <div class="card">
    <h3>Rothko Painting</h3>
    <p>CSS art experiment</p>
    <a href="https://vermashaurya.github.io/fcc-websites/RothkoPainting/rothkopainting.html">View Project</a>
  </div>

  <div class="card">
    <h3>Photo Gallery</h3>
    <p>Flexbox layout exploration</p>
    <a href="https://vermashaurya.github.io/fcc-websites/PhotoGallery/photogallery.html">View Project</a>
  </div>

  <div class="card">
    <h3>Nutrition Label</h3>
    <p>Structured layout using divs</p>
    <a href="https://vermashaurya.github.io/fcc-websites/NutritionLabel/nutritionlabel.html">View Project</a>
  </div>

  <div class="card">
    <h3>Accessibility Quiz</h3>
    <p>Accessibility best practices</p>
    <a href="https://vermashaurya.github.io/fcc-websites/AccessibilityQuiz/accessibilityquiz.html">View Project</a>
  </div>

</div>

<footer>
  <p>© 2026 Shaurya Verma</p>
  <a href="https://vermashaurya.github.io/fcc-websites/" target="_blank">
    View Full Catalogue
  </a>
</footer>

</body>
</html>