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
            font-family: 'MuffelsausenFont', Fredoka, sans-serif;
            background-color: rgb(128, 0, 128);
            background-size: cover;
            background-position: center;
            margin-top: 50px; 
            color: yellow;
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
            bottom: 0;
            left: -250px;
            width: 250px;
            height: 87%;
            background: rgba(128, 0, 128, 1);
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
            background: rgba(128, 0, 128, 1);
        }
        .menu.active {
            left: 0;
        }
        .header-image {
            width: 600px;
            height: 300px;
            object-fit: cover;
            margin: 20px auto;
            display: block;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <button class="menu-button" onclick="toggleMenu()">☰</button>
    <div class="menu" id="menu">
        <a href="main.html" onclick="toggleMenu()">Home</a>
        <a href="event.html" onclick="toggleMenu()">Events</a>
        <a href="contact.html" onclick="toggleMenu()">Contact</a>
        <a href="about.html" onclick="toggleMenu()">About</a>
    </div>
    <div class="container">
        <h1>Muffelsausen</h1>
        <img src="figures/logo.PNG" alt="Muffelsausen Event" class="header-image" style="max-width: 100%; height: auto; display: block; margin: 20px auto; border-radius: 10px;">
        <p>Welcome to the official Muffelsausen event page.</p>
        <p>Bla Bla Bla Bla Bla Bla Bla Bla Bla Bla Bla Bla!</p>
    </div>
    <script>
        function toggleMenu() {
            var menu = document.getElementById("menu");
            if (menu.style.left === "0px") {
                menu.style.left = "-250px";
            } else {
                menu.style.left = "0px";
            }
        }
    </script>
</body>
</html>
