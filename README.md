<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Mi Notube Mejorado</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    /* Reset básico */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: Arial, sans-serif;
      background: #f5f5f5;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }
    header {
      background: #333;
      color: #fff;
      padding: 15px;
      text-align: center;
    }
    .container {
      flex: 1;
      display: flex;
      flex-direction: row;
    }
    /* Sección de descargas a la izquierda */
    .sidebar-left {
      background: #fff;
      width: 300px;
      padding: 20px;
      border-right: 1px solid #ddd;
    }
    /* Contenido principal */
    .main-content {
      flex: 1;
      padding: 20px;
    }
    /* Panel de anuncios a la derecha */
    .sidebar-right {
      background: #fff;
      width: 200px;
      padding: 20px;
      border-left: 1px solid #ddd;
    }
    footer {
      background: #333;
      color: #fff;
      text-align: center;
      padding: 10px;
    }
    /* Estilos para el formulario de descargas */
    .download-form {
      margin-bottom: 20px;
    }
    .download-form label {
      display: block;
      margin-bottom: 5px;
      font-weight: bold;
    }
    .download-form input[type="text"] {
      width: 100%;
      padding: 10px;
      margin-bottom: 10px;
      border: 1px solid #ccc;
    }
    .download-form button {
      padding: 10px 20px;
      background: #007BFF;
      border: none;
      color: #fff;
      cursor: pointer;
    }
    .download-form button:hover {
      background: #0056b3;
    }
  </style>
</head>
<body>
  <header>
    <h1>Mi Notube Mejorado</h1>
  </header>
  <div class="container">
    <!-- Sección izquierda: Descargas -->
    <div class="sidebar-left">
      <h2>Descargas</h2>
      <form class="download-form">
        <label for="video-url">URL del video:</label>
        <input type="text" id="video-url" placeholder="Pega la URL aquí">
        <button type="submit">Descargar</button>
      </form>
      <p>Instrucciones: Ingresa la URL del video para iniciar la descarga.</p>
    </div>
    <!-- Contenido principal -->
    <div class="main-content">
      <h2>Contenido Principal</h2>
      <p>Aquí irá el contenido principal, como un reproductor de video o resultados de búsqueda.</p>
      <!-- Puedes integrar más funcionalidades dinámicas aquí -->
    </div>
    <!-- Panel derecho: Anuncios -->
    <div class="sidebar-right">
      <h2>Anuncios</h2>
      <p>Aquí se mostrarán los anuncios.</p>
      <!-- Inserta el código de tus anuncios o widgets publicitarios -->
    </div>
  </div>
  <footer>
    <p>&copy; 2025 Mi Notube Mejorado. Todos los derechos reservados.</p>
  </footer>
  <script>
    // Lógica básica para el formulario de descargas
    document.querySelector('.download-form').addEventListener('submit', function(e) {
      e.preventDefault();
      var videoUrl = document.getElementById('video-url').value;
      if(videoUrl) {
        alert('Iniciando descarga para: ' + videoUrl);
        // Aquí puedes integrar la lógica para gestionar la descarga o redirigir a una API de conversión
      } else {
        alert('Por favor, ingresa una URL.');
      }
    });
  </script>
</body>
</html>
