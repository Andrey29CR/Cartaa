<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carta con Amor</title>
    <style>
        /* Estilos generales */
        body {
            font-family: 'Georgia', serif;
            margin: 0;
            padding: 0;
            background-color: #ffe4e1;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        /* Estilo del contenedor cerrado */
        .carta-cerrada {
            width: 300px;
            height: 200px;
            background: linear-gradient(45deg, #ff7f7f, #ffb6c1);
            border-radius: 15px;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #fff;
            font-size: 20px;
            text-align: center;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
            cursor: pointer;
            position: relative;
            animation: bounce 2s infinite;
        }

        .carta-cerrada::before {
            content: "❤️";
            font-size: 50px;
            position: absolute;
            top: -30px;
        }

        @keyframes bounce {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }

        /* Contenedor de la carta abierta (oculta inicialmente) */
        .carta-abierta {
            display: none;
            width: 90%;
            max-width: 600px;
            background-color: #fff0f5;
            border-radius: 15px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
            padding: 30px;
            color: #444;
        }

        /* Encabezado */
        .carta-abierta h1 {
            text-align: center;
            color: #ff69b4;
            margin-bottom: 20px;
            font-family: 'Cursive', serif;
        }

        /* Decoración adicional */
        .decoracion {
            text-align: center;
            font-size: 25px;
            color: #ff6a6a;
            margin-bottom: 20px;
        }

        /* Texto principal */
        .carta-abierta p {
            line-height: 1.8;
            font-size: 18px;
            margin: 10px 0;
        }

        /* Firma */
        .carta-abierta .firma {
            margin-top: 20px;
            text-align: right;
            font-size: 16px;
            font-weight: bold;
            color: #555;
        }

        /* Footer */
        .footer {
            margin-top: 20px;
            text-align: center;
            font-size: 14px;
            color: #aaa;
        }
    </style>
</head>
<body>
    <!-- Carta cerrada -->
    <div class="carta-cerrada" id="cartaCerrada" onclick="abrirCarta()">
        📩 ❤️  Ábreme  ❤️📩
    </div>

    <!-- Carta abierta -->
    <div class="carta-abierta" id="cartaAbierta">
        <div class="decoracion">Para Las Piojosas </div>
        <h1> 💖💌💖 </h1>
        <p>
            Chichas espero que pasen un bonito día, que en esta nueva etapa Dios las guie y las bendiga siempre. 🙏 
        </p>
        <p>
            Nunca olviden lo especiales que son y que con Dios todo es posible.
            <p> "Todo lo puedo en Cristo que me fortalece" Filipenses 4:13  </p>
        </p>
        <p>
            Recuerden que pueden contar siempre conmigo para lo que necesiten y espero que cumplan todas las metas y sueños que se propongan 
        </p>
        <p class="firma">
            Con Cariño,<br>
            Su primo OKO 💞 
        </p>
        <div class="footer">
            <p>💞 Muchos exitos en esta nueva etapa 💞</p>
            <p>Las Quiero Mucho 🫶🏻 </p>
        </div>
    </div>

    <script>
        // Función para abrir la carta
        function abrirCarta() {
            document.getElementById('cartaCerrada').style.display = 'none';
            document.getElementById('cartaAbierta').style.display = 'block';
        }
    </script>
</body>
</html>
