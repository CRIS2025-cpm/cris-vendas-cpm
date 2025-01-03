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
    </style>
    <script>
        let cart = [];

        function addToCart(item, quantity) {
            if (quantity <= 0 || isNaN(quantity)) {
                alert('Por favor, insira uma quantidade válida.');
                return;
            }
            cart.push({ item, quantity });
            alert(`${quantity} unidade(s) de "${item}" foram adicionadas ao carrinho!`);
        }

        function removeFromCart(item) {
            cart = cart.filter(cartItem => cartItem.item !== item);
            alert(`"${item}" foi removido do carrinho.`);
        }

        function finalizePurchase() {
            if (cart.length === 0) {
                alert('Seu carrinho está vazio.');
                return;
            }

            const cartSummary = cart.map(cartItem => `${cartItem.quantity}x ${cartItem.item}`).join(', ');
            const whatsappMessage = `Olá, gostaria de comprar os seguintes itens: ${cartSummary}`;
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

        <!-- Primeira Conta -->
        <h3>Conta Full - Todos os Carros</h3>
        <ul>
            <li>50 milhões de Dinheiro</li>
            <li>30 mil ou 500 mil de Gold</li>
            <li>Todos os carros desbloqueados</li>
        </ul>
        <h4>Preço: R$ 4,00</h4>
        <div class="cta">
            <input type="number" class="quantity-input" id="quant1" placeholder="Qtd" min="1">
            <button onclick="addToCart('Conta Full - Todos os Carros', parseInt(document.getElementById('quant1').value))">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('Conta Full - Todos os Carros')">Remover</button>
        </div>

        <!-- Segunda Conta -->
        <h3>Conta Full - 70 Carros com Plot</h3>
        <ul>
            <li>50 milhões de Dinheiro</li>
            <li>30 mil ou 500 mil de Gold</li>
            <li>70 Carros com Plot</li>
        </ul>
        <h4>Preço: R$ 7,00</h4>
        <div class="cta">
            <input type="number" class="quantity-input" id="quant2" placeholder="Qtd" min="1">
            <button onclick="addToCart('Conta Full - 70 Carros com Plot', parseInt(document.getElementById('quant2').value))">Adicionar ao Carrinho</button>
            <button onclick="removeFromCart('Conta Full - 70 Carros com Plot')">Remover</button>
        </div>

        <!-- Golds -->
        <h3>Golds</h3>
        <ul>
            <li>10K de Golds: R$ 2,00 
                <input type="number" class="quantity-input" id="gold10" placeholder="Qtd" min="1">
                <button onclick="addToCart('10K de Golds', parseInt(document.getElementById('gold10').value))">Adicionar</button>
                <button onclick="removeFromCart('10K de Golds')">Remover</button>
            </li>
            <li>30K de Golds: R$ 3,00 
                <input type="number" class="quantity-input" id="gold30" placeholder="Qtd" min="1">
                <button onclick="addToCart('30K de Golds', parseInt(document.getElementById('gold30').value))">Adicionar</button>
                <button onclick="removeFromCart('30K de Golds')">Remover</button>
            </li>
            <li>100K de Golds: R$ 4,00 
                <input type="number" class="quantity-input" id="gold100" placeholder="Qtd" min="1">
                <button onclick="addToCart('100K de Golds', parseInt(document.getElementById('gold100').value))">Adicionar</button>
                <button onclick="removeFromCart('100K de Golds')">Remover</button>
            </li>
        </ul>

        <!-- Dinheiro do Jogo -->
        <h3>Dinheiro do Jogo</h3>
        <ul>
            <li>5M: R$ 0,50 
                <input type="number" class="quantity-input" id="money5" placeholder="Qtd" min="1">
                <button onclick="addToCart('5M de Dinheiro do Jogo', parseInt(document.getElementById('money5').value))">Adicionar</button>
                <button onclick="removeFromCart('5M de Dinheiro do Jogo')">Remover</button>
            </li>
            <li>10M: R$ 1,00 
                <input type="number" class="quantity-input" id="money10" placeholder="Qtd" min="1">
                <button onclick="addToCart('10M de Dinheiro do Jogo', parseInt(document.getElementById('money10').value))">Adicionar</button>
                <button onclick="removeFromCart('10M de Dinheiro do Jogo')">Remover</button>
            </li>
            <li>30M: R$ 2,00 
                <input type="number" class="quantity-input" id="money30" placeholder="Qtd" min="1">
                <button onclick="addToCart('30M de Dinheiro do Jogo', parseInt(document.getElementById('money30').value))">Adicionar</button>
                <button onclick="removeFromCart('30M de Dinheiro do Jogo')">Remover</button>
            </li>
        </ul>

        <!-- Finalizar Compra -->
        <div class="cta">
            <button onclick="finalizePurchase()">Finalizar Compra</button>
        </div>
    </div>
</body>
</html>
