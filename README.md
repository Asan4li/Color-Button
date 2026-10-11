

<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Кнопка Старт</title>

<style>
    body {
        margin: 0;
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        background: #111122;
        font-family: Arial, sans-serif;
    }

    .start-button {
        padding: 22px 65px;
        font-size: 30px;
        font-weight: bold;
        color: white;
        border: none;
        border-radius: 18px;
        cursor: pointer;

        background: linear-gradient(
            45deg,
            #ff0000,
            #ff9900,
            #ffee00,
            #00ff66,
            #00ccff,
            #6633ff,
            #ff00cc
        );

        background-size: 400% 400%;
        animation: rainbow 4s ease infinite;

        box-shadow: 0 0 25px #ff00cc;
        transition: transform 0.3s;
    }

    .start-button:hover {
        transform: scale(1.15);
        box-shadow: 0 0 40px #00ccff;
    }

    .start-button:active {
        transform: scale(0.95);
    }

    @keyframes rainbow {
        0%   { background-position: 0% 50%; }
        50%  { background-position: 100% 50%; }
        100% { background-position: 0% 50%; }
    }
</style>
</head>

<body>

<button class="start-button" onclick="startGame()">
    ▶ СТАРТ
</button>

<script>
    function startGame() {
        alert("🚀 Игра начинается!");
    }
</script>

</body>
</html>

