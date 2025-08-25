<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rayos de Luna | Bisutería</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #fff0f3;
      color: #333;
    }
    header {
      background: #f48b9a;
      padding: 15px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      color: white;
    }
    header h1 {
      margin: 0;
    }
    nav {
      display: flex;
      gap: 15px;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }
    section {
      display: none;
      padding: 40px;
    }
    section.active {
      display: block;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
    }
    .card {
      background: white;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      text-align: center;
    }
    .card img {
      max-width: 100%;
      border-radius: 8px;
    }
    button {
      margin-top: 10px;
      padding: 8px 15px;
      border: none;
      border-radius: 5px;
      background: #f48b9a;
      color: white;
      cursor: pointer;
    }
    button:hover {
      background: #e76a7d;
    }
    /* Carrito */
    .cart-icon {
      cursor: pointer;
      font-size: 20px;
      position: relative;
    }
    .cart-count {
      position: absolute;
      top: -8px;
      right: -8px;
      background: white;
      color: #f48b9a;
      border-radius: 50%;
      padding: 2px 6px;
      font-size: 12px;
      font-weight: bold;
    }
    .cart-panel {
      position: fixed;
      top: 0;
      right: -350px;
      width: 300px;
      height: 100%;
      background: white;
      box-shadow: -2px 0 8px rgba(0,0,0,0.2);
      padding: 20px;
      transition: right 0.3s ease;
      overflow-y: auto;
      z-index: 1000;
    }
    .cart-panel.active {
      right: 0;
    }
    .cart-item {
      border-bottom: 1px solid #ddd;
      padding: 10px 0;
    }
    .cart-total {
      font-weight: bold;
      margin-top: 15px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Rayos de Luna</h1>
    <nav>
      <a href="#inicio" onclick="showSection('inicio')">Inicio</a>
      <a href="#nosotros" onclick="showSection('nosotros')">Nosotros</a>
      <a href="#productos" onclick="showSection('productos')">Productos</a>
      <a href="#pedidos" onclick="showSection('pedidos')">Pedidos</a>
      <a href="#politicas" onclick="showSection('politicas')">Políticas</a>
      <a href="#contacto" onclick="showSection('contacto')">Contacto</a>
      <a href="#faq" onclick="showSection('faq')">FAQ</a>
    </nav>
    <div class="cart-icon" onclick="toggleCart()">🛒<span class="cart-count" id="cart-count">0</span></div>
  </header>

  <!-- Secciones -->
  <section id="inicio" class="active">
    <h2>Bienvenidos a Rayos de Luna</h2>
    <p>Bisutería hecha con amor y detalle para resaltar tu estilo único.</p>
  </section>

  <section id="nosotros">
    <h2>Nosotros</h2>
    <p>Somos un emprendimiento dedicado a la creación de bisutería artesanal con diseños exclusivos.</p>
  </section>

  <section id="productos">
    <h2>Nuestros Productos</h2>
    <div class="products">
      <div class="card">
        <img src="https://i.ibb.co/1GvnrWB1/4.png" alt="Combo Estelar">
        <h3>Combo Estelar</h3>
        <p>$15.00</p>
        <button onclick="addToCart('Combo Estelar', 15)">Añadir al carrito</button>
      </div>
      <div class="card">
        <img src="https://i.ibb.co/HD1bwv3t/tu-imagen.jpg" alt="Colección Aura">
        <h3>Colección Aura</h3>
        <p>$20.00</p>
        <button onclick="addToCart('Colección Aura', 20)">Añadir al carrito</button>
      </div>
    </div>
  </section>

  <section id="pedidos">
    <h2>Pedidos</h2>
    <p>Haz tus pedidos y te contactaremos para la entrega.</p>
  </section>

  <section id="politicas">
    <h2>Políticas de Privacidad</h2>
    <p>Respetamos tu privacidad y protegemos tus datos.</p>
  </section>

  <section id="contacto">
    <h2>Contacto</h2>
    <p>Escríbenos a nuestro WhatsApp para más información.</p>
  </section>

  <section id="faq">
    <h2>Preguntas Frecuentes</h2>
    <p>Encuentra aquí respuestas a tus dudas más comunes.</p>
  </section>

  <!-- Carrito -->
  <div class="cart-panel" id="cart-panel">
    <h2>Tu Carrito</h2>
    <div id="cart-items"></div>
    <p class="cart-total">Total: $<span id="cart-total">0.00</span></p>
    <button onclick="checkout()">Confirmar Pedido</button>
  </div>

  <script>
    let cart = [];

    function showSection(id) {
      document.querySelectorAll("section").forEach(s => s.classList.remove("active"));
      document.getElementById(id).classList.add("active");
    }

    function toggleCart() {
      document.getElementById("cart-panel").classList.toggle("active");
    }

    function addToCart(product, price) {
      cart.push({ product, price });
      updateCart();
    }

    function updateCart() {
      const cartItems = document.getElementById("cart-items");
      cartItems.innerHTML = "";
      let total = 0;
      cart.forEach(item => {
        total += item.price;
        cartItems.innerHTML += `<div class="cart-item">${item.product} - $${item.price.toFixed(2)}</div>`;
      });
      document.getElementById("cart-total").textContent = total.toFixed(2);
      document.getElementById("cart-count").textContent = cart.length;
    }

    function checkout() {
      let message = "Hola, quiero confirmar mi pedido:\n";
      cart.forEach(item => {
        message += `- ${item.product}: $${item.price.toFixed(2)}\n`;
      });
      message += `Total: $${document.getElementById("cart-total").textContent}`;
      window.open(`https://wa.me/593995372875?text=${encodeURIComponent(message)}`, "_blank");
    }
  </script>
</body>
</html>




 
  
  <title>Rayos de Luna | Asistente Rayito</title>
  <style>
    /* Estilos del botón flotante */
    .chat-btn {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #f48b9a;
      color: white;
      border: none;
      border-radius: 50%;
      width: 60px;
      height: 60px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 28px;
      cursor: pointer;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      transition: all 0.3s ease;
    }
    .chat-btn:hover {
      background-color: #e07282;
    }

    /* Ventana de chat */
    .chat-window {
      position: fixed;
      bottom: 90px;
      right: 20px;
      width: 300px;
      max-height: 400px;
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 6px 12px rgba(0,0,0,0.3);
      display: none;
      flex-direction: column;
      overflow: hidden;
      font-family: Arial, sans-serif;
    }
    .chat-header {
      background: #f48b9a;
      color: white;
      padding: 10px;
      text-align: center;
      font-weight: bold;
    }
    .chat-body {
      flex: 1;
      padding: 10px;
      overflow-y: auto;
      font-size: 14px;
    }
    .chat-footer {
      display: flex;
      border-top: 1px solid #ddd;
    }
    .chat-footer input {
      flex: 1;
      padding: 8px;
      border: none;
      outline: none;
    }
    .chat-footer button {
      background: #f48b9a;
      border: none;
      color: white;
      padding: 8px 12px;
      cursor: pointer;
    }
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

  

