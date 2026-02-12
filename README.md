# Fancy-Web-Page
A fancy animated web page built using pure HTML and CSS featuring gradient backgrounds, glowing text effects, and interactive button animations.

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fancy Web Page ✨</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(135deg, #6a11cb, #2575fc);
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      font-family: 'Poppins', sans-serif;
      color: white;
      overflow: hidden;
    }

    h1 {
      font-size: 3em;
      text-shadow: 0 0 20px rgba(255, 255, 255, 0.7);
      animation: glow 2s infinite alternate;
    }

    @keyframes glow {
      from { text-shadow: 0 0 10px #fff, 0 0 20px #00f6ff; }
      to { text-shadow: 0 0 20px #ff00ff, 0 0 40px #ff9900; }
    }

    p {
      font-size: 1.2em;
      margin-top: -10px;
      letter-spacing: 2px;
    }

    button {
      margin-top: 30px;
      padding: 15px 40px;
      border: none;
      border-radius: 30px;
      background: linear-gradient(45deg, #ff0066, #ffcc00);
      color: white;
      font-size: 1.1em;
      cursor: pointer;
      box-shadow: 0 0 20px rgba(255, 255, 255, 0.5);
      transition: all 0.3s ease;
    }

    button:hover {
      transform: scale(1.1);
      box-shadow: 0 0 30px #fff;
    }

    .stars {
      position: absolute;
      width: 100%;
      height: 100%;
      background: url('https://i.ibb.co/ZVh01dm/stars.png') repeat;
      animation: moveStars 60s linear infinite;
      z-index: -1;
    }

    @keyframes moveStars {
      from {background-position: 0 0;}
      to {background-position: 10000px 10000px;}
    }
  </style>
</head>
<body>
  <div class="stars"></div>
  <h1>✨ Welcome to My Fancy Page ✨</h1>
  <p>Created with pure HTML & CSS</p>
  <button onclick="alert('You clicked the magic button! 🌈')">Click Me!</button>
</body>
</html>



