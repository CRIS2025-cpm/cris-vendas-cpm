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
        img {
            width: 100%;
            max-width: 400px;
            margin: 10px auto;
            display: block;
            border-radius: 10px;
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
            img {
                max-width: 100%;
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
            <a href="https://wa.me/5574999392169" target="_blank">Comprar Agora via WhatsApp</a>
        </div>

        <!-- Segunda Conta -->
        <h3>Conta Full - 70 Carros com Plot</h3>
        <p>Confira abaixo tudo o que está incluído nesta conta:</p>
        
        <!-- Adicionando Imagens -->
        <img src="https://drive.google.com/uc?export=download&id=10lh9rnML643ZaFi6_GHSE4WTt62zfbBz" alt="Conta Full - Imagem 1">
        <img src="https://drive.google.com/uc?export=download&id=10dOReJkPCzPGcq5yeFQsHCXBotnisvJy" alt="Conta Full - Imagem 2">
        <img src="https://drive.google.com/uc?export=download&id=10bvSB7DHsI4_0-n8BlDMmf8_3Iq5ti1Y" alt="Conta Full - Imagem 3">
        
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
            <a href="https://wa.me/5574999392169" target="_blank">Comprar Agora via WhatsApp</a>
        </div>

        <!-- Golds -->
        <h3>Golds</h3>
        <ul>
            <li>10K: R$ 2,00 <a href="https://wa.me/5574999392169?text=Quero+comprar+10K+de+golds+por+R$2,00" class="cta">Comprar</a></li>
            <li>30K: R$ 3,00 <a href="https://wa.me/5574999392169?text=Quero+comprar+30K+de+golds+por+R$3,00" class="cta">Comprar</a></li>
            <li>100K: R$ 4,00 <a href="https://wa.me/5574999392169?text=Quero+comprar+100K+de+golds+por+R$4,00" class="cta">Comprar</a></li>
            <li>500K: R$ 5,00 <a href="https://wa.me/5574999392169?text=Quero+comprar+500K+de+golds+por+R$5,00" class="cta">Comprar</a></li>
        </ul>

        <!-- Dinheiro do Jogo -->
        <h3>Dinheiro do Jogo</h3>
        <ul>
            <li>5M: R$ 0,50 <a href="https://wa.me/5574999392169?text=Quero+comprar+5M+de+dinheiro+do+jogo+por+R$0,50" class="cta">Comprar</a></li>
            <li>10M: R$ 1,00 <a href="https://wa.me/5574999392169?text=Quero+comprar+10M+de+dinheiro+do+jogo+por+R$1,00" class="cta">Comprar</a></li>
            <li>30M: R$ 2,00 <a href="https://wa.me/5574999392169?text=Quero+comprar+30M+de+dinheiro+do+jogo+por+R$2,00" class="cta">Comprar</a></li>
            <li>40M: R$ 3,00 <a href="https://wa.me/5574999392169?text=Quero+comprar+40M+de+dinheiro+do+jogo+por+R$3,00" class="cta">Comprar</a></li>
            <li>50M: R$ 4,00 <a href="https://wa.me/5574999392169?text=Quero+comprar+50M+de+dinheiro+do+jogo+por+R$4,00" class="cta">Comprar</a></li>
        </ul>
    </div>
</body>
</html>
