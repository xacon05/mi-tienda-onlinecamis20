<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SportShop 2026 | Equipaciones</title>
    <style>
        /* Variables de diseño deportivo */
        :root {
            --bg-dark: #121212;
            --card-dark: #1e1e1e;
            --accent: #ff4757;
            --text-light: #ffffff;
            --barca: #a50044;
            --madrid: #000000;
            --betis: #008f39;
        }

        body {
            font-family: 'Oswald', sans-serif; /* Tipografía tipo deporte */
            background-color: var(--bg-dark);
            color: var(--text-light);
            margin: 0;
            text-transform: uppercase;
        }

        header {
            background: linear-gradient(135deg, #000 0%, #333 100%);
            padding: 60px 20px;
            text-align: center;
            border-bottom: 4px solid var(--accent);
        }

        header h1 { font-size: 3rem; margin: 0; letter-spacing: 2px; }
        header p { color: var(--accent); font-weight: bold; }

        .container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
            padding: 50px 20px;
            max-width: 1200px;
            margin: auto;
        }

        /* Tarjeta Estilo Deportivo */
        .card {
            background: var(--card-dark);
            border: 1px solid #333;
            border-radius: 0px; /* Bordes rectos = más agresivo/deportivo */
            overflow: hidden;
            transition: 0.3s;
            position: relative;
        }

        .card:hover {
            border-color: var(--accent);
            transform: scale(1.02);
        }

        .card img {
            width: 100%;
            height: 350px;
            object-fit: cover;
            filter: grayscale(30%);
            transition: 0.5s;
        }

        .card:hover img { filter: grayscale(0%); }

        .badge {
            position: absolute;
            top: 15px;
            right: 15px;
            background: var(--accent);
            padding: 5px 15px;
            font-weight: bold;
            font-size: 1.2rem;
        }

        .info { padding: 25px; text-align: left; }
        
        .team-name { font-size: 1.5rem; margin: 0; }
        .price { font-size: 2rem; color: var(--accent); margin: 10px 0; }

        .buy-btn {
            display: block;
            width: 100%;
            padding: 15px;
            text-align: center;
            text-decoration: none;
            color: white;
            font-weight: bold;
            font-size: 1.1rem;
            border: none;
            cursor: pointer;
            transition: 0.3s;
        }

        /* Colores específicos */
        .btn-barca { background-color: var(--barca); }
        .btn-madrid { background-color: var(--madrid); border: 1px solid #fff; }
        .btn-betis { background-color: var(--betis); }

        .buy-btn:hover { opacity: 0.8; letter-spacing: 3px; }

    </style>
    <link href="https://fonts.googleapis.com/css2?family=Oswald:wght@700&display=swap" rel="stylesheet">
</head>
<body>

<header>
    <h1>TOP TEAMS 2026</h1>
    <p>SENTIMIENTO EN CADA FIBRA • ENVÍO GRATIS</p>
</header>

<div class="container">
    <div class="card">
        <div class="badge">20€</div>
        <img src="https://images.unsplash.com/photo-1522778119026-d647f0596c20?w=600" alt="Barça">
        <div class="info">
            <p class="team-name">FC BARCELONA</p>
            <p style="font-size: 0.8rem; color: #888;">HOME KIT 25/26</p>
            <div class="price">20.00€</div>
            <button class="buy-btn btn-barca" onclick="window.location.href='URL_PAGO_BARCA'">COMPRAR AHORA</button>
        </div>
    </div>

    <div class="card">
        <div class="badge">20€</div>
        <img src="https://images.unsplash.com/photo-1599401042594-859b1bdad92a?w=600" alt="Madrid">
        <div class="info">
            <p class="team-name">REAL MADRID</p>
            <p style="font-size: 0.8rem; color: #888;">ELITE EDITION</p>
            <div class="price">20.00€</div>
            <button class="buy-btn btn-madrid" onclick="window.location.href='URL_PAGO_MADRID'">COMPRAR AHORA</button>
        </div>
    </div>

    <div class="card">
        <div class="badge">20€</div>
        <img src="https://images.unsplash.com/photo-1518091043644-c1d4457512c6?w=600" alt="Betis">
        <div class="info">
            <p class="team-name">REAL BETIS</p>
            <p style="font-size: 0.8rem; color: #888;">VERDIBLANCA 2026</p>
            <div class="price">20.00€</div>
            <button class="buy-btn btn-betis" onclick="window.location.href='URL_PAGO_BETIS'">COMPRAR AHORA</button>
        </div>
    </div>
</div>

</body>
</html>
