<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Da Sando - Sedi</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f8f8f8;
            padding: 20px;
        }
        .container {
            max-width: 600px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #333;
        }
        .logo {
            width: 150px;
            margin-bottom: 20px;
        }
        .location {
            margin: 20px 0;
            padding: 15px;
            border: 1px solid #ddd;
            border-radius: 10px;
            background: #fff;
            cursor: pointer;
        }
        .info {
            display: none;
            margin-top: 10px;
        }
        .image {
            width: 100%;
            border-radius: 10px;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="/mnt/data/Progetto senza titolo (17).png" alt="Da Sando Logo" class="logo">
        <h1>Seleziona la tua sede Da Sando</h1>
        
        <div class="location" onclick="toggleInfo('credaro')">
            <img src="https://source.unsplash.com/600x400/?pizza" alt="Pizza" class="image">
            📍 <strong>Credaro</strong> - Via degli Alpini 3, 24060
            <div id="credaro" class="info">
                <p>📞 <a href="tel:0355902944">0355902944</a></p>
                <p>📍 <a href="https://www.google.com/maps/place/Pizzeria+DA+SANDO/@45.6604851,9.9251307,17z/data=!3m1!4b1!4m6!3m5!1s0x4781673cbba1a2eb:0xa568eda458c335ba!8m2!3d45.6604814!4d9.9277056!16s%2Fg%2F11s3xtf8z8?entry=ttu&g_ep=EgoyMDI1MDIxMi4wIKXMDSoASAFQAw%3D%3D" target="_blank">Google Maps</a></p>
                <p>📷 <a href="https://www.instagram.com/dasando_credaro" target="_blank">Instagram</a></p>
                <p>🌐 <a href="https://www.dasando.it" target="_blank">Visita il sito</a></p>
            </div>
        </div>
        
        <div class="location" onclick="toggleInfo('grumello')">
            <img src="https://source.unsplash.com/600x400/?pizza-restaurant" alt="Pizza" class="image">
            📍 <strong>Grumello del Monte</strong> - Viale degli Alpini 31, 24064
            <div id="grumello" class="info">
                <p>📞 <a href="tel:0350632994">0350632994</a></p>
                <p>📍 <a href="https://www.google.com/maps/place//data=!4m2!3m1!1s0x47815d00600e2481:0xfbc40bc046504b0f?sa=X&ved=1t:8290&ictx=111" target="_blank">Google Maps</a></p>
                <p>📷 <a href="https://www.instagram.com/dasando_" target="_blank">Instagram</a></p>
                <p>🌐 <a href="https://www.dasando.it" target="_blank">Visita il sito</a></p>
            </div>
        </div>
        
        <div class="location" onclick="toggleInfo('brescia')">
            <img src="https://source.unsplash.com/600x400/?italian-food" alt="Pizza" class="image">
            📍 <strong>Brescia</strong> - Via Monte Nero 25, 25128
            <div id="brescia" class="info">
                <p>📞 <a href="tel:0308081782">0308081782</a></p>
                <p>📍 <a href="https://www.google.com/maps/place//data=!4m2!3m1!1s0x478177081a579eef:0x29e7567f403a958d?sa=X&ved=1t:8290&ictx=111" target="_blank">Google Maps</a></p>
                <p>📷 <a href="https://www.instagram.com/dasando_brescia" target="_blank">Instagram</a></p>
                <p>🌐 <a href="https://www.dasando.it" target="_blank">Visita il sito</a></p>
            </div>
        </div>
    </div>
    
    <script>
        function toggleInfo(id) {
            var info = document.getElementById(id);
            var allInfos = document.querySelectorAll('.info');
            allInfos.forEach(el => el.style.display = 'none');
            info.style.display = 'block';
        }
    </script>
</body>
</html>
