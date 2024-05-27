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
            <!-- Contenido del video -->
        </div>
        <!-- Sección de comentarios generales -->
        <div class="comments-section">
            <h2>Comentarios Generales</h2>
            <!-- Formulario para agregar un comentario -->
            <form action="comentarios.php" method="post">
                <label for="nombre">Nombre:</label><br>
                <input type="text" id="nombre" name="nombre" required><br><br>
                <label for="comentario">Comentario:</label><br>
                <textarea id="comentario" name="comentario" rows="4" cols="50" required></textarea><br><br>
                <button type="submit">Enviar Comentario</button>
            </form>

            <!-- Mostrar comentarios existentes -->
            <div class="comment">
                <strong>Usuario 1:</strong> Este es un comentario existente.
            </div>
            <div class="comment">
                <strong>Usuario 2:</strong> Este es otro comentario existente.
            </div>
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


