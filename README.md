<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>LocalWeb</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #f5f5f5;
      color: #333;
    }
    header {
      background: #2ecc71;
      color: white;
      padding: 20px;
      text-align: center;
    }
    nav {
      display: flex;
      justify-content: center;
      gap: 30px;
      background: #27ae60;
      padding: 10px;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: 600;
    }
    section {
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
    }
    .pack {
      background: white;
      border-radius: 12px;
      padding: 20px;
      margin: 20px 0;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    .pack button {
      background: #2ecc71;
      color: white;
      border: none;
      padding: 10px 20px;
      margin-top: 10px;
      border-radius: 8px;
      cursor: pointer;
      font-weight: 600;
    }
    .formulario-compra {
      display: none;
      margin-top: 20px;
    }
    .formulario-compra input,
    .formulario-compra textarea {
      width: 100%;
      margin-bottom: 10px;
      padding: 8px;
      border-radius: 6px;
      border: 1px solid #ccc;
    }
    .formulario-compra button {
      background: #27ae60;
    }
    footer {
      background: #2ecc71;
      color: white;
      text-align: center;
      padding: 20px;
    }
  </style>
  <script>
    function mostrarFormulario(id) {
      const formulario = document.getElementById(id);
      formulario.style.display = formulario.style.display === 'none' ? 'block' : 'none';
    }
  </script>
</head>
<body>
  <header>
    <h1>LocalWeb</h1>
    <p>Tu web. Tu barrio. Tu momento.</p>
  </header>

  <nav>
    <a href="#inicio">Inicio</a>
    <a href="#servicios">Servicios</a>
    <a href="#sobre">Sobre mí</a>
    <a href="#contacto">Contacto</a>
  </nav>

  <section id="inicio">
    <h2>Bienvenido a LocalWeb</h2>
    <p>Ayudamos a negocios locales a tener una presencia online profesional, moderna y eficaz.</p>
  </section>

  <section id="servicios">
    <h2>Servicios</h2>

    <div class="pack">
      <h3>Pack Básico - 250 €</h3>
      <p>Web de hasta 5 secciones, diseño responsive, WhatsApp, Google Maps y formulario de contacto.</p>
      <button onclick="mostrarFormulario('formulario1')">Comprar</button>
      <div id="formulario1" class="formulario-compra">
        <h4>Formulario de compra - Pack Básico</h4>
        <input type="text" placeholder="Tu nombre" required />
        <input type="email" placeholder="Tu correo electrónico" required />
        <textarea placeholder="Información adicional o dudas (opcional)"></textarea>
        <button>Enviar pedido</button>
      </div>
    </div>

    <div class="pack">
      <h3>Pack Avanzado - 450 €</h3>
      <p>Incluye todo lo del Pack Básico + sistema de reservas o tienda online, pagos y secciones extra.</p>
      <button onclick="mostrarFormulario('formulario2')">Comprar</button>
      <div id="formulario2" class="formulario-compra">
        <h4>Formulario de compra - Pack Avanzado</h4>
        <input type="text" placeholder="Tu nombre" required />
        <input type="email" placeholder="Tu correo electrónico" required />
        <textarea placeholder="Información adicional o dudas (opcional)"></textarea>
        <button>Enviar pedido</button>
      </div>
    </div>

    <div class="pack">
      <h3>Mantenimiento Mensual - 25 €/mes</h3>
      <p>Hosting seguro, soporte, cambios menores y actualizaciones.</p>
      <button onclick="mostrarFormulario('formulario3')">Comprar</button>
      <div id="formulario3" class="formulario-compra">
        <h4>Formulario de compra - Mantenimiento Mensual</h4>
        <input type="text" placeholder="Tu nombre" required />
        <input type="email" placeholder="Tu correo electrónico" required />
        <textarea placeholder="Información adicional o dudas (opcional)"></textarea>
        <button>Enviar pedido</button>
      </div>
    </div>
  </section>

  <section id="sobre">
    <h2>Sobre mí</h2>
    <p>Soy un diseñador web especializado en ayudar a negocios locales a digitalizarse. Trabajo de forma cercana, rápida y profesional.</p>
  </section>

  <section id="contacto">
    <h2>Contacto</h2>
    <p><strong>WhatsApp:</strong> 667 92 53 18</p>
    <p><strong>Email:</strong> localwebes@proton.me</p>
    <p><strong>Instagram:</strong> @lild1ablo</p>
  </section>

  <footer>
    <p>&copy; 2025 LocalWeb · Todos los derechos reservados</p>
  </footer>
</body>
</html>
