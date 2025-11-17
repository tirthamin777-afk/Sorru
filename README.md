<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sorry Website</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            overflow: hidden;
            font-family: 'Dancing Script', cursive;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            position: relative;
        }

        /* Sorry theme background with subtle animation */
        body::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            animation: fadeInOut 5s ease-in-out infinite;
            z-index: -1;
        }

        @keyframes fadeInOut {
            0%, 100% { opacity: 0.3; }
            50% { opacity: 0.6; }
        }

        /* Center text */
        .center-text {
            font-size: 4em;
            text-align: center;
            margin-bottom: 50px;
            text-shadow: 0 0 10px #fff, 0 0 20px #fff;
        }

        /* Bottom text */
        .bottom-text {
            position: absolute;
            bottom: 20px;
            font-size: 1.5em;
            text-align: center;
        }

        /* Falling sorry words */
        .falling-sorry {
            position: absolute;
            top: -50px;
            font-size: 1.2em;
            color: rgba(255, 255, 255, 0.7);
            animation: fall 5s linear infinite;
            pointer-events: none;
        }

        @keyframes fall {
            0% { transform: translateY(-100px) rotate(0deg); opacity: 1; }
            100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
        }

        /* Generate multiple falling sorry elements */
        .falling-sorry:nth-child(1) { left: 10%; animation-delay: 0s; }
        .falling-sorry:nth-child(2) { left: 20%; animation-delay: 1s; }
        .falling-sorry:nth-child(3) { left: 30%; animation-delay: 2s; }
        .falling-sorry:nth-child(4) { left: 40%; animation-delay: 3s; }
        .falling-sorry:nth-child(5) { left: 50%; animation-delay: 4s; }
        .falling-sorry:nth-child(6) { left: 60%; animation-delay: 0.5s; }
        .falling-sorry:nth-child(7) { left: 70%; animation-delay: 1.5s; }
        .falling-sorry:nth-child(8) { left: 80%; animation-delay: 2.5s; }
        .falling-sorry:nth-child(9) { left: 90%; animation-delay: 3.5s; }
        .falling-sorry:nth-child(10) { left: 15%; animation-delay: 4.5s; }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            .center-text {
                font-size: 2.5em;
            }
            .bottom-text {
                font-size: 1.2em;
            }
        }
    </style>
</head>
<body>
    <!-- Falling sorry words -->
    <div class="falling-sorry">sorry</div>
    <div class="falling-sorry">sorry</div>
    <div class="falling-sorry">sorry</div>
    <div class="falling-sorry">sorry</div>
    <div class="falling-sorry">sorry</div>
    <div class="falling-sorry">sorry</div>
    <div class="falling-sorry">sorry</div>
    <div class="falling-sorry">sorry</div>
    <div class="falling-sorry">sorry</div>
    <div class="falling-sorry">sorry</div>

    <!-- Center text -->
    <div class="center-text">sorry Harleen and Amaira</div>

    <!-- Bottom text -->
    <div class="bottom-text">ab ham tumko sari chizo me add karnge</div>
</body>
</html>

