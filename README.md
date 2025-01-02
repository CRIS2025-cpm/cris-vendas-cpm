<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CRIS VENDAS CPM - Conta Full Car Parking</title>
    <style>
        /* Reset CSS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #0078d7, #00c3ff);
            color: #333;
            line-height: 1.6;
            overflow-x: hidden;
        }
        header {
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
            padding: 20px;
            text-align: center;
            animation: fadeInDown 1.5s;
        }
        .container {
            max-width: 800px;
            margin: 20px auto;
            background: white;
            padding: 20px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
            border-radius: 10px;
            animation: fadeInUp 1.5s;
        }
        h1, h2, h3, h4 {
            color: #0078d7;
        }
        ul {
            line-height: 1.8;
            margin-left: 20px;
        }
        .cta {
            text-align: center;
            margin-top: 20px;
        }
        .cta a {
            display: inline-block;
            padding: 10px 20px;
            background-color: #0078d7;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            font-size: 16px;
            transition: all 0.3s;
            animation: pulse 2s infinite;
        }
        .cta a:hover {
            background-color: #005bb5;
            transform: scale(1.1);
        }
        /* Animações */
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        @keyframes pulse {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.05);
            }
        }
        /* Responsividade */
        @media (max-width: 600px) {
            body {
                padding: 10px;
            }
            .container {
                margin: 10px;
                padding: 15px;
            }
            header {
                padding: 15px;
            }
            .cta a {
                font-size: 14px;
                padding: 8px 16px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>CRIS VENDAS CPM</h1>
    </header>
    <div class="container">
        <h2>Detalhes dos Produtos</h2>

        <!-- Dinheiro do Jogo -->
        <h3>Dinheiro do Jogo</h3>
        <p>Confira as variações disponíveis:</p>
        <ul>
            <li><strong>5M:</strong> R$ 0,50</li>
            <div class="cta">
                <a href="https://wa.me/74999392169?text=Quero+comprar+5M+de+dinheiro+do+jogo+por+R$0,50">Comprar 5M</a>
            </div>

            <li><strong>10M:</strong> R$ 1,00</li>
            <div class="cta">
                <a href="https://wa.me/74999392169?text=Quero+comprar+10M+de+dinheiro+do+jogo+por+R$1,00">Comprar 10M</a>
            </div>

            <li><strong>30M:</strong> R$ 2,00</li>
            <div class="cta">
                <a href="https://wa.me/74999392169?text=Quero+comprar+30M+de+dinheiro+do+jogo+por+R$2,00">Comprar 30M</a>
            </div>

            <li><strong>40M:</strong> R$ 3,00</li>
            <div class="cta">
                <a href="https://wa.me/74999392169?text=Quero+comprar+40M+de+dinheiro+do+jogo+por+R$3,00">Comprar 40M</a>
            </div>

            <li><strong>50M:</strong> R$ 4,00</li>
            <div class="cta">
                <a href="https://wa.me/74999392169?text=Quero+comprar+50M+de+dinheiro+do+jogo+por+R$4,00">Comprar 50M</a>
            </div>
        </ul>
    </div>
</body>
</html>
