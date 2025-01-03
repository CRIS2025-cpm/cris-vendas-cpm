<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CRIS VENDAS CPM - Loja Oficial</title>
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
        }
        .container {
            max-width: 800px;
            margin: 20px auto;
            background: white;
            padding: 20px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
            border-radius: 10px;
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
        .cta button {
            padding: 10px 20px;
            background-color: #0078d7;
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 16px;
            cursor: pointer;
        }
        .cta button:hover {
            background-color: #005bb5;
        }
        .quantity-input {
            width: 60px;
            padding: 5px;
            text-align: center;
            margin-right: 10px;
        }
        .contact-owner {
            text-align: center;
            margin-top: 40px;
            font-size: 40px;
            font-weight: bold;
            color: #ff4500;
            text-shadow: 2px 2px 4px #000;
        }
        .arrow {
            font-size: 40px;
            color: #ff4500;
        }
        .whatsapp-link {
            display: block;
            text-align: center;
            margin-top: 10px;
            font-size: 24px;
            font-weight: bold;
            color: #0078d7;
            text-decoration: none;
        }
        .whatsapp-link:hover {
            text-decoration: underline;
            color: #005bb5;
        }
    </style>
    <script>
        let cart = [];

        function addToCart(item, quantity) {
            const cartItem = { item, quantity };
            cart.push(cartItem);
            alert(`${quantity} unidade(s) de ${item} foram adicionadas ao carrinho!`);
        }

        function removeFromCart(item) {
            cart = cart.filter(cartItem => cartItem.item !== item);
            alert(`${item} foi removido do carrinho.`);
        }

        function finalizePurchase() {
            if (cart.length === 0) {
                alert('Seu carrinho está vazio.');
                return;
            }

            const cartDetails = cart.map(cartItem => `${cartItem.quantity}x ${cartItem.item}`).join(', ');
            const whatsappMessage = `Olá, gostaria de comprar os seguintes itens: ${cartDetails}`;
            const encodedMessage = encodeURIComponent(whatsappMessage);
            const whatsappUrl = `https://wa.me/5574999392169?text=${encodedMessage}`;
            window.location.href = whatsappUrl;
        }
    </script>
</head>
<body>
    <header>
        <h1>CRIS VENDAS CPM</h1>
    </header>
    <div class="container">
        <h2>Detalhes das Contas</h2>

        <!-- Conta Full - Todos os Carros -->
        <h3>Conta Full - Todos os Carros</h3>
        <ul>
            <li>50 milhões de Dinheiro</li>
            <li>30 mil ou 500 mil de Gold</li>
            <li>Todos os carros desbloqueados</li>
            <li>W16 permanente na conta</li>
            <li>King</li>
            <li>Sirene em alguns carros</li>
            <li>Carro Não Quebra</li>
            <li>Todas as buzinas</li>
            <li>Gasolina infinita</li>
            <li>Nome colorido (opcional)</li>
            <li>ID personalizado (opcional)</li>
        </ul>
        <h4>Preço: R$ 4,00</h4>
        <div class="cta">
            <input class="quantity-input" type="number" min="1" value="1" id="quantityFullAllCars">
            <button onclick="addToCart('Conta Full - Todos os Carros', document.getElementById('quantityFullAllCars').value)">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('Conta Full - Todos os Carros')">Remover do Carrinho</button>
        </div>

        <!-- Conta Full - 70 Carros com Plot -->
        <h3>Conta Full - 70 Carros com Plot</h3>
        <ul>
            <li>50 milhões de Dinheiro</li>
            <li>30 mil ou 500 mil de Gold</li>
            <li>70 Carros com Plot</li>
            <li>W16 permanente na conta</li>
            <li>King</li>
            <li>Sirene em alguns carros</li>
            <li>Carro Não Quebra</li>
            <li>Todas as buzinas</li>
            <li>Gasolina infinita</li>
            <li>Nome colorido (opcional)</li>
            <li>ID personalizado (opcional)</li>
        </ul>
        <h4>Preço: R$ 7,00</h4>
        <div class="cta">
            <input class="quantity-input" type="number" min="1" value="1" id="quantityFull70Cars">
            <button onclick="addToCart('Conta Full - 70 Carros com Plot', document.getElementById('quantityFull70Cars').value)">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('Conta Full - 70 Carros com Plot')">Remover do Carrinho</button>
        </div>

        <!-- Golds -->
        <h3>Golds</h3>
        <ul>
            <li>10K de Golds: R$ 2,00</li>
            <li>30K de Golds: R$ 3,00</li>
            <li>100K de Golds: R$ 4,00</li>
            <li>500K de Golds: R$ 5,00</li>
        </ul>
        <div class="cta">
            <input class="quantity-input" type="number" min="1" value="1" id="quantity10KGold">
            <button onclick="addToCart('10K de Golds', document.getElementById('quantity10KGold').value)">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('10K de Golds')">Remover do Carrinho</button>
        </div>
        <div class="cta">
            <input class="quantity-input" type="number" min="1" value="1" id="quantity30KGold">
            <button onclick="addToCart('30K de Golds', document.getElementById('quantity30KGold').value)">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('30K de Golds')">Remover do Carrinho</button>
        </div>
        <div class="cta">
            <input class="quantity-input" type="number" min="1" value="1" id="quantity100KGold">
            <button onclick="addToCart('100K de Golds', document.getElementById('quantity100KGold').value)">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('100K de Golds')">Remover do Carrinho</button>
        </div>
        <div class="cta">
            <input class="quantity-input" type="number" min="1" value="1" id="quantity500KGold">
            <button onclick="addToCart('500K de Golds', document.getElementById('quantity500KGold').value)">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('500K de Golds')">Remover do Carrinho</button>
        </div>

        <!-- Dinheiro do Jogo -->
        <h3>Dinheiro do Jogo</h3>
        <ul>
            <li>5M: R$ 0,50</li>
            <li>10M: R$ 1,00</li>
            <li>30M: R$ 2,00</li>
            <li>50M: R$ 3,00</li>
        </ul>
        <div class="cta">
            <input class="quantity-input" type="number" min="1" value="1" id="quantity5MDinheiro">
            <button onclick="addToCart('5M de Dinheiro do Jogo', document.getElementById('quantity5MDinheiro').value)">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('5M de Dinheiro do Jogo')">Remover do Carrinho</button>
        </div>
        <div class="cta">
            <input class="quantity-input" type="number" min="1" value="1" id="quantity10MDinheiro">
            <button onclick="addToCart('10M de Dinheiro do Jogo', document.getElementById('quantity10MDinheiro').value)">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('10M de Dinheiro do Jogo')">Remover do Carrinho</button>
        </div>
        <div class="cta">
            <input class="quantity-input" type="number" min="1" value="1" id="quantity30MDinheiro">
            <button onclick="addToCart('30M de Dinheiro do Jogo', document.getElementById('quantity30MDinheiro').value)">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('30M de Dinheiro do Jogo')">Remover do Carrinho</button>
        </div>
        <div class="cta">
            <input class="quantity-input" type="number" min="1" value="1" id="quantity50MDinheiro">
            <button onclick="addToCart('50M de Dinheiro do Jogo', document.getElementById('quantity50MDinheiro').value)">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('50M de Dinheiro do Jogo')">Remover do Carrinho</button>
        </div>

        <!-- Finalizar Compra -->
        <div class="cta">
            <button onclick="finalizePurchase()">Finalizar Compra</button>
        </div>
    </div>

    <!-- Fale com o Dono -->
    <div class="contact-owner">
        Fale com o Dono
        <span class="arrow">➡️</span>
        <a class="whatsapp-link" href="https://wa.me/32991584303" target="_blank">Clique aqui para conversar com o dono</a>
    </div>
</body>
</html>
