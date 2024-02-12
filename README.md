# san-valentin
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            text-align: center;
            font-family: 'Arial', sans-serif;
        }
        #oso {
            width: 150px;
            height: auto;
        }
        .quiero-button {
            font-size: 16px;
            padding: 10px;
            margin: 5px;
            background-color: #ff5c8d;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .noquiero-button {
            font-size: 12px;
            padding: 5px;
            margin: 5px;
            background-color: #ff5c8d;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
    <script>
        function mostrarRespuesta() {
            alert("¡Sí quiero que seas mi San Valentín! Nos vemos el miércoles. ¡Te amo!");
        }

        function mostrarNoQuiero() {
            alert("Esta opción no es válida. Lo siento.");
        }

        function crearBotones() {
            var cantidadBotones = 500;

            for (var i = 0; i < cantidadBotones; i++) {
                var boton = document.createElement("button");
                boton.textContent = "Sí, quiero ❤️";
                boton.className = "quiero-button";
                boton.onclick = mostrarRespuesta;
                document.body.appendChild(boton);
            }

            var botonNoQuiero = document.createElement("button");
            botonNoQuiero.textContent = "No, gracias";
            botonNoQuiero.className = "noquiero-button";
            botonNoQuiero.onclick = mostrarNoQuiero;
            document.body.appendChild(botonNoQuiero);
        }

        window.onload = crearBotones;
    </script>
</head>
<body>
    <h1>¿Quieres ser mi San Valentín? ❤️</h1>
    <img src="oso.jpg" alt="Osito" id="oso">
</body>
</html>
