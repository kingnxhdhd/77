<!DOCTYPE html>
<html lang="ku">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KING | Bio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            background: url('https://images.unsplash.com/photo-1477959858617-67f85cf4f1df?q=80&w=1200&auto=format&fit=crop') no-repeat center center fixed;
            background-size: cover;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            overflow-x: hidden;
            position: relative;
        }

        /* ستایلێ بارینا بەفرێ */
        .snowflake {
            position: absolute;
            top: -10px;
            color: #fff;
            font-size: 1em;
            pointer-events: none;
            animation: fall linear infinite;
        }

        @keyframes fall {
            to {
                transform: translateY(105vh) rotate(360deg);
            }
        }

        /* کانتینەرێ سەرەکی */
        .bio-container {
            width: 100%;
            max-width: 450px;
            padding: 40px 20px;
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
            z-index: 2;
        }

        /* وێنێ پڕۆفایلی یێ بازنەیی */
        .profile-img {
            width: 110px;
            height: 110px;
            border-radius: 50%;
            object-fit: cover;
            border: 2px solid rgba(255, 255, 255, 0.2);
            margin-bottom: 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);
        }

        /* ناڤێ سەرەکی KING */
        .main-name {
            font-size: 3.5rem;
            font-weight: 800;
            letter-spacing: 3px;
            text-shadow: 0 0 20px rgba(255, 255, 255, 0.9);
            margin-bottom: 5px;
        }

        /* نڤیسینا ئاینی */
        .sub-text {
            font-size: 1.4rem;
            margin-bottom: 15px;
            text-shadow: 0 2px 5px rgba(0,0,0,0.5);
        }

        /* جهـ */
        .location {
            font-size: 0.95rem;
            letter-spacing: 2px;
            margin-bottom: 30px;
            text-shadow: 0 2px 5px rgba(0,0,0,0.5);
            display: flex;
            align-items: center;
            gap: 5px;
        }

        /* لۆگۆ و لینکێن حسابان */
        .social-icons {
            display: flex;
            gap: 25px;
            margin-bottom: 40px;
        }

        .social-icons a {
            color: white;
            font-size: 2rem;
            text-decoration: none;
            transition: transform 0.3s ease, filter 0.3s ease;
            filter: drop-shadow(0 2px 5px rgba(0,0,0,0.5));
        }

        .social-icons a:hover {
            transform: scale(1.2);
        }

        /* کارتێ موزیک پلەیەری ل خوارێ */
        .music-player {
            background: rgba(0, 0, 0, 0.4);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 12px 15px;
            width: 100%;
            display: flex;
            align-items: center;
            gap: 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.4);
            margin-top: auto;
            text-decoration: none;
            color: white;
            transition: transform 0.2s ease;
        }

        .music-player:hover {
            transform: scale(1.02);
            background: rgba(0, 0, 0, 0.5);
        }

        .music-thumb {
            width: 50px;
            height: 50px;
            border-radius: 8px;
            object-fit: cover;
        }

        .music-details {
            flex-grow: 1;
            text-align: left;
        }

        .track-name {
            font-size: 1rem;
            font-weight: 600;
            margin-bottom: 4px;
        }

        .time-bar {
            font-size: 0.8rem;
            color: #ccc;
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .progress-line {
            height: 3px;
            background: rgba(255,255,255,0.2);
            flex-grow: 1;
            position: relative;
            border-radius: 2px;
        }

        .progress-current {
            position: absolute;
            left: 0;
            top: 0;
            height: 100%;
            width: 35%; /* رێژەکا دیاریکری بۆ جوانیێ */
            background: white;
            border-radius: 2px;
        }

        .music-controls {
            display: flex;
            gap: 12px;
            font-size: 1.1rem;
        }
    </style>
</head>
<body>

    <script>
        function createSnowflake() {
            const flake = document.createElement('div');
            flake.classList.add('snowflake');
            flake.innerText = '❄';
            flake.style.left = Math.random() * 100 + 'vw';
            flake.style.animationDuration = Math.random() * 3 + 2 + 's';
            flake.style.opacity = Math.random();
            flake.style.fontSize = Math.random() * 10 + 10 + 'px';
            
            document.body.appendChild(flake);
            
            setTimeout(() => {
                flake.remove();
            }, 5000);
        }
        setInterval(createSnowflake, 200);
    </script>

    <div class="bio-container">
        <img class="profile-img" src="
