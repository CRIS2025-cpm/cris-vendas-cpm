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
        <h2>Detalhes das Contas</h2>

        <!-- Primeira Conta -->
        <h3>Conta Full - Todos os Carros</h3>
        <p>Confira abaixo tudo o que está incluído nesta conta:</p>
        <ul>
            <li><strong>Dinheiro:</strong> 50 milhões.</li>
            <li><strong>Gold:</strong> 30 mil ou 500 mil (dependendo da sua escolha).</li>
            <li><strong>Todos os carros desbloqueados.</strong></li>
            <li><strong>Todas as buzinas pagas.</strong></li>
            <li><strong>Sirene instalada em alguns carros.</strong></li>
            <li><strong>Motor W16 permanente na conta.</strong></li>
            <li><strong>3ª casa paga liberada.</strong></li>
            <li><strong>ID personalizado (opcional).</strong></li>
            <li><strong>Nome colorido.</strong></li>
            <li><strong>Título King.</strong></li>
        </ul>
        <h4>Preço</h4>
        <p><strong>R$ 4,00</strong> - Pagamento via Pix ou transferência bancária.</p>
        <div class="cta">
            <a href="https://wa.me/5532991584303" target="_blank">Comprar Agora via WhatsApp</a>
        </div>

        <!-- Segunda Conta -->
        <h3>Conta Full - 70 Carros com Plot</h3>
        <p>Confira abaixo tudo o que está incluído nesta conta:</p>
        <ul>
            <li><strong>Dinheiro:</strong> 50 milhões.</li>
            <li><strong>Gold:</strong> 30 mil ou 500 mil (dependendo da sua escolha).</li>
            <li><strong>70 carros com plot incluídos.</strong></li>
            <li><strong>Todas as buzinas pagas.</strong></li>
            <li><strong>Sirene instalada em alguns carros.</strong></li>
            <li><strong>Motor W16 permanente na conta.</strong></li>
            <li><strong>3ª casa paga liberada.</strong></li>
            <li><strong>ID personalizado (opcional).</strong></li>
            <li><strong>Nome colorido.</strong></li>
            <li><strong>Título King.</strong></li>
        </ul>
        <h4>Preço</h4>
        <p><strong>R$ 7,00</strong> - Pagamento via Pix ou transferência bancária.</p>
        <div class="cta">
            <a href="https://wa.me/5532991584303" target="_blank">Comprar Agora via WhatsApp</a>
        </div>
    </div>
</body>
</html> 
