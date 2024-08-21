<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quer namorar comigo?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f0f0f0;
            padding: 20px;
        }
        .container {
            background-color: #ffffff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            max-width: 400px;
            margin: auto;
        }
        h1 {
            color: #333;
        }
        .buttons {
            margin: 20px 0;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin: 5px;
        }
        #btnSim {
            background-color: #28a745;
            color: white;
        }
        #btnNao {
            background-color: #dc3545;
            color: white;
        }
        .message, .next-button {
            display: none;
            margin-top: 20px;
        }
        .next-button a {
            text-decoration: none;
            padding: 10px 20px;
            background-color: #007bff;
            color: white;
            border-radius: 5px;
            display: inline-block;
        }
        #warning {
            color: red;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Quer namorar comigo?</h1>
        <div class="buttons">
            <button id="btnSim">Sim</button>
            <button id="btnNao">Não</button>
        </div>
        <div id="warning">Eu não me atreveria a apertar o não</div>
        <div id="messageNao" class="message">Acho melhor você apertar o sim, hein.</div>
        <div id="messageSim" class="message">
            Caramba… eu não fazia ideia de que você iria aceitar. Bem, primeiramente, eu aprendi a fazer programação durante um tempo e resolvi colocá-la em prática. Legal, né? Bem, vamos ao que interessa… É gratificante saber que tenho você ao meu lado. Gosto da sua companhia, da sua personalidade, da pessoa incrível que você é e de cada coisa que me faz lembrar você. Você sempre poderá contar comigo. Aceita o meu pedido? Prometo amar você muito mais do que Javier Gonzales amou Eleanor Roosevelt.
        </div>
        <div class="next-button">
            <a href="https://youtu.be/UQhDEJhtkv0?si=9XA6kY6sbC_h21iD">Apertar depois de ler o texto</a>
        </div>
    </div>

    <script>
        document.getElementById('btnNao').addEventListener('click', function() {
            this.style.display = 'none';
            document.getElementById('messageNao').style.display = 'block';
        });

        document.getElementById('btnSim').addEventListener('click', function() {
            document.getElementById('messageSim').style.display = 'block';
            document.querySelector('.next-button').style.display = 'block';
        });
    </script>

</body>
</html>
