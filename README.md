<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blog de sh4d0wk33n</title>
    <style>
        body {
            font-family: 'Georgia', serif;
            background-color: #1a1a1a;
            color: #f0f0f0;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        header {
            background-color: #4b0082;
            padding: 20px;
            text-align: center;
            width: 100%;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
            color: #f0f0f0;
        }
        nav {
            text-align: center;
            margin-top: 20px;
        }
        nav a {
            color: #f0f0f0;
            text-decoration: none;
            margin: 0 15px;
            font-size: 1.2em;
        }
        nav a:hover {
            text-decoration: underline;
        }
        .bio {
            padding: 40px 20px;
            text-align: center;
        }
        .bio h2 {
            font-size: 2em;
            color: #4b0082;
        }
        .bio p {
            font-size: 1.2em;
            max-width: 800px;
            margin: 0 auto;
        }
        .container {
            display: flex;
            justify-content: center;
            align-items: flex-start;
            margin: 20px;
            width: 100%;
            max-width: 1200px;
        }
        .main-content {
            flex: 3;
            padding: 20px;
            background-color: #2e2e2e;
            border-radius: 8px;
            margin-right: 20px;
        }
        .comments-section {
            flex: 1;
            padding: 20px;
            background-color: #333;
            border-radius: 8px;
            color: #f0f0f0;
        }
        footer {
            background-color: #333;
            color: #f0f0f0;
            padding: 20px;
            text-align: center;
            width: 100%;
        }
        footer a {
            color: #f0f0f0;
            text-decoration: none;
            margin: 0 10px;
        }
        footer a:hover {
            text-decoration: underline;
        }
        .menu {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            text-align: center;
            background-color: #4b0082;
            color: #f0f0f0;
            width: 100%;
        }
        .menu h1 {
            font-size: 3em;
            margin: 0;
        }
        .menu p {
            font-size: 1.5em;
            margin: 10px 0;
        }
        .menu button {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 1.2em;
            background-color: #f0f0f0;
            color: #4b0082;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .menu button:hover {
            background-color: #ddd;
        }
        #contact-info {
            padding: 40px 20px;
            text-align: center;
        }
        #contact-info h1 {
            font-size: 2.5em;
            color: #f0f0f0;
        }
    </style>
    <script>
        function enterSite() {
            document.getElementById('menu').style.display = 'none';
            document.getElementById('main-content').style.display = 'block';
        }
        function goToContact() {
            document.getElementById('menu').style.display = 'none';
            document.getElementById('main-content').style.display = 'none';
            document.getElementById('contact-info').style.display = 'block';
        }
    </script>
</head>
<body>
    <div id="menu" class="menu">
        <h1>sh4d0wk33n</h1>
        <p>*Simpático usuario de discord nacido en argentina*</p>
        <button onclick="enterSite()">Entrar al sitio</button>
    </div>

    <div id="main-content" style="display:none;">
        <header>
            <h1>Blog de sh4d0wk33n</h1>
        </header>

        <nav>
            <a href="#bio">Biografía</a>
            <a href="#diario">Mi día a día</a>
            <a href="javascript:void(0)" onclick="goToContact()">Contacto</a>
        </nav>

        <section class="bio" id="bio">
            <h2>Sobre Mí</h2>
            <p>
                ¡HOLA! Soy sh4d0wk33n, esta página está en desarrollo.
            </p>
        </section>

        <div class="container">
            <div class="main-content" id="diario">
                <h2>Mi día a día</h2>
                <p>Aquí puedes compartir tus pensamientos, experiencias, y todo lo que quieras sobre tu día a día. Este espacio está listo para tus publicaciones.</p>
            </div>
            <div class="comments-section">
                <h3>Comentarios</h3>
                <p>Deja tus comentarios aquí:</p>
                <textarea rows="5" cols="30" placeholder="Escribe tu comentario..."></textarea>
                <br>
                <button type="button">Enviar</button>
            </div>
        </div>

        <footer id="contacto">
            <p>Encuéntrame en:</p>
            <a href="https://x.com/dark_light976" target="_blank">Twitter</a> |
            <a href="https://www.instagram.com/sh4d0wk33n/" target="_blank">Instagram</a>
        </footer>
    </div>

    <div id="contact-info" style="display:none;">
        <h1>DISCORD: x_el_shadow_x</h1>
    </div>
</body>
</html>
