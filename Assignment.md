Assignment 7.4 — Modern Landing Page Header,Assignment-7.4.md — Complete Code
Save the following code in an index.html file and open it in your browser.


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Modern Landing Page</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      background: #f8faff;
      color: #1e293b;
      line-height: 1.6;
    }

    /* Header */
    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 8%;
      background: #ffffff;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
    }

    .logo {
      font-size: 26px;
      font-weight: bold;
      color: #4f46e5;
    }

    nav {
      display: flex;
      align-items: center;
      gap: 28px;
    }

    nav a {
      text-decoration: none;
      color: #334155;
      font-weight: 500;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #4f46e5;
    }

    .btn {
      display: inline-block;
      padding: 12px 24px;
      background: #4f46e5;
      color: white;
      text-decoration: none;
      border-radius: 8px;
      font-weight: bold;
      transition: background 0.3s;
    }

    .btn:hover {
      background: #3730a3;
    }

    /* Hero Section */
    .hero {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 50px;
      padding: 80px 8%;
      min-height: 80vh;
    }

    .hero-content {
      flex: 1;
      max-width: 550px;
    }

    .hero-content h1 {
      font-size: clamp(36px, 5vw, 56px);
      line-height: 1.15;
      margin-bottom: 24px;
      color: #0f172a;
    }

    .hero-content h1 span {
      color: #4f46e5;
    }

    .hero-content p {
      font-size: 18px;
      color: #64748b;
      margin-bottom: 30px;
    }

    .hero-image {
      flex: 1;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .hero-image img {
      width: 100%;
      max-width: 480px;
      height: auto;
      border-radius: 20px;
      box-shadow: 0 20px 50px rgba(79, 70, 229, 0.12);
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 22px;
      background: #0f172a;
      color: #ffffff;
    }

    /* Responsive Design */
    @media (max-width: 768px) {
      header {
        flex-direction: column;
        gap: 20px;
        padding: 20px 5%;
      }

      nav {
        flex-wrap: wrap;
        justify-content: center;
        gap: 16px;
      }

      .hero {
        flex-direction: column;
        text-align: center;
        padding: 55px 6%;
        gap: 40px;
      }

      .hero-content {
        max-width: 100%;
      }

      .hero-content p {
        font-size: 16px;
      }

      .hero-image img {
        max-width: 100%;
      }
    }

    @media (max-width: 420px) {
      nav {
        gap: 12px;
      }

      nav a {
        font-size: 14px;
      }

      .hero-content h1 {
        font-size: 34px;
      }

      .btn {
        padding: 10px 18px;
      }
    }
  </style>
</head>

<body>

  <!-- Header -->
  <header>
    <div class="logo">Nova.</div>

    <nav aria-label="Main navigation">
      <a href="#home">Home</a>
      <a href="#features">Features</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
      <a href="#get-started" class="btn">Get Started</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <main>
    <section class="hero" id="home">

      <div class="hero-content">
        <h1>
          Build Your Future
          <span>With Confidence</span>
        </h1>

        <p>
          Discover smarter digital solutions designed to help
          you grow, create, and achieve more. Start your journey
          today with our modern platform.
        </p>

        <a href="#get-started" class="btn" id="get-started">
          Get Started →
        </a>
      </div>

      <div class="hero-image">
        <img
          src="https://images.unsplash.com/photo-1497366754035-f200968a6e72?auto=format&fit=crop&w=1000&q=80"
          alt="Modern workspace with desks and computers"
        >
      </div>

    </section>
  </main>

  <!-- Footer -->
  <footer id="contact">
    <p>&copy; 2026 Nova. All rights reserved.</p>
  </footer>

</body>
</html>
Assignment requirements covered
Header: Logo, navigation links, and CTA button.

Hero section: Main heading, paragraph, and button.

Image: Modern workspace illustration/photo.

Flexbox: Places text and image side by side.

Alignment: Uses align-items: center and justify-content: space-between.

Footer: Dark background with copyright text.

Responsive design: Media queries adjust the layout for mobile screens.