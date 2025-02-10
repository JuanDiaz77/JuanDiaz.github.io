# JuanDiaz.github.io
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Página Personal</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        header {
            background: #333;
            color: white;
            padding: 10px 0;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-size: 18px;
        }
        .section {
            padding: 50px;
        }
        #contacto input, #contacto textarea {
            width: 80%;
            padding: 10px;
            margin: 10px 0;
        }
        button {
            padding: 10px 20px;
            background: #333;
            color: white;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <header>
        <h1>Bienvenido a Mi Página Personal</h1>
        <nav>
            <a href="#sobre-mi">Sobre Mí</a>
            <a href="#proyectos">Proyectos</a>
            <a href="#contacto">Contacto</a>
        </nav>
    </header>
    <section id="sobre-mi" class="section">
        <h2>Sobre Mí</h2>
        <p>Hola, soy [Tu Nombre], un apasionado por el desarrollo web.</p>
    </section>
    <section id="proyectos" class="section">
        <h2>Mis Proyectos</h2>
        <p>Aquí algunos de mis proyectos recientes.</p>
    </section>
    <section id="contacto" class="section">
        <h2>Contacto</h2>
        <form onsubmit="return enviarFormulario()">
            <input type="text" id="nombre" placeholder="Tu Nombre" required>
            <input type="email" id="email" placeholder="Tu Email" required>
            <textarea id="mensaje" placeholder="Tu Mensaje" required></textarea>
            <button type="submit">Enviar</button>
        </form>
        <p id="respuesta"></p>
    </section>
    <script>
        function enviarFormulario() {
            let nombre = document.getElementById("nombre").value;
            let email = document.getElementById("email").value;
            let mensaje = document.getElementById("mensaje").value;
            document.getElementById("respuesta").innerText = `Gracias ${nombre}, pronto te responderé.`;
            return false;
        }
    </script>
</body>
</html>
