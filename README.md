14th February 2026
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>This is only for my shiny♥</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Great+Vibes&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            /* Romantic pinkish-red gradient */
            background: linear-gradient(135deg, #ff758f 0%, #ff4d6d 50%, #c9184a 100%);
            font-family: 'Dancing Script', cursive;
            color: white;
            overflow-x: hidden;
        }

        .container {
            text-align: center;
            padding: 20px;
        }

        h1 {
            font-family: 'Great Vibes', cursive;
            font-size: 5rem;
            margin-bottom: 30px;
            text-shadow: 3px 3px 10px rgba(0, 0, 0, 0.3);
            animation: heartbeat 1.5s infinite;
        }

        /* Heartbeat animation for the text */
        @keyframes heartbeat {
            0% { transform: scale(1); }
            14% { transform: scale(1.1); }
            28% { transform: scale(1); }
            42% { transform: scale(1.1); }
            70% { transform: scale(1); }
        }

        .gallery {
            display: flex;
            gap: 20px;
            justify-content: center;
            flex-wrap: wrap;
            max-width: 1000px;
        }

        .gallery img {
            width: 250px;
            height: 350px;
            object-fit: cover;
            border-radius: 15px;
            border: 5px solid white;
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
            transition: transform 0.3s ease;
        }

        .gallery img:hover {
            transform: translateY(-10px) rotate(3deg);
        }

        /* Adding some floating hearts in the background */
        .heart {
            position: absolute;
            color: rgba(255, 255, 255, 0.4);
            font-size: 20px;
            user-select: none;
            pointer-events: none;
            animation: float 6s linear infinite;
        }

        @keyframes float {
            0% { transform: translateY(100vh) rotate(0deg); opacity: 1; }
            100% { transform: translateY(-10vh) rotate(360deg); opacity: 0; }
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Happy Valentine's Day My dear, Saini</h1>
        
        <div class="gallery">
            <img src="https://i.ibb.co/prdBzx54/JS-S-SD-png.png" alt="JS-S-SD-png" alt="Rose">
            <img src="https://i.ibb.co/tTqkKksG/S-SD.jpg" alt="Hearts">
            <img src="https://i.ibb.co/21Lq2NPm/IMG-20260212-135646.jpg" alt="Flowers">
        </div>
    </div>

    <script>
        function createHeart() {
            const heart = document.createElement('div');
            heart.classList.add('heart');
            heart.innerHTML = '❤️';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = Math.random() * 3 + 3 + 's';
            document.body.appendChild(heart);

            setTimeout(() => {
                heart.remove();
            }, 6000);
        }
        setInterval(createHeart, 500);
    </script>


</body>
</html>
