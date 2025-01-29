<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Live Store - Loja de Roupas Virtuais</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f7f7f7;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }
        .container {
            width: 80%;
            max-width: 800px;
            background-color: white;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
            text-align: left;
            color: #333;
        }
        h1 {
            color: #008cba;
        }
        h2 {
            color: #005f75;
        }
        p {
            color: #555;
            background-color: #f7f7f7;
            padding: 10px;
            border-radius: 5px;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        ul li {
            background-color: #f0f0f0;
            margin: 5px 0;
            padding: 10px;
            border-radius: 5px;
        }
        .highlight {
            color: blue;
            font-size: 20px;
            font-style: italic;
        }
        .nav-link {
            text-decoration: none;
            color: #008cba;
            font-weight: bold;
            padding: 10px 20px;
            border-radius: 5px;
            transition: background-color 0.3s ease, color 0.3s ease;
        }
        .nav-link:hover {
            background-color: #005f75;
            color: #ffffff;
        }
        .button {
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #008cba;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .button:hover {
            background-color: #005f75;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Bem-vindo à Live Store</h1>
        <p>Estamos felizes de te ver por aqui. Explore nosso site e descubra tudo o que temos a oferecer!</p>
        <button class="button" onclick="alert('Seja bem-vindo!')">Clique aqui</button>
        <nav>
            <a class="nav-link" href="outra/index.html">Cartões</a>
            <a class="nav-link" href="outra1/index.html">Bandeiras</a>
        </nav>
        <h1>Sobre a Live Store</h1>
        <p>A Live Store é uma loja de roupas virtuais que oferece as últimas tendências da moda diretamente para você. Nosso objetivo é fornecer peças de alta qualidade e estilo incomparável, garantindo uma experiência de compra única e satisfatória.</p>
        <h2>Nossos Produtos</h2>
        <ul>
            <li>Vestidos elegantes para todas as ocasiões</li>
            <li>Camisas e camisetas estilosas</li>
            <li>Calças e jeans confortáveis</li>
            <li>Acessórios que complementam seu look</li>
        </ul>
        <div class="highlight">Explore agora mesmo e renove seu guarda-roupa com a Live Store!</div>
    </div>
</body>
</html>