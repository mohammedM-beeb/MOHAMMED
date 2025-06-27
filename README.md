<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>My Portfolio</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>Mohammed Alquriniy</h1>
    <p>Web Developer | Student | Creator</p>
  </header>

  <nav>
    <ul>
      <li><a href="#about">About Me</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <main>
    <section id="about">
      <h2>About Me</h2>
      <p>I'm learning web development and this is my personal portfolio website built using HTML, CSS, and JavaScript.</p>
      <img src="profile.jpg" alt="A professional photo of Mohammed Alquriniy" width="200" />
    </section>

    <section id="projects">
      <h2>Projects</h2>
      <ul>
        <li>Simple Calculator App</li>
        <li>Weather Dashboard</li>
        <li>To-Do List Web App</li>
      </ul>
    </section>

    <section id="contact">
      <h2>Contact</h2>
      <form id="contact-form">
        <input type="text" placeholder="Your Name" required />
        <input type="email" placeholder="Your Email" required />
        <textarea placeholder="Your Message" required></textarea>
        <button type="submit">Send</button>
      </form>
      <p id="form-message"></p>
    </section>
  </main>

  <footer>
    <p>© 2025 Mohammed Alquriniy</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>






















* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  padding: 20px;
  background-color: #f4f4f4;
}

header, footer {
  text-align: center;
  padding: 20px;
  background: #333;
  color: #fff;
}

nav ul {
  display: flex;
  justify-content: center;
  list-style: none;
  background: #444;
  padding: 10px;
}

nav ul li {
  margin: 0 10px;
}

nav ul li a {
  color: #fff;
  text-decoration: none;
}

main {
  margin-top: 20px;
}

section {
  margin-bottom: 40px;
}

form input, form textarea {
  display: block;
  width: 100%;
  margin-bottom: 10px;
  padding: 10px;
}

button {
  background: #333;
  color: white;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
}

@media (max-width: 600px) {
  nav ul {
    flex-direction: column;
    align-items: center;
  }

  img {
    width: 100%;
    height: auto;
  }
}






















document.getElementById("contact-form").addEventListener("submit", function (e) {
  e.preventDefault();
  document.getElementById("form-message").textContent = "Thanks for your message!";
});

  
