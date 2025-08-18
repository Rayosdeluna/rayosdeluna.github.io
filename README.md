<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rayos de Luna | Bisutería</title>
  <style>
 
  body { font-family: Arial, sans-serif; margin: 0; padding: 0; }
    header { background: #f48b9a; padding: 15px; text-align: center; color: white; }
    nav { background: #ffd6e4; padding: 10px; text-align: center; }
    nav a { margin: 0 15px; text-decoration: none; color: #333; font-weight: bold; }
    section { padding: 30px; display: none; }
    section.active { display: block; }
    .producto { border: 1px solid #ccc; padding: 15px; margin: 10px; border-radius: 8px; }
    .boton { background: #f48b9a; color: white; padding: 10px; border: none; border-radius: 5px; cursor: pointer; }
    .formulario input, .formulario select { display: block; margin: 10px 0; padding: 8px; width: 100%; }
    footer { background: #f48b9a; color: white; text-align: center; padding: 15px; margin-top: 20px; }
    #rayito { position: fixed; bottom: 20px; right: 20px; background: #ffd6e4; border-radius: 50%; padding: 15px; cursor: pointer; box-shadow: 0 4px 6px rgba(0,0,0,0.2); }
    #rayitoMenu { display: none; position: fixed; bottom: 80px; right: 20px; background: white; border: 1px solid #ccc; border-radius: 10px; padding: 15px; width: 220px; }
    #rayitoMenu p { margin: 8px 0; cursor: pointer; color: #f48b9a; }
  </style>
</head>
<body>

  <header>
    <a href="https://imgbb.com/"><img src="https://i.ibb.co/dJmSGh63/logo-Rayos-de-luna.png" alt="logo-Rayos-de-luna" border="0"></a>
    <h1> Rayos de Luna </h1>
    <p>Bisutería hechas con amor desde Ecuador. Entregas a domicilio.</p>
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
  <section id="inicio">
    <h2>Bienvenidos a Rayos de Luna</h2>
    <p>Somos una marca ecuatoriana de bisutería exclusiva. Diseñamos piezas únicas para iluminar tus momentos especiales. Contamos con entregas a domicilio a nivel nacional.</p>
    <p>💖 Compra fácil, segura y sin complicaciones, desde la comodidad de tu casa.</p>
    <p>👉 Solo elige tu favorito, haz tu pedido ¡y nosotros lo llevamos directo a tu puerta! 🚚
    <p>📍Ecuador - Guayaquil</p>

  

  <!-- NOSOTROS -->
  <section id="nosotros">
    <h2>¿Quiénes Somos?</h2>
     <p>En Rayos de Luna somos marca d bisutería apasionada por crear puezas únicasque reflejan elegancia, estilo y personalidad. Cada una de nuestras piezas está diseñada pensando en ti, para que puedas  expresar tú esencia en cada momento especial. Nos caraterizamos por combinar calidad, creatividad y atención personalizada, ofrecemos no solo un producto, sino experiencias que ilumina tu día a día. Nuestra mision es  es acercarte a piezas que enamoran y te hagan sentir especial en cada ocación.</p>
    <h3>Misión</h3>
    <p>Brindar piezas únicas y elegantes que realzan la belleza y personalidad de cada cliente, ofreciendo una experiencia de compra segura, accesible y cercana, con atención personalizada que genera confianza y satisfacción.</p>
    <h3>Visión</h3>
    <p>Convertirnos en la marca de bisutería online preferida a nivel nacional, reconocida por la calidad de nuestros productos, la creatividad de nuestros diseños y la conexión emocional con nuestros clientes, inspirando momentos especiales y memorables.</p>
    <h3>Valores</h3>
    <ul>
      <p>Calidad:Nos comprometemos a ofrecer productos duraderos y bien elaborados.</p>
      <li>Creatividad: Cada pieza refleja originalidad y estilo.</li>
      <li>Confianza: Atención cercana y honesta en cada compra.</li>
      <li>Pasión: Amamos lo que hacemos y transmitimos esa pasión en nuestros productos.</li>
      <li>innovación: Buscamos siempre mejorar y sorprender a nuestros clientes con nuevas tendencias.</li>
    </ul>
  </section>

  <!-- PRODUCTOS -->
  <section id="productos">
    <h2>Nuestros Productos</h2>
    <div class="producto"> 
      <img src="https://i.ibb.co/HD1bwv3t/tu-imagen.jpg" alt="Descripción de la imagen" width="500">
      <h3>Combo Estrella ⭐</h3>
      <p>Incluye: un par de argollas</p>
      <p>Precio: $10</p>
      <button class="boton" onclick="mostrar('pedidos')">Comprar</button>
    </div>
    <div class="producto">
      <img src="https://i.ibb.co/7tM5jJ5K/imagen.jpg" alt="Descripción de la imagen" width="500"> 
      <h3>Combo Doble Estrella ⭐⭐</h3>
      <p>Incluye: un par de argollas + una pulsera</p>
      <p>Precio: $15</p>
      <button class="boton" onclick="mostrar('pedidos')">Comprar</button>
    </div>
    <div class="producto">
      <a href="https://imgbb.com/"><img src="https://i.ibb.co/1GvnrWB1/4.png" alt="4" border="0"></a> estelar
      <h3>Combo Estelar 🌟</h3>
      <p>Incluye: un juego de pulseras</p>
      <p>Precio: $13</p>
      <button class="boton" onclick="mostrar('pedidos')">Comprar</button>
    </div>
    <div class="producto">
      <img src="https://i.ibb.co/C3qcfPkk/tu-imagen.jpg" alt="Descripción de la imagen" width="500">
      <h3>Colección Aura ✨</h3>
      <p>Incluye: un par de argollas únicas</p>
      <p>Precio: $10</p>
      <button class="boton" onclick="mostrar('pedidos')">Comprar</button>
    </div>
  </section>

  <!-- PEDIDOS -->
  <section id="pedidos" class=active>
    <h2>Formulario de Pedido</h2>
    <form class="formulario" onsubmit="procesarPedido(event)">
      <label>Nombre Completo:</label>
      <input type="text" required>
      <label>Correo:</label>
      <input type="email" required>
      <label>Producto:</label>
      <select id="producto" onchange="actualizarTotal()">
        <option value="15">Combo Estrella - $10</option>
        <option value="25">Combo Doble Estrella - $15</option>
        <option value="20">Combo Estelar - $13</option>
        <option value="18">Colección Aura - $10</option>
      </select>
      <label>Cantidad:</label>
      <input type="number" id="cantidad" value="1" min="1" onchange="actualizarTotal()">
      <p><strong>Total: $<span id="total"></span></strong></p>
      <label>Método de Pago:</label>
      <select required>
        <option>Transferencia</option>
        <option>Efectivo</option>
      </select>
      <button class="boton" type="submit">Generar Pedido</button>
    </form>
    <h3>Estado del Pedido</h3>
    <ul>
      <li>Por aprobar</li>
      <li>Por preparar</li>
      <li>Por enviar</li>
      <li>En tránsito</li>
      <li>Entregado</li>
      <li>Anulado</li>
    </ul>
  </section>

  <!-- POLÍTICAS -->
  <section id="politicas">
    <h2>Políticas</h2>
    <h3>Privacidad</h3>
    <p>Cuidamos tu información personal con total responsabilidad. Los datos se usan solo para procesar pedidos y promociones.</p>
    <h3>Pedidos y Compras</h3>
    <p>Todos los pedidos se confirman por WhatsApp. Métodos de pago: transferencia o efectivo. Tiempo de entrega: 3 días hábiles.</p>
    <h3>Devoluciones y Cambios</h3>
    <p>Aceptamos devoluciones solo por defectos de fabricación, hasta 48h después de la entrega.</p>
  </section>

  <!-- CONTACTO -->
  <section id="contacto">
    <h2>Contacto</h2>
    <p>📧 Correo: rayo_de_luna_13@hotmail.com</p>
    <p>📱 Instagram & Facebook: @Rayos_de_luna_13</p>
    <p>🕒 Horario de atención: Lun-Vie 9AM - 4PM</p>
  </section>

  <!-- FAQ -->
  <section id="faq" 
    <h2>Preguntas Frecuentes</h2>
    <p><strong>¿Cuáles son los combos?</strong> Combo Estrella, Doble Estrella, Estelar y la colección Aura.</p>
    <p><strong>¿Cómo puedo pagar?</strong> Transferencia o efectivo.</p>
    <p><strong>¿Horario de atención?</strong> Lun-Vie 9AM - 4PM</p>
  </section>

  <footer>
    <p>&copy; 2025 Rayos de Luna - Todos los derechos reservados.</p>
  </footer>
 <!-- Botón flotante -->
  <button id="chat-btn">💬</button>

  <!-- Caja del chat -->
  <div id="chat-box">
    <div id="chat-header">Asistente Rayito</div>
    <div id="chat-messages">
      <div class="msg bot">¡Hola! Soy Rayito 🌙<br> ¿En qué puedo ayudarte?</div>
      <div>
        <span class="option-btn" onclick="sendOption('Ver combos')">Ver combos</span>
        <span class="option-btn" onclick="sendOption('Horario de atención')">Horario de atención</span>
        <span class="option-btn" onclick="sendOption('Hablar por WhatsApp')">Hablar por WhatsApp</span>
      </div>
    </div>
    <div id="chat-input">
      <input type="text" id="user-input" placeholder="Escribe un mensaje...">
      <button id="send-btn">➤</button>
    </div>
  </div>


  <script>
    function mostrar(id) {
      document.querySelectorAll('section').forEach(sec => sec.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }

    function actualizarTotal() {
      let precio = parseFloat(document.getElementById('producto').value);
      let cantidad = parseInt(document.getElementById('cantidad').value);
      document.getElementById('total').innerText = precio * cantidad;
    }

    function procesarPedido(e) {
      e.preventDefault();
      alert("✅ Pedido generado con éxito. Te confirmaremos por WhatsApp.");
    }

    document.getElementById('rayito').addEventListener('click', () => {
      let menu = document.getElementById('rayitoMenu');
      menu.style.display = menu.style.display === "block" ? "none" : "block";
    });
  </script>

</body>
</html>

