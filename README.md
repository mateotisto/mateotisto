<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>P&R (Peluche & Randy)</title>
    <style>
        /* Estilos previos */
    </style>
</head>
<body>
    <header>
        <h1>P&R (Peluche & Randy)</h1>
    </header>
    <nav>
        <a href="#">Inicio</a>
        <a href="#">Videos</a>
        <a href="#">Contacto</a>
        <a href="#">Sobre Nosotros</a>
    </nav>
    <button class="theme-toggle" onclick="toggleTheme()">Cambiar a Modo Oscuro</button>
    <div class="container">
        <div class="video-card">
            <!-- Contenido de videos existentes -->
        </div>
        <!-- Formulario para subir videos -->
        <div class="upload-form">
            <h2>Subir Video</h2>
            <form>
                <label for="video-url">URL del Video (YouTube, Vimeo, etc.):</label><br>
                <input type="url" id="video-url" name="video-url" required><br><br>
                <label for="video-description">Descripción:</label><br>
                <textarea id="video-description" name="video-description" rows="4" cols="50" required></textarea><br><br>
                <button type="submit">Subir Video</button>
            </form>
        </div>
    </div>
    <footer>
        <p>&copy; 2024 P&R (Peluche & Randy) - Todos los derechos reservados.</p>
    </footer>
    <script>
        /* Función de cambio de tema */
        function toggleTheme() {
            document.body.classList.toggle('dark-mode');
            const button = document.querySelector('.theme-toggle');
            if (document.body.classList.contains('dark-mode')) {
                button.textContent = 'Cambiar a Modo Claro';
            } else {
                button.textContent = 'Cambiar a Modo Oscuro';
            }
        }
    </script>
</body>
</html>

