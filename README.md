<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Festa della Paddoccola - Alfano</title>
    <!-- Importazione font stile hand-made/fumetto e icone -->
    <link rel="preconnect" href="https://googleapis.com">
    <link rel="preconnect" href="https://gstatic.com" crossorigin>
    <link href="https://googleapis.com/css2?family=Fredoka:wght@700&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cloudflare.com">
    
    <style>
        /* Reset generali */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #FF0000;
            color: #ffffff;
            font-family: 'Open Sans', sans-serif;
            overflow-x: hidden;
        }

        /* Schermata Iniziale (Stile Immagine) */
        .hero-section {
            height: 100vh;
            width: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            padding-left: 10%;
            position: relative;
            background-color: #FF0000;
        }

        /* Font in stile fumetto/pennarello come l'immagine */
        .title-container {
            font-family: 'Fredoka', sans-serif;
            text-transform: uppercase;
            line-height: 1.1;
            margin-bottom: 30px;
        }

        .title-top {
            font-size: 2.5rem;
            display: block;
        }

        .title-main {
            font-size: 5rem;
            display: block;
            letter-spacing: 1px;
        }

        .date-info {
            font-family: 'Fredoka', sans-serif;
            font-size: 1.8rem;
            text-transform: uppercase;
            margin-bottom: 50px;
        }

        /* Icone Social Tonde */
        .social-container {
            display: flex;
            gap: 15px;
            margin-bottom: 60px;
        }

        .social-icon {
            width: 45px;
            height: 45px;
            border: 2px solid #ffffff;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #ffffff;
            text-decoration: none;
            font-size: 1.2rem;
            transition: background 0.3s, color 0.3s;
        }

        .social-icon:hover {
            background-color: #ffffff;
            color: #FF0000;
        }

        /* Freccia verso il basso */
        .scroll-arrow {
            width: 45px;
            height: 45px;
            border: 2px solid #ffffff;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #ffffff;
            text-decoration: none;
            font-size: 1.2rem;
            animation: bounce 2s infinite;
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-10px); }
            60% { transform: translateY(-5px); }
        }

        /* Sezioni di Contenuto (Sotto la copertina) */
        .content-container {
            max-width: 900px;
            margin: 0 auto;
            padding: 80px 20px;
        }

        section {
            margin-bottom: 70px;
        }

        h2 {
            font-family: 'Fredoka', sans-serif;
            font-size: 2.5rem;
            text-transform: uppercase;
            margin-bottom: 25px;
            border-bottom: 3px solid #ffffff;
            padding-bottom: 10px;
        }

        p {
            font-size: 1.2rem;
            line-height: 1.7;
            margin-bottom: 20px;
        }

        /* Menu stilizzato in linea con la grafica pulita */
        .menu-list {
            display: flex;
            flex-direction: column;
            gap: 15px;
            margin-top: 30px;
        }

        .menu-row {
            display: flex;
            justify-content: space-between;
            font-size: 1.4rem;
            font-weight: 600;
            border-bottom: 1px dashed rgba(255, 255, 255, 0.4);
            padding-bottom: 8px;
        }

        .menu-price {
            font-family: 'Fredoka', sans-serif;
        }

        /* Info utili */
        .info-box {
            background-color: rgba(255, 255, 255, 0.1);
            padding: 30px;
            border-radius: 10px;
            margin-top: 20px;
        }

        .info-box p {
            margin-bottom: 10px;
            font-weight: 600;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 40px 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.2);
            font-size: 1rem;
            opacity: 0.8;
        }

        /* Adattamento per Smartphone */
        @media (max-width: 768px) {
            .hero-section {
                padding-left: 20px;
            }
            .title-top { font-size: 1.8rem; }
            .title-main { font-size: 3.2rem; }
            .date-info { font-size: 1.4rem; }
            h2 { font-size: 2rem; }
            .menu-row { font-size: 1.1rem; }
        }
    </style>
</head>
<body>

    <!-- COPPERTINA (Uguale alla tua immagine) -->
    <div class="hero-section">
        <div class="title-container">
            <span class="title-top">Alfano <span style="font-size: 3rem;">Festa</span> della</span>
            <span class="title-main">Paddoccola</span>
        </div>
        
        <div class="date-info">
            12-13 Agosto, Ore 20:00
        </div>

        <div class="social-container">
            <a href="#" class="social-icon" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
            <a href="#" class="social-icon" aria-label="Facebook"><i class="fab fa-facebook-f"></i></a>
            <a href="mailto:info@esempio.com" class="social-icon" aria-label="Email"><i class="far fa-envelope"></i></a>
        </div>

        <a href="#storia" class="scroll-arrow" aria-label="Scorri verso il basso">
            <i class="fas fa-arrow-down"></i>
        </a>
    </div>

    <!-- CONTENUTI PAGINA (Scorrendo verso il basso) -->
    <div class="content-container">

        <!-- Storia -->
        <section id="storia">
            <h2>La Nostra Storia</h2>
            <p>La Paddoccola nasce nelle famiglie contadine di Alfano come espressione di cucina "povera". Il segreto del gusto e la consistenza è nell'utilizzo di prodotti locali, con una qualità eccellente e genuina.</p>
            <p>La paddoccola viene lavorata esclusivamente a mano.</p>
            <p>La festa è nata con un obiettivo nobile, salvaguardare questo nostro pezzo di storia culinaria affinchè non andasse perduto, promuovendo allo stesso tempo la bellezza del piccolo borgo di Alfano!</p>
        </section>

        <!-- Menu -->
        <section id="menu">
            <h2>Menu Stand</h2>
            <div class="menu-list">
                <div class="menu-row">
                    <span>PADDOCCOLE (5 PEZZI)</span>
                    <span class="menu-price">€ 4.00</span>
                </div>
                <div class="menu-row">
                    <span>CIAURIEDDU</span>
                    <span class="menu-price">€ 5.00</span>
                </div>
                <div class="menu-row">
                    <span>PANINI</span>
                    <span class="menu-price">€ 4.50</span>
                </div>
                <div class="menu-row">
                    <span>DOLCI VARI</span>
                    <span class="menu-price">€ 2.00</span>
                </div>
                <div class="menu-row">
                    <span>BIRRA</span>
                    <span class="menu-price">€ 2.50</span>
                </div>
                <div class="menu-row">
                    <span>COCA COLA</span>
                    <span class="menu-price">€ 2.00</span>
                </div>
                <div class="menu-row">
                    <span>ACQUA 0.5 L</span>
                    <span class="menu-price">€ 2.00</span>
                </div>
            </div>
        </section>

        <!-- Consigli aggiuntivi integrati con lo stile pulito -->
        <section id="info">
            <h2>Info Utili</h2>
            <div class="info-box">
                <p>📍 Dove: Centro Storico di Alfano (SA)</p>
                <p>🚗 Parcheggio: Disponibile all'ingresso del borgo</p>
                <p>🎶 Intrattenimento: Musica popolare dal vivo nelle piazze</p>
            </div>
        </section>

    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Festa della Paddoccola - Alfano (SA)</p>
    </footer>

</body>
</html>
