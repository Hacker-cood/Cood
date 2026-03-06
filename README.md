<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VORTX | روابطي</title>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        :root {
            --neon-purple: #9d00ff;
            --neon-blue: #00f3ff;
            --bg-dark: #0b001a;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Tajawal', sans-serif;
        }

        body {
            background-color: var(--bg-dark);
            background-image: 
                radial-gradient(circle at 15% 50%, rgba(157, 0, 255, 0.15), transparent 25%),
                radial-gradient(circle at 85% 30%, rgba(0, 243, 255, 0.15), transparent 25%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            color: #fff;
            overflow-x: hidden;
            position: relative;
        }

        /* --- شعارات الخلفية المائلة --- */
        .bg-icon {
            position: absolute;
            z-index: 0;
            opacity: 0.6;
            width: 150px;
            border-radius: 20px;
        }

        .bg-ae {
            top: 10%;
            right: 5%;
            filter: drop-shadow(0 0 30px var(--neon-purple));
            animation: floatAE 6s ease-in-out infinite;
        }

        .bg-am {
            bottom: 15%;
            left: 5%;
            width: 130px;
            border-radius: 50%;
            filter: drop-shadow(0 0 30px var(--neon-blue));
            animation: floatAM 7s ease-in-out infinite;
        }

        @keyframes floatAE {
            0%, 100% { transform: translateY(0) rotate(15deg); }
            50% { transform: translateY(-25px) rotate(25deg); }
        }

        @keyframes floatAM {
            0%, 100% { transform: translateY(0) rotate(-20deg); }
            50% { transform: translateY(-20px) rotate(-30deg); }
        }

        /* --- الحاوية الرئيسية --- */
        .container {
            background: rgba(20, 5, 35, 0.65);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border: 1px solid rgba(157, 0, 255, 0.3);
            border-radius: 25px;
            padding: 50px 30px;
            width: 100%;
            max-width: 600px;
            text-align: center;
            box-shadow: 0 0 40px rgba(157, 0, 255, 0.15), inset 0 0 20px rgba(0, 243, 255, 0.05);
            position: relative;
            z-index: 1;
        }

        .container::before {
            content: '';
            position: absolute;
            top: -2px; left: -2px; right: -2px; bottom: -2px;
            background: linear-gradient(45deg, var(--neon-purple), var(--neon-blue), var(--neon-purple));
            z-index: -1;
            border-radius: 27px;
            animation: glowingBorder 4s linear infinite;
            opacity: 0.5;
        }

        @keyframes glowingBorder {
            0% { filter: hue-rotate(0deg); }
            100% { filter: hue-rotate(360deg); }
        }

        /* --- اللوقو الشخصي --- */
        .logo-container {
            width: 150px;
            height: 150px;
            margin: 0 auto 20px;
            border-radius: 50%;
            padding: 5px;
            background: linear-gradient(45deg, var(--neon-purple), var(--neon-blue));
            box-shadow: 0 0 30px var(--neon-purple);
        }

        .logo {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid #0b001a;
        }

        h1 {
            font-size: 32px;
            font-weight: 900;
            margin-bottom: 5px;
            text-transform: uppercase;
            letter-spacing: 2px;
            text-shadow: 0 0 15px var(--neon-purple);
        }

        p.bio {
            font-size: 16px;
            color: #b3b3b3;
            margin-bottom: 35px;
            line-height: 1.6;
        }

        /* --- الأزرار --- */
        .links-wrapper {
            display: flex;
            flex-direction: column;
            gap: 18px;
        }

        .link-btn {
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            color: #fff;
            background: rgba(0, 0, 0, 0.5);
            padding: 18px 20px;
            border-radius: 15px;
            font-size: 18px;
            font-weight: 700;
            transition: all 0.3s ease;
            border: 1px solid rgba(157, 0, 255, 0.3);
            position: relative;
            overflow: hidden;
            text-shadow: 0 0 5px rgba(255,255,255,0.3);
        }

        .link-btn:hover {
            background: rgba(157, 0, 255, 0.25);
            border-color: var(--neon-blue);
            transform: scale(1.03);
            box-shadow: 0 0 25px rgba(0, 243, 255, 0.3);
        }

        /* --- زر المتجر --- */
        .store-btn {
            background: linear-gradient(90deg, #4a00e0, #8e2de2);
            border: 1px solid var(--neon-blue);
            animation: pulseStore 2s infinite;
        }

        .store-btn:hover {
            background: linear-gradient(90deg, #8e2de2, #4a00e0);
        }

        @keyframes pulseStore {
            0% { box-shadow: 0 0 0 0 rgba(0, 243, 255, 0.5); }
            70% { box-shadow: 0 0 0 15px rgba(0, 243, 255, 0); }
            100% { box-shadow: 0 0 0 0 rgba(0, 243, 255, 0); }
        }
    </style>
</head>
<body>

    <img src="ae.png" alt="After Effects" class="bg-icon bg-ae">
    <img src="am.png" alt="Alight Motion" class="bg-icon bg-am">

    <div class="container">
        <div class="logo-container">
            <img src="lg.png" alt="VORTX Logo" class="logo">
        </div>

        <h1>VORTX</h1>
        <p class="bio">صانع محتوى | Edit & Motion Graphics</p>

        <div class="links-wrapper">
            <a href="#" class="link-btn store-btn">🛒 المتجر الإلكتروني</a>
            <a href="#" class="link-btn">📱 تيك توك</a>
            <a href="#" class="link-btn">▶️ يوتيوب</a>
            <a href="#" class="link-btn">📸 إنستقرام</a>
        </div>
    </div>

</body>
</html>
