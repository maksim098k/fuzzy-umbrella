<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Скутерец гнойный пидр?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #72EDF2 10%, #5151E5 100%);
            color: #fff;
            text-align: center;
            margin: 0;
            padding: 50px;
            overflow: hidden;
            height: 100vh; /* добавим высоту для полного экрана */
            display: flex;
            justify-content: center;
            align-items: center;
        }
        .container {
            background: rgba(255, 255, 255, 0.1);
            padding: 40px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            display: inline-block;
            width: 80%;
            max-width: 800px;
            border-radius: 10px;
        }
        .btn-container {
            margin-top: 20px;
            position: relative;
            height: 200px;
        }
        .btn {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            margin: 5px;
            transition: all 0.1s;
            border: none;
            border-radius: 5px;
        }
        .btn-yes {
            background-color: #4CAF50;
            color: white;
        }
        .btn-no {
            background-color: #f44336;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Скутерец гнойный пидр?</h1>
        <div class="btn-container">
            <button class="btn btn-yes">Да</button>
            <button class="btn btn-no">Нет</button>
        </div>
    </div>

    <script>
        const btnNo = document.querySelector('.btn-no');
        const btnYes = document.querySelector('.btn-yes');

        btnNo.addEventListener('mouseover', function() {
            const container = document.querySelector('.btn-container');
            const x = Math.random() * (container.clientWidth - btnNo.clientWidth);
            const y = Math.random() * (container.clientHeight - btnNo.clientHeight);
            btnNo.style.left = `${x}px`;
            btnNo.style.top = `${y}px`;
        });

        btnNo.addEventListener('click', function() {
            alert("Ты всё равно лох");
        });

        btnYes.addEventListener('click', function() {
            alert("Ай тигр :)");
        });
    </script>
</body>
</html>
