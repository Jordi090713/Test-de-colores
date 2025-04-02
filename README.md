# Test-de-colores
Test ( Quantos colores sabes?)

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🎨 Test de Colores Favoritos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            text-align: center;
            padding: 50px;
        }
        h1 {
            color: #333;
        }
        .color-button {
            padding: 20px;
            margin: 10px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.2rem;
            border: none;
            transition: transform 0.2s;
        }
        .color-button:hover {
            transform: scale(1.1);
        }
        #result {
            margin-top: 30px;
            font-size: 1.5rem;
            color: #e74c3c;
        }
    </style>
</head>
<body>

    <h1>🎨 Test de Colores Favoritos</h1>
    <p>¡Elige tu color favorito para empezar!</p>

    <button class="color-button" style="background-color: #FF5733;" onclick="showResult('rojo')">Rojo</button>
    <button class="color-button" style="background-color: #33FF57;" onclick="showResult('verde')">Verde</button>
    <button class="color-button" style="background-color: #3357FF;" onclick="showResult('azul')">Azul</button>
    <button class="color-button" style="background-color: #FF33A1;" onclick="showResult('rosa')">Rosa</button>

    <div id="result"></div>

    <script>
        function showResult(color) {
            let resultText = "";
            
            if (color === 'rojo' || color === 'verde' || color === 'azul' || color === 'rosa') {
                resultText = "Me lo temía, ¡eres realmente gilipollas!";
            } else {
                resultText = "¡Interesante elección!";
            }
            
            document.getElementById("result").textContent = resultText;
        }
    </script>

</body>
</html>  
