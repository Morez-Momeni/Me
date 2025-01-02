<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub README</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background: linear-gradient(120deg, #0f2027, #203a43, #2c5364);
            color: #ffffff;
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            overflow: hidden;
        }

        .container {
            text-align: center;
            position: relative;
            animation: fadeIn 2s ease-in-out;
        }

        h1 {
            font-size: 3rem;
            margin: 0;
            background: linear-gradient(to right, #00c6ff, #0072ff);
            -webkit-background-clip: text;
            color: transparent;
            animation: slideIn 2s ease-in-out;
        }

        p {
            margin: 10px 0;
            font-size: 1.2rem;
            color: rgba(255, 255, 255, 0.8);
            animation: fadeIn 3s ease-in-out;
        }

        .stars {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: radial-gradient(circle, #ffffff 2px, transparent 2px);
            background-size: 50px 50px;
            animation: starMovement 30s linear infinite;
        }

        .button {
            margin-top: 20px;
            display: inline-block;
            padding: 10px 20px;
            background: #00c6ff;
            border: none;
            border-radius: 20px;
            color: white;
            font-size: 1.2rem;
            text-decoration: none;
            animation: pulse 2s infinite;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        @keyframes slideIn {
            from {
                transform: translateY(-50px);
            }
            to {
                transform: translateY(0);
            }
        }

        @keyframes starMovement {
            from {
                background-position: 0 0;
            }
            to {
                background-position: 1000px 1000px;
            }
        }

        @keyframes pulse {
            0%, 100% {
                box-shadow: 0 0 20px rgba(0, 198, 255, 0.5);
            }
            50% {
                box-shadow: 0 0 40px rgba(0, 198, 255, 1);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Welcome to My GitHub!</h1>
        <p>Explore my Python projects, ideas, and contributions.</p>
        <a href="#" class="button">Check My Projects</a>
    </div>
    <div class="stars"></div>
</body>
</html>
