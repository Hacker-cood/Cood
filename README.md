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
            /* خلفية مدمجة بين البنفسجي الغامق والأزرق */
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
        }

        /* حاوية زجاجية بحواف مضيئة */
        .container {
            background: rgba(20, 5, 35, 0.6);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border: 1px solid rgba(157, 0, 255, 0.3);
            border-radius: 25px;
            padding: 40px 20px;
            width: 100%;
            max-width: 450px;
            text-align: center;
            box-shadow: 0 0 30px rgba(157, 0, 255, 0.2), inset 0 0 20px rgba(0, 243, 255, 0.1);
            position: relative;
        }

        /* تأثير اللمعان المتحرك على الحاوية */
        .container::before {
            content: '';
            position: absolute;
            top: -2px; left: -2px; right: -2px; bottom: -2px;
            background: linear-gradient(45deg, var(--neon-purple), var(--neon-blue), var(--neon-purple));
            z-index: -1;
            border-radius: 27px;
            animation: glowingBorder 3s linear infinite;
            opacity: 0.5;
        }

        @keyframes glowingBorder {
            0% { filter: hue-rotate(0deg); }
            100% { filter: hue-rotate(360deg); }
        }

        /* اللوقو الشخصي */
        .logo-container {
            width: 140px;
            height: 140px;
            margin: 0 auto 20px;
            border-radius: 50%;
            padding: 5px;
            background: linear-gradient(45deg, var(--neon-purple), var(--neon-blue));
            box-shadow: 0 0 25px var(--neon-purple);
        }

        .logo {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid #0b001a;
        }

        h1 {
            font-size: 28px;
            font-weight: 900;
            margin-bottom: 5px;
            text-transform: uppercase;
            letter-spacing: 2px;
            text-shadow: 0 0 10px var(--neon-purple);
        }

        p.bio {
            font-size: 15px;
            color: #b3b3b3;
            margin-bottom: 25px;
            line-height: 1.6;
        }

        /* قسم البرامج (أفتر افكت ولايت موشن) */
        .tools-section {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 30px;
        }

        .tool-icon {
            width: 45px;
            height: 45px;
            border-radius: 10px;
            box-shadow: 0 0 15px rgba(255,255,255,0.2);
            animation: float 3s ease-in-out infinite;
        }

        .tool-icon:nth-child(2) {
            animation-delay: 1.5s; /* عشان يتحركون عكس بعض */
        }

        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }

        /* الأزرار */
        .links-wrapper {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .link-btn {
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            color: #fff;
            background: rgba(0, 0, 0, 0.4);
            padding: 16px 20px;
            border-radius: 15px;
            font-size: 18px;
            font-weight: 700;
            transition: all 0.3s ease;
            border: 1px solid rgba(157, 0, 255, 0.4);
            position: relative;
            overflow: hidden;
            text-shadow: 0 0 5px rgba(255,255,255,0.5);
        }

        .link-btn:hover {
            background: rgba(157, 0, 255, 0.2);
            border-color: var(--neon-blue);
            transform: scale(1.05);
            box-shadow: 0 0 20px rgba(0, 243, 255, 0.4);
        }

        /* زر المتجر الإلكتروني */
        .store-btn {
            background: linear-gradient(90deg, #4a00e0, #8e2de2);
            border: 1px solid var(--neon-blue);
            animation: pulseStore 2s infinite;
        }

        .store-btn:hover {
            background: linear-gradient(90deg, #8e2de2, #4a00e0);
        }

        @keyframes pulseStore {
            0% { box-shadow: 0 0 0 0 rgba(0, 243, 255, 0.6); }
            70% { box-shadow: 0 0 0 15px rgba(0, 243, 255, 0); }
            100% { box-shadow: 0 0 0 0 rgba(0, 243, 255, 0); }
        }

    </style>
</head>
<body>

    <div class="container">
        <div class="logo-container">
            <img src="logo.png" alt="VORTX Logo" class="logo">
        </div>

        <h1>VORTX</h1>
        <p class="bio">صانع محتوى | Edit & Motion Graphics</p>

        <div class="tools-section">
            <img src="https://upload.wikimedia.org/wikipedia/commons/4/40/Adobe_After_Effects_CC_icon.svg" alt="After Effects" class="tool-icon">
            <img src="https://play-lh.googleusercontent.com/1GZBvcX0R1EwIeN-V9sV-TzYtWn5gJzXUvB62Q0u81yW6x71XmQkZcO2T0QyR16V0g=w240-h480-rw" alt="Alight Motion" class="tool-icon" style="border-radius: 50%;">
        </div>

        <div class="links-wrapper">
            <a href="#" class="link-btn store-btn">
                🛒 المتجر الإلكتروني
            </a>

            <a href="#" class="link-btn">
                📱 تيك توك
            </a>
            
            <a href="#" class="link-btn">
                ▶️ يوتيوب
            </a>
            
            <a href="#" class="link-btn">
                📸 إنستقرام
            </a>
        </div>
    </div>

</body>
</html>
