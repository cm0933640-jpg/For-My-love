<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meri JAANEMANN ke liye❤️</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            font-family: 'Arial', sans-serif;
            /* BG PHOTO:  */
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), 
                        url('https://i.postimg.cc/N0sJGNDf/Screenshot-20260126-232831-Gallery.jpg');
            background-size: cover;
            background-position: center;
            overflow: hidden;
        }

        .container {
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(15px);
            padding: 30px;
            border-radius: 20px;
            text-align: center;
            color: white;
            border: 1px solid rgba(255,255,255,0.4);
            width: 80%;
            z-index: 10;
        }

        .floating-img {
            position: absolute;
            width: 70px;
            height: 70px;
            border-radius: 50%;
            border: 2px solid white;
            object-fit: cover;
            animation: float 4s infinite ease-in-out;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }

        .btn-group { margin-top: 20px; display: flex; justify-content: center; gap: 15px; }

        button {
            padding: 12px 25px;
            border-radius: 50px;
            border: none;
            font-weight: bold;
            cursor: pointer;
        }

        #yes-btn { background: #ff4757; color: white; }
        #no-btn { background: white; color: #ff4757; position: relative; }

        #success-msg { display: none; }
    </style>
</head>
<body>

    <img src="https://i.postimg.cc/k40XdtC4/20260123-193159.jpg" class="floating-img" style="top: 10%; left: 5%;">
    <img src="https://i.postimg.cc/k40XdtC4/20260123-193159.jpg" class="floating-img" style="bottom: 15%; right: 10%;">

    <div class="container" id="main-card">
        <h1>Helaawwww JAANEMANN! ✨</h1>
        <p>MERE PASS APKE LIYE KUCH HAI...</p>
        <h2 style="color: #ff4757;">Will you be mine? 💍</h2>
        
        <div class="btn-group">
            <button id="yes-btn" onclick="celebrate()">YES! ❤️</button>
            <button id="no-btn">No</button>
        </div>
    </div>

    <div class="container" id="success-msg">
        <h1>I Love You! 🎉❤️</h1>
        <p>You are the best I LOVE YOU!</p>
        <p style="font-size: 40px;">♾️💑</p>
    </div>

    <script>
        const noBtn = document.getElementById('no-btn');

        // Ye function button ko bhagayega
        function bhagButton() {
            // Screen ki width aur height ke hisaab se random jagah
            const x = Math.random() * (window.innerWidth - noBtn.clientWidth - 50);
            const y = Math.random() * (window.innerHeight - noBtn.clientHeight - 50);
            
            noBtn.style.position = 'fixed';
            noBtn.style.left = x + 'px';
            noBtn.style.top = y + 'px';
        }

        // Jab woh mobile pe touch karegi
        noBtn.addEventListener('touchstart', (e) => {
            e.preventDefault(); // Button click nahi hone dega
            bhagButton();
        });

        // Agar laptop pe dekhegi toh mouse le jaate hi bhagega
        noBtn.addEventListener('mouseover', bhagButton);

        function celebrate() {
            document.getElementById('main-card').style.display = 'none';
            document.getElementById('success-msg').style.display = 'block';
        }
    </script>
</body>
</html>


# For-My-love
