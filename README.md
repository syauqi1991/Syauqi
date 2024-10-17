# Syauqi

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Romantic Congratulations</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background: linear-gradient(to bottom right, #ff9a9e, #fad0c4, #fad0c4, #ff9a9e);
            font-family: 'Arial', sans-serif;
            overflow: hidden;
            animation: fadeIn 2s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .container {
            text-align: center;
            background: rgba(255, 255, 255, 0.8);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            animation: slideDown 2s ease-in-out;
        }

        @keyframes slideDown {
            from { transform: translateY(-50px); }
            to { transform: translateY(0); }
        }

        h1 {
            font-size: 2.5em;
            color: #ff4081;
        }

        p {
            font-size: 1.2em;
            color: #333;
        }

        .flower {
            position: fixed;
            top: -10%;
            background-size: contain;
            background-repeat: no-repeat;
            z-index: 9999;
            animation: fall linear infinite;
        }

        @keyframes fall {
            0% {
                transform: translateY(0);
            }
            100% {
                transform: translateY(100vh);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Halo Cantik🥰</h1>
        <p>Agar hubungan tidak putus,bolehkah minta pap 100?</p>
    </div>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const flowerCount = 20;
            const body = document.body;

            for (let i = 0; i < flowerCount; i++) {
                let flower = document.createElement('div');
                flower.className = 'flower';
                flower.style.left = `${Math.random() * 100}vw`;
                flower.style.animationDuration = `${Math.random() * 3 + 2}s`;
                flower.style.animationDelay = `${Math.random() * 5}s`;
                flower.style.width = `${Math.random() * 20 + 10}px`;
                flower.style.height = flower.style.width;
                flower.style.backgroundImage = "url('flower.png')";
                body.appendChild(flower);
            }
        });
    </script>
</body>
</html>
