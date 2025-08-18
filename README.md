<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rayos de Luna | Bisuterías</title>
  <style>
    body {font-family: Arial, sans-serif; margin:0; padding:0; background:#fffafc;}
    header {background:#f48b9a; color:white; padding:15px; text-align:center;}
    nav {display:flex; justify-content:center; background:#ffd6e4;}
    nav a {padding:14px 20px; text-decoration:none; color:#333; font-weight:bold;}
    nav a:hover {background:#f48b9a; color:white;}
    section {padding:40px; display:none;}
    section.active {display:block;}
    h2 {color:#f48b9a;}
    .producto {border:1px solid #ffd6e4; border-radius:10px; padding:20px; margin:20px 0;}
    button {background:#f48b9a; color:white; padding:10px 15px; border:none; border-radius:10px; cursor:pointer;}
    button:hover {background:#ff5c7a;}
    footer {background:#ffd6e4; text-align:center; padding:20px; margin-top:40px;}

    /* Asistente virtual */
    #asistente {position:fixed; bottom:20px; right:20px; background:#f48b9a; color:white; padding:15px; border-radius:50%; cursor:pointer; box-shadow:0 4px 6px rgba(0,0,0,0.2);} 
    #chatbox {display:none; position:fixed; bottom:80px; right:20px; width:300px; background:white; border:1px solid #ccc; border-radius:10px; box-shadow:0 4px 6px rgba(0,0,0,0.2);}
    #chatbox header {background:#f48b9a; color:white; padding:10px; border-radius:10px 10px 0 0;}
    #chatbox div {padding:10px;}
  </style>
</head>
<body>
  <header>
    <a href="https://imgbb.com/"><img src="https://i.ibb.co/dJmSGh63/logo-Rayos-de-luna.png" alt="logo-Rayos-de-luna" border="0"></a>
    <h1>✨ Rayos de Luna ✨</h1>
    <p>Joyas únicas hechas en Ecuador, con entregas a domicilio</p>
  </header>

  <nav>
    <a href="#" onclick="mostrar('inicio')">Inicio</a>
    <a href="#" onclick="mostrar('nosotros')">Nosotros</a>
    <a href="#" onclick="mostrar('productos')">Productos</a>
    <a href="#" onclick="mostrar('pedidos')">Pedidos</a>
    <a href="#" onclick="mostrar('politicas')">Políticas</a>
    <a href="#" onclick="mostrar('contacto')">Contacto</a>
    <a href="#" onclick="mostrar('faq')">Preguntas Frecuentes</a>
  </nav>

  <!-- INICIO -->
  <section id="inicio" class="active">
    <h2>Bienvenidos a Rayos de Luna</h2>
    <p>Somos una marca ecuatoriana dedicada a la creación de joyas exclusivas. Contamos con entregas a domicilio en todo el país ✨.</p>
    <p>Ofrecemos piezas únicas y exclusivas para destacar tu estilo.</p>
    <p>💖 Compra fácil, segura y sin complicaciones, desde la comodidad de tu casa.</p>
    <p>👉 Solo elige tu favorito, haz tu pedido ¡y nosotros lo llevamos directo a tu puerta! 🚚
    <p>📍Ecuador - Guayaquil</p>

  </section>

  <!-- NOSOTROS -->
  <section id="nosotros">
    <h2>Quiénes Somos</h2>
    <p><strong>Misión:</strong> Diseñar joyas que iluminen cada momento especial de nuestros clientes.</p>
    <p><strong>Visión:</strong> Ser la marca de joyería preferida en Ecuador por calidad y exclusividad.</p>
    <p><strong>Valores:</strong> Confianza, responsabilidad y creatividad.</p>
  </section>

  <!-- PRODUCTOS -->
  <section id="productos">
    <h2>Nuestros Productos</h2>
    <div class="producto">
      <h3>⭐ Combo Estrella</h3>
      <p>Un par de argollas.</p>
      <button onclick="mostrar('pedidos')">Comprar</button>
    </div>
    <div class="producto">
      <h3>⭐⭐ Combo Doble Estrella</h3>
      <p>Un par de argollas + una pulsera.</p>
      <button onclick="mostrar('pedidos')">Comprar</button>
    </div>
    <div class="producto">
      <h3>🌟 Combo Estelar</h3>
      <p>Un juego de pulseras.</p>
      <button onclick="mostrar('pedidos')">Comprar</button>
    </div>
    <div class="producto">
      <h3>✨ Colección Aura</h3>
      <p>Un par de argollas únicas.</p>
      <button onclick="mostrar('pedidos')">Comprar</button>
    </div>
  </section>

  <!-- PEDIDOS -->
  <section id="pedidos">
    <h2>Realiza tu Pedido</h2>
    <form id="formPedido">
      <label>Nombre:</label><br>
      <input type="text" required><br><br>
      <label>Producto:</label><br>
      <select id="producto">
        <option value="Combo Estrella - $10">Combo Estrella - $10</option>
        <option value="Combo Doble Estrella - $18">Combo Doble Estrella - $18</option>
        <option value="Combo Estelar - $15">Combo Estelar - $15</option>
        <option value="Colección Aura - $12">Colección Aura - $12</option>
      </select><br><br>
      <label>Método de pago:</label><br>
      <select>
        <option>Transferencia</option>
        <option>Efectivo</option>
      </select><br><br>
      <button type="submit">Generar Pedido</button>
    </form>
    <p id="resPedido"></p>
  </section>

  <!-- POLÍTICAS -->
  <section id="politicas">
    <h2>Políticas</h2>
    <h3>Privacidad</h3>
    <p>Cuidamos tu información personal con total responsabilidad. Los datos se usan solo para procesar pedidos y promociones.</p>

  <h3>Pedidos y Compras</h3>
    <p>Todos los pedidos se confirman por WhatsApp.<br> Métodos de pago: transferencia o efectivo.<br> Tiempo de entrega: 3 días hábiles.</p>

   <h3>Devoluciones y Cambios</h3>
    <p>Aceptamos devoluciones solo por defectos de fabricación, hasta 48h después de la entrega.</p>
  </section>

  <!-- CONTACTO -->
  <section id="contacto">
    <h2>Contacto</h2>
    <p>Correo: <a href="mailto:rayo_de_luna_13@hotmail.com">rayo_de_luna_13@hotmail.com</a></p>
    <p>Instagram & Facebook: @Rayos_de_luna_13</p>
  </section>

  <!-- PREGUNTAS FRECUENTES -->
  <section id="faq">
    <h2>Preguntas Frecuentes</h2>
    <p><strong>¿Cuáles son los combos?</strong> Combo Estrella, Doble Estrella, Estelar y la Colección Aura.</p>
    <p><strong>¿Cómo puedo pagar?</strong> Transferencia o efectivo.</p>
    <p><strong>¿Horario de atención?</strong> Lun-Vie 9AM - 4PM.</p>
  </section>

  <footer>
    <p>© 2025 Rayos de Luna. Todos los derechos reservados.</p>
  </footer>

  <!-- Asistente Virtual Rayito -->
  <div id="asistente" onclick="abrirChat()">⚡</div>
  <div id="chatbox">
    <header>Rayito ⚡</header>
    <div>
      <p>¡Hola! Soy Rayito, tu asistente virtual 🌙<br> ¿En qué puedo ayudarte?</p>
      <ul>
        <li><a href="#" onclick="mostrar('productos')">Ver Combos</a></li>
        <li><a href="#" onclick="mostrar('faq')">Preguntas Frecuentes</a></li>
        <li><a href="https://wa.me/593995372875" target="_blank">WhatsApp</a></li>
        <li>Horario de atención: 9AM - 4PM</li>
      </ul>
    </div>
  </div>

  <script>
    function mostrar(id){
      document.querySelectorAll('section').forEach(sec=>sec.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }

    function abrirChat(){
      const chat = document.getElementById('chatbox');
      chat.style.display = chat.style.display === 'block' ? 'none' : 'block';
    }

    document.getElementById("formPedido").addEventListener("submit", function(e){
      e.preventDefault();
      let producto = document.getElementById("producto").value;
      document.getElementById("resPedido").innerText = "✅ Pedido generado: " + producto + ". Estado: Por aprobar.";
    });
  </script>
</body>
</html>
