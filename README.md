# Reloj-digital
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TIU Virtual</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f5f5f5;
            padding: 20px;
        }
        #clock {
            font-size: 2em;
            font-weight: bold;
            background: #ddd;
            display: inline-block;
            padding: 10px 20px;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <h1>TIU Virtual</h1>
    <p id="date"></p>
    <div id="clock"></div>

    <script>
        function updateTime() {
            const now = new Date();
            document.getElementById('clock').textContent = now.toLocaleTimeString();
            document.getElementById('date').textContent = now.toLocaleDateString('es-ES', {
                weekday: 'long', year: 'numeric', month: 'long', day: 'numeric'
            });
        }
        setInterval(updateTime, 1000);
        updateTime();
    </script>
</body>
</html>
Commit changes
