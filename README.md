
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Barbie</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f58ad1;
            color: #252525;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #fa578d;
            color: white;
            text-align: center;
            padding: 20px 0;
        }
        h1 {
            margin: 0;
        }
        .content {
            padding: 20px;
            max-width: 800px;
            margin: 20px auto;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .image {
            width: 100%;
            height: auto;
            border-radius: 8px;
            display: none; /* Initially hidden */
        }
        .footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            position: absolute;
            bottom: 0;
            width: 100%;
        }
        .btn {
            display: block;
            margin: 10px 0;
            padding: 10px 15px;
            background-color: #fa578d;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .btn:hover {
            background-color: #e34779;
        }
    </style>
</head>
<body>

    <header>
        <h1>I'm a Barbie Girl, in a Barbie World</h1>
    </header>

    <div class="content">
        <button class="btn" onclick="toggleImage()">Show Image</button>
        <img src="Barbie.jpg" alt="Barbie" class="image" id="barbieImage">
        <h2>About Barbie</h2>
        <p>Barbie is a fashion doll created by American businesswoman Ruth Handler, manufactured by American toy and entertainment company Mattel and introduced on March 9, 1959. The toy was based on the German Bild Lilli doll which Handler had purchased while in Europe. The figurehead of an eponymous brand that includes a range of fashion dolls and accessories, Barbie has been an important part of the toy fashion doll market for over six decades. Mattel has sold over a billion Barbie dolls, making it the company's largest and most profitable line.[1] The brand has expanded into a multimedia franchise since 1984, including video games, animated films, television/web series, and a live-action film.</p>
    </div>

    <div class="footer">
        <p>&copy; Barbie World</p>
    </div>

    <script>
        function toggleImage() {
            const image = document.getElementById("barbieImage");
            const button = document.querySelector(".btn");
            if (image.style.display === "none" || image.style.display === "") {
                image.style.display = "block";
                button.textContent = "Hide Image";
            } else {
                image.style.display = "none";
                button.textContent = "Show Image";
            }
        }
    </script>

</body>
</html>
