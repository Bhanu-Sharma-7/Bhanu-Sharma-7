<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Portfolio - Bhanu Sharma</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background: linear-gradient(135deg, #f5f7fa, #c3cfe2);
      color: #333;
    }

    header {
      background: #222;
      color: white;
      padding: 20px 0;
      text-align: center;
    }

    header h1 {
      font-size: 2rem;
      letter-spacing: 1px;
    }

    nav {
      margin-top: 10px;
    }

    nav a {
      color: #fff;
      margin: 0 15px;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s ease;
    }

    nav a:hover {
      color: #ff9800;
    }

    section {
      padding: 50px 10%;
      text-align: center;
    }

    section h2 {
      font-size: 2rem;
      margin-bottom: 20px;
      position: relative;
      display: inline-block;
    }

    section h2::after {
      content: '';
      display: block;
      height: 3px;
      width: 50%;
      background: #ff9800;
      margin: 10px auto 0;
    }

    .about p {
      max-width: 700px;
      margin: auto;
      line-height: 1.6;
      font-size: 1.1rem;
    }

    .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
      margin-top: 30px;
    }

    .project-card {
      background: white;
      border-radius: 12px;
      padding: 20px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .project-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 16px rgba(0,0,0,0.15);
    }

    .contact-form {
      max-width: 600px;
      margin: auto;
      text-align: left;
    }

    .contact-form label {
      display: block;
      font-weight: 500;
      margin: 15px 0 5px;
    }

    .contact-form input, 
    .contact-form textarea {
      width: 100%;
      padding: 10px;
      border-radius: 6px;
      border: 1px solid #ccc;
      outline: none;
      font-size: 1rem;
      transition: border 0.3s ease;
    }

    .contact-form input:focus,
    .contact-form textarea:focus {
      border: 1px solid #ff9800;
    }

    .contact-form button {
      margin-top: 15px;
      padding: 10px 20px;
      background: #ff9800;
      color: white;
      border: none;
      border-radius: 6px;
      font-size: 1rem;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    .contact-form button:hover {
      background: #e68900;
    }

    footer {
      background: #222;
      color: white;
      text-align: center;
      padding: 15px 0;
      margin-top: 40px;
    }

    @media (max-width: 768px) {
      section {
        padding: 40px 5%;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Bhanu Sharma</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="about" class="about">
    <h2>About Me</h2>
    <p>
      Hi! I am Bhanu Sharma, a passionate web developer skilled in HTML, CSS, JavaScript, React, and more.
      I am pursuing B.Tech in Computer Science and Engineering, and I love creating beautiful, functional web applications.
    </p>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="projects">
      <div class="project-card">
        <h3>Frontend Portfolio</h3>
        <p>A responsive personal portfolio website made using HTML, CSS, and JavaScript.</p>
      </div>
      <div class="project-card">
        <h3>React Todo App</h3>
        <p>A simple and effective task management app built with React JS.</p>
      </div>
      <div class="project-card">
        <h3>Weather App</h3>
        <p>A live weather forecasting app using API integration and JavaScript.</p>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <form class="contact-form">
      <label for="name">Name</label>
      <input type="text" id="name" placeholder="Your name" required>

      <label for="email">Email</label>
      <input type="email" id="email" placeholder="Your email" required>

      <label for="message">Message</label>
      <textarea id="message" rows="5" placeholder="Write your message here..." required></textarea>

      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    &copy; 2025 Bhanu Sharma. All rights reserved.
  </footer>
</body>
</html>