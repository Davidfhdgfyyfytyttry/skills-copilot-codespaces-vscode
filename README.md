<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Davi e Wendell Vendas</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
        }
        header {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 1rem 0;
        }
        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 20px;
        }
        .card {
            background: white;
            border: 1px solid #ddd;
            border-radius: 8px;
            margin: 10px;
            padding: 15px;
            width: 300px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        .card img {
            width: 100%;
            border-radius: 5px;
        }
        .card h3 {
            margin: 10px 0;
            color: #333;
        }
        .card button {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 10px 15px;
            cursor: pointer;
            border-radius: 5px;
        }
        .card button:hover {
            background-color: #45a049;
        }
    </style>
    <script>
        function showPaymentInfo(price) {
            const paymentWindow = window.open('', '_blank');
            paymentWindow.document.write(`
                <!DOCTYPE html>
                <html lang="pt-BR">
                <head>
                    <meta charset="UTF-8">
                    <meta name="viewport" content="width=device-width, initial-scale=1.0">
                    <title>Pagamento</title>
                    <style>
                        body {
                            font-family: Arial, sans-serif;
                            text-align: center;
                            margin: 0;
                            padding: 20px;
                            background-color: #f4f4f9;
                        }
                        h1 {
                            color: #333;
                        }
                        p {
                            color: #555;
                            font-size: 18px;
                            margin: 10px 0;
                        }
                    </style>
                </head>
                <body>
                    <h1>Use uma das chaves Pix para o pagamento</h1>
                    <p>Valor: R$${price.toFixed(2)}</p>
                    <p>Chave Pix (Número): <strong>11987652160</strong></p>
                    <p>Chave Pix (E-mail): <strong>natalibmendes@gmail.com</strong></p>
                    <p>Após o pagamento, envie o comprovante para o WhatsApp Para Enviarmos Acesso A Conta: <strong>+55 11 91644-9066</strong></p>
                </body>
                </html>
            `);
        }
    </script>
</head>
<body>
    <header>
        <h1>Davi e Wendell Vendas</h1>
    </header>
    <div style="text-align: center; margin: 20px;">
        <button style="background-color: #4CAF50; color: white; padding: 10px 20px; font-size: 16px; border: none; border-radius: 5px; cursor: pointer;" onclick="showPaymentInfo(18)">Comprar VIP para comprar contas mais barato</button>
    </div>
    <div class="container">
        <!-- Conta 3: alli_xit -->
        <div class="card">
            <img src="/mnt/data/A_mysterious_Roblox_character_in_the_Blox_Fruits_g.png" alt="Conta misteriosa">
            <h3>Conta: alli_xit</h3>
            <p>Nível: 2550 | Fruta: ??? | Preço: R$17,00</p>
            <button onclick="showPaymentInfo(17)">Comprar</button>
        </div>

        <!-- Conta de Brookhaven -->
        <div class="card">
            <img src="https://via.placeholder.com/300" alt="Conta de Brookhaven">
            <h3>Conta: BrookhavenVIP</h3>
            <p>Inclui VIP no Brookhaven, Game Pass do Carro Rápido e Skins de Robux | Preço: R$7,00</p>
            <button onclick="showPaymentInfo(7)">Comprar</button>
        </div>

        <!-- Botão de Sorteio -->
        <div class="card">
            <h3>Participe do Sorteio de uma Conta Misteriosa!</h3>
            <p>Preço: R$0,20</p>
            <button onclick="showPaymentInfo(0.20)">Participar do Sorteio</button>
        </div>
    </div>
</body>
</html>
