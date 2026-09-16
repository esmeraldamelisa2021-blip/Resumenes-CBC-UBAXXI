[gemini-code-1789593821549.html](https://github.com/user-attachments/files/32309779/gemini-code-1789593821549.html)
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Resúmenes UBA XXI - ICSE Pedrosa</title>
    <!-- Fuentes modernas -->
    <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&family=Quicksand:wght@500;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --uba-blue: #0055A5;
            --uba-light-blue: #00A8E8;
            --accent-yellow: #FFD166;
            --accent-orange: #FF70A6;
            --price-green: #06D6A0;
            --bg-light: #F4F7F6;
            --dark-text: #1D2D44;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Quicksand', sans-serif;
        }

        body {
            background-color: var(--bg-light);
            color: var(--dark-text);
            line-height: 1.6;
        }

        /* HEADER */
        header {
            background: linear-gradient(135deg, var(--uba-blue), #002B5B);
            color: white;
            padding: 3rem 1rem 2.5rem 1rem;
            text-align: center;
            border-bottom: 8px solid var(--accent-yellow);
        }

        header .badge {
            background-color: var(--accent-orange);
            color: white;
            font-weight: bold;
            padding: 0.4rem 1rem;
            border-radius: 20px;
            display: inline-block;
            font-size: 0.9rem;
            margin-bottom: 1rem;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        header h1 {
            font-family: 'Fredoka One', cursive;
            font-size: 2.8rem;
            margin-bottom: 0.8rem;
            color: var(--accent-yellow);
            text-shadow: 2px 2px 0px rgba(0,0,0,0.2);
        }

        header p {
            font-size: 1.2rem;
            max-width: 650px;
            margin: 0 auto 1.5rem auto;
        }

        /* CONTAINER */
        .container {
            max-width: 900px;
            margin: 2rem auto;
            padding: 0 1.5rem;
        }

        /* TARJETA DE PRODUCTO */
        .product-card {
            background: white;
            border-radius: 25px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.08);
            border: 3px solid #E0E6ED;
            overflow: hidden;
            margin-bottom: 3rem;
            display: flex;
            flex-direction: column;
        }

        .product-header {
            background: linear-gradient(90deg, var(--uba-light-blue), var(--uba-blue));
            color: white;
            padding: 1.5rem;
            text-align: center;
        }

        .product-header h2 {
            font-family: 'Fredoka One', cursive;
            font-size: 2.2rem;
            color: var(--accent-yellow);
        }

        .product-header p {
            font-size: 1.1rem;
            opacity: 0.95;
        }

        .product-body {
            padding: 2rem;
        }

        /* BANNER DE PRECIO */
        .price-box {
            background-color: #E8F8F5;
            border: 2px dashed var(--price-green);
            border-radius: 15px;
            padding: 1rem;
            text-align: center;
            margin-bottom: 1.5rem;
        }

        .price-box span {
            display: block;
            font-size: 0.95rem;
            color: #2D6A4F;
            font-weight: bold;
            text-transform: uppercase;
        }

        .price-amount {
            font-family: 'Fredoka One', cursive;
            font-size: 2.5rem;
            color: #1B4332;
        }

        .features-list {
            list-style: none;
            margin: 1.5rem 0;
        }

        .features-list li {
            padding: 0.6rem 0;
            font-size: 1.1rem;
            display: flex;
            align-items: center;
            border-bottom: 1px dashed #E0E6ED;
        }

        .features-list li:last-child {
            border-bottom: none;
        }

        .features-list li::before {
            content: "✨";
            margin-right: 12px;
            font-size: 1.2rem;
        }

        .topics-box {
            background-color: #EBF5FF;
            border-left: 5px solid var(--uba-blue);
            padding: 1.2rem;
            border-radius: 12px;
            margin-top: 1.5rem;
        }

        .topics-box h4 {
            font-family: 'Fredoka One', cursive;
            color: var(--uba-blue);
            margin-bottom: 0.5rem;
            font-size: 1.2rem;
        }

        /* BOTÓN DE COMPRA */
        .buy-section {
            text-align: center;
            padding: 1.5rem;
            background-color: #FAFBFD;
            border-top: 2px solid #E0E6ED;
        }

        .whatsapp-btn {
            background-color: #25D366;
            color: white;
            padding: 1rem 2.2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.3rem;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            box-shadow: 0 5px 15px rgba(37, 211, 102, 0.3);
            transition: transform 0.2s, background-color 0.2s;
        }

        .whatsapp-btn:hover {
            background-color: #1eb857;
            transform: translateY(-3px);
        }

        /* METODOLOGÍA / BENEFICIOS */
        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .benefit-card {
            background: white;
            padding: 1.5rem;
            border-radius: 18px;
            text-align: center;
            box-shadow: 0 4px 12px rgba(0,0,0,0.05);
            border-top: 5px solid var(--accent-orange);
        }

        .benefit-card h3 {
            font-family: 'Fredoka One', cursive;
            color: var(--dark-text);
            margin-bottom: 0.5rem;
        }

        /* FOOTER */
        footer {
            background-color: var(--dark-text);
            color: white;
            text-align: center;
            padding: 2.5rem 1rem;
            margin-top: 4rem;
        }

        footer h3 {
            font-family: 'Fredoka One', cursive;
            color: var(--accent-yellow);
            margin-bottom: 0.5rem;
        }

        .phone-display {
            font-size: 1.3rem;
            font-weight: bold;
            color: var(--uba-light-blue);
            margin-top: 0.5rem;
        }

        /* RESPONSIVE */
        @media (max-width: 600px) {
            header h1 { font-size: 2rem; }
            .product-header h2 { font-size: 1.8rem; }
            .whatsapp-btn { font-size: 1.1rem; width: 100%; justify-content: center; }
            .price-amount { font-size: 2.1rem; }
        }
    </style>
</head>
<body>

    <!-- HEADER -->
    <header>
        <span class="badge">UBA XXI · Resúmenes</span>
        <h1>¡Aprobá tu Parcial de ICSE! 🎓📖</h1>
        <p>Ahorrá horas de lectura con resúmenes completos, explicados de forma clara, directa y estructurados clase por clase.</p>
    </header>

    <div class="container">

        <!-- TARJETA DEL RESUMEN -->
        <div class="product-card">
            <div class="product-header">
                <h2>ICSE · Cátedra Pedrosa</h2>
                <p>Introducción al Conocimiento de la Sociedad y el Estado (UBA XXI)</p>
            </div>
            
            <div class="product-body">
                <!-- SECCIÓN DE PRECIO -->
                <div class="price-box">
                    <span>Precio Promocional</span>
                    <div class="price-amount">$6.000 ARS</div>
                </div>

                <p><strong>¿Qué incluye este resumen?</strong>[cite: 1]</p>
                
                <ul class="features-list">
                    <li><strong>Estructura clara:</strong> Organizado semana por semana para estudiar en orden cronológico[cite: 1].</li>
                    <li><strong>Conceptos clave explicados:</strong> Estado, Nación, Populismo, Ciudadanía, Democracia, tipos de Estado y más[cite: 1].</li>
                    <li><strong>Autores de la cátedra:</strong> Weber, Hobbes, Bourdieu, Jelin, Gellner, Anderson y Hobsbawm resumidos[cite: 1].</li>
                    <li><strong>Sintetizado y listo para usar:</strong> Ideal para repasar rápido y fijar conceptos antes del examen[cite: 1].</li>
                </ul>

                <div class="topics-box">
                    <h4>📌 Contenidos del 1er Parcial incluidos:</h4>
                    <p>• <strong>Semana 1:</strong> Conceptos de Estado, tipos de Estado (Liberal, Fascista, Bienestar, Neoliberal) y Nación[cite: 1].<br>
                       • <strong>Semana 2:</strong> Conceptos de Populismo, Democracia, Sociedad Civil y Actores Sociales[cite: 1].<br>
                       • <strong>Semana 3 a 5:</strong> Golpes de Estado y capítulos de Romero[cite: 1].</p>
                </div>
            </div>

            <!-- SECCIÓN DE COMPRA POR WHATSAPP -->
            <div class="buy-section">
                <p style="margin-bottom: 1rem; font-weight: bold; font-size: 1.1rem;">Recibí el PDF de inmediato en tu celular o mail por solo $6.000:</p>
                
                <!-- Enlace a WhatsApp con número +54 9 11 4099-2106 y texto del precio -->
                <a href="https://wa.me/5491140992106?text=Hola!%20Quiero%20comprar%20el%20resumen%20de%20ICSE%20UBA%20XXI%20(Pedrosa)%20por%20$6000" target="_blank" class="whatsapp-btn">
                    💬 Comprar por WhatsApp ($6.000)
                </a>
            </div>
        </div>

        <!-- VENTAJAS DEL RESUMEN -->
        <div class="benefits-grid">
            <div class="benefit-card">
                <h3>⚡ Entrega Inmediata</h3>
                <p>Te envío el archivo PDF al instante apenas realizás la compra.</p>
            </div>
            <div class="benefit-card">
                <h3>📲 Formato Digital</h3>
                <p>Leelo cómodamente desde tu celular, tablet, computadora o imprimilo.</p>
            </div>
            <div class="benefit-card">
                <h3>🎯 Directo al Punto</h3>
                <p>Sin rodeos ni texto de relleno, enfocado en los temas que toman en los parciales[cite: 1].</p>
            </div>
        </div>

    </div>

    <!-- FOOTER -->
    <footer>
        <h3>¿Tenés alguna consulta?</h3>
        <p>Escribime directamente por WhatsApp para coordinar la compra[cite: 1].</p>
        <p class="phone-display">📱 11 4099-2106</p>
        
        <p style="margin-top: 2rem; font-size: 0.85rem; opacity: 0.7;">© 2026 Resúmenes UBA XXI | Material de estudio para estudiantes</p>
    </footer>

</body>
</html>
