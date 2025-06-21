# Grand-State
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Grand State</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #121212;
      color: white;
      text-align: center;
    }

    header {
      padding: 20px;
      background: #1f1f1f;
    }

    h1 {
      font-size: 3em;
      color: #00ffff;
    }

    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-size: 1.2em;
    }

    .main {
      padding: 50px 20px;
    }

    .btn {
      background: #00ffff;
      color: #000;
      padding: 15px 30px;
      margin: 10px;
      border: none;
      border-radius: 10px;
      font-size: 1em;
      cursor: pointer;
      transition: background 0.3s;
    }

    .btn:hover {
      background: #00dddd;
    }

    footer {
      margin-top: 50px;
      padding: 20px;
      background: #1f1f1f;
      font-size: 0.9em;
    }
  </style>
</head>
<body>

  <header>
    <h1>Grand State </h1>
    <nav>
      <a href="#">Home</a>
      <a href="#features">Features</a>
      <a href="#download">Download</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <div class="main">
    <h2 id="welcome-msg"></h2>
    <p>Welcome to the official site of Grand State</p>

    <div>
      <button class="btn" onclick="alert('Download coming soon!')">Download APK</button>
      <button class="btn" onclick="window.open('https://discord.gg/QQXrWyWBJv')">Join Discord</button>
    </div>
  </div>

  <footer>
    &copy; 2025 Grand State. All rights reserved.
  </footer>

  <script>
    // Simple welcome message animation
    const welcomeText = "Grand State";
    let i = 0;

    function typeMessage() {
      if (i < welcomeText.length) {
        document.getElementById("welcome-msg").innerHTML += welcomeText.charAt(i);
        i++;
        setTimeout(typeMessage, 70); // typing speed
      }
    }

    window.onload = typeMessage;
  </script>

</body>
</html>
