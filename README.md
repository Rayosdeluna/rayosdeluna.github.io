<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rayos de Luna | Piezas Exclusivas</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #fff;
      color: #333;
    }
    header {
      background: #fff;
      padding: 15px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 2px solid #ffd6e4;
    }
    header img {
      height: 60px;
    }
    nav {
      display: flex;
      gap: 15px;
    }
    nav a {
      text-decoration: none;
      color: #333;
      font-weight: bold;
      padding: 8px 12px;
      border-radius: 8px;
      transition: background 0.3s;
    }
    nav a:hover, nav a.active {
      background: ##f48b9a;
    }
    #carrito-btn {
      background: #ffd6e4;
      border: none;
      padding: 10px;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
    }
    section {
      display: none;
      padding: 30px;
    }
    section.active {
      display: block;
    }
    .rectangulo {
      background: #ffd6e4;
      border: 2px solid #ffd6e4;
      border-radius: 12px;
      padding: 20px;
      margin: 15px 0;
      box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
    }
    .productos {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
    }
    .producto {
      background: #fff;
      border: 1px solid #ffd6e4;
      border-radius: 12px;
      padding: 15px;
      text-align: center;
    }
    .producto img {
      max-width: 100%;
      border-radius: 8px;
    }
    .producto button {
      margin-top: 10px;
      padding: 8px 12px;
      background: #ffd6e4;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
    }
    #carrito {
      position: fixed;
      top: 80px;
      right: 20px;
      width: 300px;
      background: #fff;
      border: 2px solid #ffd6e4;
      border-radius: 12px;
      padding: 15px;
      display: none;
      box-shadow: 2px 2px 10px rgba(0,0,0,0.2);
      z-index: 1000;
    }
    #carrito h3 {
      margin-top: 0;
      color: #333;
    }
    #carrito ul {
      list-style: none;
      padding: 0;
    }
    #carrito li {
      margin: 5px 0;
      font-size: 14px;
    }
    #carrito button {
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      background: #f48b9a;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 15px;
    }
    table, th, td {
      border: 1px solid #f48b9a;
    }
    th, td {
      padding: 10px;
      text-align: center;
    }
    .nosotros-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
    }
    .nosotros-box {
      background: #ffd6e4;
      border: 2px solid #fFF;
      border-radius: 12px;
      padding: 15px;
      text-align: center;
      box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
    }
    form input {
      width: 100%;
      padding: 8px;
      margin: 8px 0;
      border: 1px solid #f48b9a;
      border-radius: 8px;
    }
  </style>
</head>
<body>

  <header>
    <a href="https://ibb.co/vC6yGSm3"><img src="https://i.ibb.co/vC6yGSm3/logo-Rayos-de-luna.png" alt="logo-Rayos-de-luna" border="0"></a>
    <nav>
      <a href="#inicio" class="active">Inicio</a>
      <a href="#nosotros">Nosotros</a>
      <a href="#productos">Productos</a>
      <a href="#pedidos">Pedidos</a>
      <a href="#politicas">Políticas</a>
      <a href="#contacto">Contacto</a>
      <a href="#faq">FAQ</a>
    </nav>
    <button id="carrito-btn">🛒  (<span id="carrito-count">0</span>)</button>
  </header>

  <!-- Inicio -->
  <section id="inicio" class="active">
    <div class="rectangulo">
      <h2>Bienvenidos a Rayos de Luna</h2>
      <p>Ofrecemos joyas únicas y exclusivas para destacar tu estilo.</p>
      <p>Aquí cada detalle está pensado para ti. Encuentra productos únicos, de la mejor calidad y a precios que se ajustan a lo que buscas.</p>
      <p>💖 Compra fácil, segura y sin complicaciones, desde la comodidad de tu casa.</p>
      <p>👉 Solo elige tu favorito, haz tu pedido ¡y nosotros lo llevamos directo a tu puerta! 🚚✨</p>
     <a href="https://imgbb.com/"><img src="https://i.ibb.co/hnQHVrm/El-texto-del-p-rrafo-1.png" alt="El-texto-del-p-rrafo-1" border="0"></a>
    </div>
  </section>

  <!-- Nosotros -->
  <section id="nosotros">
    <h2>Nosotros</h2>
    <div class="nosotros-grid">
      <div class="nosotros-box">
        <h3>Quiénes Somos</h3>
        <p>Somos una marca que busca resaltar la belleza y autenticidad a través de joyas exclusivas.</p>
      </div>
      <div class="nosotros-box">
        <h3>Misión y Visión</h3>
        <p><b>Misión:</b> Brindar productos de calidad que transmitan elegancia y personalidad.</p>
        <p><b>Visión:</b> Ser reconocidos como líderes en joyería artesanal a nivel nacional.</p>
      </div>
      <div class="nosotros-box">
        <h3>Valores</h3>
        <p>Compromiso, pasión, exclusividad y confianza en cada pieza.</p>
      </div>
    </div>
  </section>

  <!-- Productos -->
  <section id="productos">
    <h2>Nuestros Productos</h2>
    <div class="productos">
      <div class="producto">
        <a href="https://ibb.co/VcJX7Bbp"><img src="https://i.ibb.co/VcJX7Bbp/combo-estrella.png" alt="combo-estrella" border="0"></a>
        <h3>Combo Estrella</h3>
        <p>$10.00</p>
        <button onclick="agregarAlCarrito('Combo Estrella', 10.00)">Añadir al carrito</button>
      </div>
      <div class="producto">
    <a href="https://ibb.co/Qv0jhTrb"><img src="https://i.ibb.co/Qv0jhTrb/2.png" alt="combo-doble-estrella" border="0"></a>
        <h3>Combo Doble Estrella</h3>
        <p>$15.00</p>
        <button onclick="agregarAlCarrito('Combo Doble Estrella', 15.00)">Añadir al carrito</button>
      </div>
      <div class="producto">
        <a href="https://ibb.co/CFsk15H"><img src="https://i.ibb.co/CFsk15H/4.png" alt="combo-estelar" border="0"></a>
        <h3>Combo Estelar</h3>
        <p>$13.00</p>
        <button onclick="agregarAlCarrito('Combo Estelar', 13.00)">Añadir al carrito</button>
      </div>
      <div class="producto">
        <a href="https://ibb.co/TxvNXqz0"><img src="https://i.ibb.co/TxvNXqz0/3.png" alt="colección-Aura" border="0"></a>
        <h3>Colección Aura</h3>
        <p>$10.00</p>
        <button onclick="agregarAlCarrito('Colección Aura', 10.00)">Añadir al carrito</button>
      </div>
      <div class="producto">
        <a href="https://ibb.co/Mxg1B057"><img src="https://i.ibb.co/Mxg1B057/Logo-Servicios-Profesionales-Moderno-Ilustrado-Rosado.png" alt="Logo-Servicios-Profesionales-Moderno-Ilustrado-Rosado" border="0"></a>
        <h3>Stella Bags</h3>
        <p>$20.00</p>
        <button onclick="agregarAlCarrito('Stella Bags', 20.00)">Añadir al carrito</button>
      </div>
    </div>
  </section>
<!-- Botón para catálogo Combos -->
<a href="https://www.canva.com/design/DAGvc_2MElU/qVUR8dLijXOCEZZoHOpr8A/view?utm_content=DAGvc_2MElU&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=hc23b1edaf1" target="_blank">
  <button style="background-color:#f48b9a; color:white; padding:10px 20px; border:none; border-radius:5px; cursor:pointer;">
    Ver catálogo Combos
  </button>
</a>
<!-- Botón para catálogo Stella Bags -->
<a href="https://www.canva.com/design/DAGw2zJWdKY/gUHcSTCXBe0ttl_0_bYkag/view?utm_content=DAGw2zJWdKY&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=hb9ec7dedc2" target="_blank">
  <button style="background-color:#f48b9a; color:white; padding:10px 20px; border:none; border-radius:5px; cursor:pointer;">
    Ver catálogo Stella Bags
  </button>
</a>
  <!-- Pedidos -->
  <section id="pedidos">
    <h2>Seguimiento y Registro de Pedido</h2>
    <form id="pedido-form">
      <input type="text" id="nombre" placeholder="Nombre completo" required>
      <input type="text" id="numPedido" placeholder="Número de pedido" required>
      <input type="tel" id="telefono" placeholder="Número de teléfono" required>
      <button type="submit">Registrar Pedido</button>
    </form>
    <table id="tablaPedidos">
      <tr><th>Número de Pedido</th><th>Nombre</th><th>Teléfono</th><th>Fase</th></tr>
    </table>
  </section>

<
  <!-- Políticas -->
  <section id="politicas">
    <div class="rectangulo">
      <h2>Políticas de Privacidad</h2>
      <p>Tu información personal será usada solo para procesar pedidos y comunicación. Nunca compartimos datos con terceros.</p>
       <h2>Políticas de compra, pago y envío</h2>
      <p>Confirmamos pedidos por WhatsApp o correo. Aceptamos pago por transferencia, depósito o efectivo (según disponibilidad). Los envíos se realizan a nivel nacional en 2 a 5 días laborables; el costo corre por cuenta del cliente.</p>
      <h2>Políticas de combios y devoluciones</h2>
      <p>Por higiene y exclusividad, no se aceptan devoluciones en argollas.

En el caso de carteras tejidas, solo se aceptan cambios por defectos de fabricación, reportados dentro de las 24 horas posteriores a la entrega. El producto debe estar en su empaque original y sin señales de uso. No aplican cambios por mal uso, desgaste, golpes, manchas o falta de cuidado.</p>
    </div>
  </section>

  <!-- Contacto -->
  <section id="contacto">
    <div class="rectangulo">
      <h2>Contacto</h2>
      <p>Tel: 0995372875</p>
      <p>Email: rayo_de_luna_13@hotmail.com</p>
         <p>Instagram: @rayo_de_luna_13</p>
    </div>
  </section>

  <!-- FAQ -->
  <section id="faq">
    <div class="rectangulo">
      <h2>Preguntas Frecuentes</h2>
       <p>¿Qué combos tienen disponibles? combo estrella, combo doble estrella, combo estelar y la colección Aura tambien contamos con Stella bags.</p>
      <p>🚚 ¿Hacen envíos? Sí, realizamos envíos a nivel nacional en un plazo de 2 a 5 días laborables.</p>
      <p>💳 ¿Qué métodos de pago aceptan? Transferencia y efectivo contra entrega.</p>
       <p>¿Cómo puedo hacer un pedido? A través de nuestra página web, el carrito de compras o escribiéndonos por WhatsApp para confirmar tu orden..</p>
       <p>¿Cómo puedo hacer un pedido? A través de nuestra página web, el carrito de compras o escribiéndonos por WhatsApp para confirmar tu orden..</p>
    </div>
  </section>
<h2>Carrito</h2>
<table>
  <thead>
    <tr>
      <th>Número de Pedido</th>
      <th>Producto</th>
      <th>Cantidad</th>
      <th>Precio</th>
      <th>Eliminar</th>
    </tr>
  </thead>
  <tbody id="carrito"></tbody>
</table>

<h3>Total: $<span id="total">0.00</span></h3>

<script>
function generarNumeroPedido() {
  return Math.floor(Math.random() * 9000) + 1000; // 1000 a 9999
}

function agregarAlCarrito(producto, precio) {
  let numeroPedido = generarNumeroPedido();
  let carrito = document.getElementById('carrito');
  
  let fila = document.createElement('tr');
  fila.innerHTML = `
    <td>${numeroPedido}</td>
    <td>${producto}</td>
    <td>1</td>
    <td>${precio}</td>
    <td><button onclick="eliminarFila(this)">❌</button></td>
  `;
  
  carrito.appendChild(fila);
  actualizarTotal();
}

function eliminarFila(boton) {
  boton.parentElement.parentElement.remove();
  actualizarTotal();
}

function actualizarTotal() {
  let filas = document.querySelectorAll('#carrito tr');
  let total = 0;
  filas.forEach(fila => {
    total += parseFloat(fila.cells[3].innerText);
  });
  document.getElementById('total').innerText = total.toFixed(2);
}
</script>

</body>
</html>

<!-- RAYITO: asistente flotante -->
<style>
  .rayito { position: fixed; bottom: 20px; right: 20px; }
  .rayito-toggle {
    background: #ffd6e4; border: none; border-radius: 50%;
    width: 60px; height: 60px; font-size: 24px; cursor: pointer;
    box-shadow: 0px 4px 6px rgba(0,0,0,0.2);
  }
  .rayito-window {
    position: fixed; bottom: 90px; right: 20px; width: 300px; max-height: 400px;
    background: white; border: 2px solid #ffd6e4; border-radius: 15px;
    display: none; flex-direction: column; box-shadow: 0px 4px 10px rgba(0,0,0,0.3);
    overflow: hidden; font-family: Arial, sans-serif;
  }
  .rayito-header {
    background: #ffd6e4; padding: 10px; font-weight: bold;
    display: flex; justify-content: space-between; align-items: center;
  }
  .rayito-body { padding: 10px; overflow-y: auto; flex: 1; font-size: 14px; }
  .rayito-msg { margin: 6px 0; padding: 8px; border-radius: 8px; background: #ffd6e4; }
  .rayito-actions { margin-top: 10px; display: flex; flex-wrap: wrap; gap: 6px; }
  .rayito-actions a, .rayito-actions button {
    flex: 1 1 auto; text-align: center; padding: 6px; border: none;
    border-radius: 6px; background: #ffd6e4; cursor: pointer;
    text-decoration: none; color: black; font-size: 13px;
  }
  .rayito-input {
    display: flex; border-top: 1px solid #ddd;
  }
  .rayito-input input {
    flex: 1; border: none; padding: 8px; outline: none;
  }
  .rayito-input button {
    background: #ffd6e4; border: none; cursor: pointer;
  }
  .msg-user { background:#eee; margin:6px 0; padding:8px; border-radius:8px; text-align:right; }
</style>

<div class="rayito">
  <button class="rayito-toggle" id="rayito-toggle">⚡</button>
</div>

<div class="rayito-window" id="rayito-window" aria-hidden="true">
  <div class="rayito-header">
    <strong>Rayito</strong>
    <button id="rayito-close">✕</button>
  </div>
  <div class="rayito-body" id="rayito-body">
    <div class="rayito-msg">¡Hola! Soy <strong>Rayito</strong> ⚡ ¿En qué puedo ayudarte?</div>
    <div class="rayito-actions">
      <a href="#productos">Ver combos</a>
      <button data-action="horario">Horarios</button>
      <a href="#faq">FAQ</a>
      <a href="https://wa.me/593995372875?text=Hola%20Rayitos%20de%20Luna%2C%20necesito%20ayuda%20con%20mi%20compra" target="_blank">WhatsApp</a>
    </div>
  </div>
  <div class="rayito-input">
    <input id="rayito-input" placeholder="Escribe aquí...">
    <button id="rayito-send">Enviar</button>
  </div>
</div>

<script>
  const toggleBtn = document.getElementById("rayito-toggle");
  const windowEl = document.getElementById("rayito-window");
  const closeBtn = document.getElementById("rayito-close");
  const bodyEl = document.getElementById("rayito-body");
  const inputEl = document.getElementById("rayito-input");
  const sendBtn = document.getElementById("rayito-send");

  toggleBtn.addEventListener("click", ()=> {
    windowEl.style.display = windowEl.style.display === "flex" ? "none" : "flex";
    windowEl.style.flexDirection = "column";
  });
  closeBtn.addEventListener("click", ()=> windowEl.style.display = "none");

  function addMsg(text, sender="bot"){
    const msg = document.createElement("div");
    msg.classList.add(sender==="user"?"msg-user":"rayito-msg");
    msg.innerHTML = text;
    bodyEl.appendChild(msg);
    bodyEl.scrollTop = bodyEl.scrollHeight;
  }

  function botReply(text){
    let response = "Lo siento, aún estoy aprendiendo ⚡";
    if(text.includes("hola")) response = "¡Hola! Soy Rayito ⚡ ¿Quieres ver combos, horario o hacer un pedido?";
    else if(text.includes("horario")) response = "Nuestro horario de atención es de 9am a 4pm 🕘";
    else if(text.includes("pedido")) response = "Puedes hacer tu pedido directo en nuestro WhatsApp 📲";
    else if(text.includes("catálogo") || text.includes("combo")) response = "Aquí tienes el catálogo 👉 <a href='#productos'>Ver combos</a>";
    addMsg(response,"bot");
  }

  function sendUserMsg(){
    const txt = inputEl.value.trim().toLowerCase();
    if(!txt) return;
    addMsg(inputEl.value,"user");
    inputEl.value="";
    setTimeout(()=> botReply(txt),600);
  }

  sendBtn.addEventListener("click", sendUserMsg);
  inputEl.addEventListener("keypress", e=>{ if(e.key==="Enter") sendUserMsg(); });

  // Botón "Horarios"
  document.querySelector("[data-action='horario']").addEventListener("click", ()=> {
    addMsg("Quiero saber el horario","user");
    botReply("horario");
  });
</script>


  

