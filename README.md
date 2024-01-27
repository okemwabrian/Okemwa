<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Adaptrap - Official Website</title>
  <style>
    /* General styling */
    body {
      font-size: 16px;
      margin: 0;
      background-image: url("path/to/background-image.jpg"); /* Add your background image */
      background-size: cover;
    }

    header, main, footer {
      padding: 1rem;
    }

    img {
      max-width: 100%;
      height: auto;
    }

    /* Search bar styling */
    input[type="search"] {
      background-color: #f0f0f0;
      border: 1px solid #ccc;
      padding: 5px;
      border-radius: 5px;
    }

    /* Login form styling */
    #login-form {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    #login-form input[type="text"],
    #login-form input[type="password"] {
      margin-bottom: 10px;
    }

    /* ... other styles (responsiveness, video, etc.) ... */
  </style>
  <script>
    // Basic login functionality (for demonstration, not secure)
    function handleLogin() {
      const username = document.querySelector("input[type='text']").value;
      const password = document.querySelector("input[type='password']").value;

      if (username === "MOKUA" && password === "1234") {
        alert("Login successful!");
        document.getElementById("login-form").style.display = "none";
        document.getElementById("main").style.display = "block";
      } else {
        alert("Invalid username or password.");
      }
    }
  </script>
</head>
<body>
  <header>
    <h1>Welcome to Adaptrap's Official Website</h1>
    <form action="/search" method="get">
      <input type="search" placeholder="Search for commodities..." style="background-color: #f0f0f0;">
      <button type="submit"><i class="fa fa-search"></i></button>
    </form>

    <div id="login-form" style="display: block;">
      <h2>Login</h2>
      <input type="text" placeholder="Username">
      <input type="password" placeholder="Password">
      <button type="submit" onclick="handleLogin()">Log In</button>
      <a href="#">Forgot Password?</a>
    </div>
  </header>
  <main id="main" style="display: none;">
    <p>This is our official online presence. Explore our products, services, and connect with us.</p>

    <img width="100" height="200" src="mokua jr.jpeg" alt="Advert 1" loading="lazy">
    <img width="100" height="200" src="stamp.jpeg" alt="Advert 2" loading="lazy">

    <video width="50%" height="200" controls>
      <source src="kevins.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </main>
  <footer>
    <p>Contact us:</p>
    <a href="tel:0701024127"><i class="fa fa-phone"></i> 0701024127</a>
    <a href="mailto:kevinmokua6@gmail.com"><i class="fa fa-envelope"></i> Email</a>
    <a href="https://wa.me/0701024127"><i class="fa fa-whatsapp"></i> WhatsApp</a>
    <p>&copy;