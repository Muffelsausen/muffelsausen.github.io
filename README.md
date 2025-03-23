<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muffelsausen</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        @font-face {
            font-family: 'MuffelsausenFont';
            src: url('your-font-file.woff2') format('woff2');
        }
        body {
            font-family: 'MuffelsausenFont', Arial, sans-serif;
            background-image: url('background.PNG');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 50px;
        }
        .container {
            max-width: 800px;
            margin: auto;
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }
        h1 {
            font-size: 3em;
            text-transform: uppercase;
        }
        p {
            font-size: 1.2em;
        }
        a {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 20px;
            background: #ffcc00;
            color: #333;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
        }
        a:hover {
            background: #ffaa00;
        }
        .menu-button {
            position: absolute;
            top: 20px;
            left: 20px;
            cursor: pointer;
            font-size: 30px;
            background: none;
            border: none;
            color: white;
        }
        .menu {
            position: fixed;
            top: 0;
            left: -250px;
            width: 250px;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            transition: left 0.3s ease;
            padding-top: 60px;
        }
        .menu a {
            display: block;
            color: white;
            padding: 10px;
            text-decoration: none;
            font-size: 1.5em;
        }
        .menu a:hover {
            background: rgba(255, 255, 255, 0.2);
        }
        .menu.active {
            left: 0;
        }
    </style>
</head>
<body>
    <button class="menu-button" onclick="toggleMenu()">☰</button>
    <div class="menu" id="menu">
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Events</a>
        <a href="#">Contact</a>
    </div>
    <div class="container">
        <h1>Muffelsausen</h1>
        <p>Welcome to the official Muffelsausen event page.</p>
        <p>Stay tuned for updates and details about the event!</p>
    </div>
    <script>
        function toggleMenu() {
            document.getElementById("menu").classList.toggle("active");
        }
    </script>
</body>
</html>
