
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rayos de Luna | Ecuador</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; }
    header { background: #f48b9a; color: white; padding: 15px; text-align: center; }
    nav { background: #ffd6e4; padding: 10px; text-align: center; }
    nav a { margin: 0 15px; text-decoration: none; color: #333; font-weight: bold; }
    section { padding: 20px; }
    .producto { border: 1px solid #ccc; border-radius: 10px; padding: 15px; margin: 15px 0; }
    button { background: #f48b9a; color: white; padding: 10px 15px; border: none; border-radius: 8px; cursor: pointer; }
    button:hover { background: #e36b81; }
    footer { background: #333; color: white; text-align: center; padding: 15px; margin-top: 20px; }
    .oculto { display: none; }
    .chatbox { position: fixed; bottom: 20px; right: 20px; background: #ffd6e4; border-radius: 15px; padding: 15px; width: 250px; box-shadow: 0 4px 6px rgba(0,0,0,0.2); }
    .chatbox h4 { margin: 0; color: #333; }
    .faq { margin-top: 10px; }
    .faq h3 { margin-bottom: 5px; }
  </style>
</head>
<body>
  <header>
      <a href="https://imgbb.com/"><img src="https://i.ibb.co/dJmSGh63/logo-Rayos-de-luna.png" alt="logo-Rayos-de-luna" border="0"></a>
    <h1>Rayos de Luna ✨</h1>
    <p>Desde Ecuador, entregamos con amor directo a tu domicilio</p>
  </header>

  <nav>
    <a href="#inicio">Inicio</a>
    <a href="#quienes">Quiénes Somos</a>
    <a href="#productos">Productos</a>
    <a href="#pedidos">Pedidos</a>
    <a href="#politicas">Políticas</a>
    <a href="#contacto">Contacto</a>
    <a href="#faq">Preguntas Frecuentes</a
  </nav>
  

  <!-- INICIO -->
  <section id="inicio">
    <h2>Bienvenidos</h2>
    <p>Somos Rayos de Luna, una marca ecuatoriana que busca resaltar tu estilo con piezas únicas y elegantes. Ofrecemos entregas rápidas y seguras en todo el país.</p>
  </section>

  <!-- QUIÉNES SOMOS -->
  <section id="quienes">
    <h2>Quiénes Somos</h2>
    <p><strong>Misión:</strong> Ofrecer joyas de calidad que inspiren confianza y elegancia en cada persona.</p>
    <p><strong>Visión:</strong> Ser la marca ecuatoriana de joyas más reconocida por su diseño y cercanía con el cliente.</p>
    <p><strong>Valores:</strong> Confianza, Responsabilidad y Pasión por el detalle.</p>
  </section>

  <!-- PRODUCTOS -->
  <section id="productos">
    <h2>Nuestros Productos</h2>
    <div class="producto">
        <img src="https://i.ibb.co/HD1bwv3t/tu-imagen.jpg" alt="Descripción de la imagen" width="500"> 
      <h3>Combo Estrella</h3>
      <p>Un par de argollas.</p>
      <button onclick="agregarPedido('Combo Estrella', $10)">Comprar</button>
    </div>
    <div class="producto">
      <img src="https://i.ibb.co/7tM5jJ5K/imagen.jpg" alt="Descripción de la imagen" width="500"> 
      <h3>Combo Doble Estrella</h3>
      <p>Un par de argollas + una pulsera.</p>
      <button onclick="agregarPedido('Combo Doble Estrella', $15)">Comprar</button>
    </div>
    <div class="producto">
      <a href="https://imgbb.com/"><img src="https://i.ibb.co/1GvnrWB1/4.png" alt="4" border="0"></a>
      <h3>Combo Estelar</h3>
      <p>Un juego de pulseras.</p>
      <button onclick="agregarPedido('Combo Estelar', $13)">Comprar</button>
    </div>
    <div class="producto">
      <img src="https://i.ibb.co/C3qcfPkk/tu-imagen.jpg" alt="Descripción de la imagen" width="500">
      <h3>Colección Aura</h3>
      <p>Un par de argollas únicas.</p>
      <button onclick="agregarPedido('Colección Aura', $10)">Comprar</button>
    </div>
  </section>

  <!-- PEDIDOS -->
  <section id="pedidos">
    <h2>Realiza tu Pedido</h2>
    <form id="formPedido">
      <label>Nombre Completo:</label><br>
      <input type="text" id="nombre" required><br><br>

  <label>Teléfono:</label><br>
      <input type="tel" id="telefono" required><br><br>
      <label>Dirección:</label><br>
      <textarea id="direccion" required></textarea><br><br>

<label>Método de pago:</label><br>
      <select id="pago">
        <option value="Transferencia">Transferencia</option>
        <option value="Efectivo">Efectivo</option>
      </select><br><br>
      <h3>Resumen de compra:</h3>
      <ul id="listaPedidos"></ul>
      <p><strong>Total: $<span id="total">0</span></strong></p>

  <button type="submit">Confirmar Pedido</button>
    </form>

   <div id="seguimiento" class="oculto">
      <h3>Estado de tu pedido:</h3>
      <p id="estadoPedido">Por aprobar ✅</p>
    </div>
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
    <p><strong>Correo:</strong> rayo_de_luna_13@hotmail.com</p>
    <p><strong>Instagram & Facebook:</strong> @Rayos_de_luna_13</p>
  </section>
 <!-- PREGUNTAS FRECUENTES -->
  <section id="faq">
    <h2>Preguntas Frecuentes</h2>
    <div class="faq">
      <h3>¿Cuáles son los combos?</h3>
      <p>Combo Estrella, Combo Doble Estrella, Combo Estelar y la Colección Aura.</p>
    </div>
    <div class="faq">
      <h3>¿Cómo puedo pagar?</h3>
      <p>Aceptamos transferencia o efectivo.</p>
    </div>
    <div class="faq">
      <h3>¿Horario de atención?</h3>
      <p>Lunes a Viernes de 9AM a 4PM.</p>
    </div>
  </section>
  <!-- ASISTENTE VIRTUAL -->
  <div class="chatbox" id="chat">
    <h4>⚡ Rayito - Tu asistente virtual</h4>
    <p>Hola, soy Rayito. ¿Cómo te puedo ayudar?</p>
    <ul>
      <li><a href="#productos">Ver Combos</a></li>
      <li><a href="#faq">Preguntas Frecuentes</a></li>
      <li><a href="#contacto">Contáctanos</a></li>
    </ul>
    <p>O escríbenos directamente por WhatsApp 📲</p>
  </div>

  <footer>
    <p>&copy; 2025 Rayos de Luna | Ecuador</p>
 script>
    let pedidos = [];
    let total = 0;

  function agregarPedido(producto, precio) {
      pedidos.push({producto, precio});
      total += precio;
      mostrarPedidos();
      alert(producto + " agregado al carrito ✅");
    }

  function mostrarPedidos() {
      let lista = document.getElementById("listaPedidos");
      lista.innerHTML = "";
      pedidos.forEach(p => {
        let li = document.createElement("li");
        li.textContent = p.producto + " - $" + p.precio;
        lista.appendChild(li);
      });
      document.getElementById("total").textContent = total;
    }

  document.getElementById("formPedido").addEventListener("submit", function(e) {
      e.preventDefault();
      document.getElementById("seguimiento").classList.remove("oculto");
      document.getElementById("estadoPedido").textContent = "Por aprobar ✅";
      alert("Tu pedido ha sido registrado. Te contactaremos por WhatsApp para confirmarlo.");
    });
