<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Rayos de Luna | Joyas</title>
<style>
:root {
  --pink:#f48b9a
  --blush:#ffd6e4;
  --ink:#1f2937;
  --muted:#6b7280;
  --radius:16px;
}
* {box-sizing:border-box;}
body {margin:0;font-family:Poppins,sans-serif;background:var(--blush);color:var(--ink);}
header {background:rgba(255,214,228,.95);position:sticky;top:0;z-index:50;padding:10px 20px;display:flex;align-items:center;justify-content:space-between;box-shadow:0 2px 5px rgba(0,0,0,0.1);}
header nav a {margin:0 10px;text-decoration:none;color:var(--ink);font-weight:600;cursor:pointer;}
header nav a.active {color:white;background:var(--pink);padding:6px 12px;border-radius:12px;}
#cart {background:var(--pink);color:white;padding:6px 12px;border-radius:12px;cursor:pointer;margin-left:10px;}
.container {max-width:1100px;margin:0 auto;padding:20px;}
section {display:none;padding:40px 0;}
section.active {display:block;}
h2 {color:var(--pink);}
.grid {display:grid;gap:20px;}
.grid-3 {grid-template-columns:repeat(3,1fr);}
.card {background:white;padding:12px;border-radius:var(--radius);text-align:center;position:relative;}
.card img {width:100%;border-radius:var(--radius);}
.btn {padding:8px 14px;border:none;border-radius:12px;cursor:pointer;font-weight:600;}
.btn-primary {background:var(--pink);color:white;}
.btn-outline {background:white;color:var(--pink);border:1px solid var(--pink);}
#cartWindow {position:absolute;top:50px;right:20px;width:300px;background:white;border-radius:16px;padding:12px;display:none;box-shadow:0 4px 12px rgba(0,0,0,0.2);z-index:70;}
#cartWindow h3 {margin-top:0;color:var(--pink);}
#cartItems {max-height:200px;overflow-y:auto;margin-bottom:10px;}
.cart-item {display:flex;justify-content:space-between;margin-bottom:6px;font-size:14px;}
.cart-total {font-weight:700;}
</style>
</head>
<body>

<header>
  <h1>Rayos de Luna</h1>
  <nav>
    <a class="active" data-tab="inicio">Inicio</a>
    <a data-tab="nosotros">Nosotros</a>
    <a data-tab="productos">Productos</a>
    <a data-tab="pedidos">Pedidos</a>
    <a data-tab="politicas">Políticas</a>
    <a data-tab="contactos">Contactos</a>
    <a data-tab="faq">FAQ</a>
    <span id="cart">🛒  (<span id="cartCount">0</span>)</span>
  </nav>
</header>

<div class="container">

<!-- Inicio -->
<section id="inicio" class="active">
<h2>Bienvenidos a Rayos de Luna</h2>
<p>Ofrecemos piezass únicas y exclusivas para destacar tu estilo.</p>
<p>Aquí cada detalle está pensado para ti. Encuentra productos únicos, de la mejor calidad y a precios que se ajustan a lo que buscas.</p>
<p>💖 Compra fácil, segura y sin complicaciones, desde la comodidad de tu casa.</p>
<p>👉 Solo elige tu favorito, haz tu pedido ¡y nosotros lo llevamos directo a tu puerta! 🚚✨</p>
</section>

<!-- Nosotros -->
<section id="nosotros">
<h2>Nosotros</h2>
<p>Quiénes somos?</p>
<p>Somos Rayos de Luna , una marca ecuatoriana enfocada en piezas modernas, delicadas y accesibles. Entregamos a domicilio y confirmamos cada pedido por WhatsApp para tu tranquilidad.</p>

<p>Misión
<p>Diseñar empaques y joyas que reflejen el valor y la identidad de nuestras clientes, ofreciendo experiencias de compra claras y confiables.</p>

<p>Visión
<p>Ser la marca de referencia en bisutería de calidad en Ecuador, con servicio cercano y entregas puntuales.</p>

<p>Valores</p>
<p>Calidad y detalle</p>
<p>Transparencia y confianza</p>
<p>Respeto por tus datos</p>
<p>Rayos de Luna celebra la feminidad y el brillo interior. Trabajamos con materiales hipoalergénicos y acabados de alta calidad.</p>
</section>

<!-- Productos -->

<section id="Combo estrella">
<h2>Combo estrella</h2>
<div class="grid grid-3" id="productGrid">
  <div class="card">
    <a href="https://ibb.co/VcJX7Bbp"><img src="https://i.ibb.co/VcJX7Bbp/combo-estrella.png" alt="combo-estrella" border="0"></a>
    <h3>Producto 1</h3>
    <p>$10.00</p>
    <button class="btn btn-primary" data-name="Producto 1" data-price="10.00">Añadir al carrito</button>
  </div>
  <div class="card">
    <img src="producto2.jpg" alt="Producto 2">
    <h3>Producto 2</h3>
    <p>$30</p>
    <button class="btn btn-primary" data-name="Producto 2" data-price="30">Añadir al carrito</button>
  </div>
  <div class="card">
    <img src="producto3.jpg" alt="Producto 3">
    <h3>Producto 3</h3>
    <p>$20</p>
    <button class="btn btn-primary" data-name="Producto 3" data-price="20">Añadir al carrito</button>
  </div>
  <div class="card">
    <img src="producto4.jpg" alt="Producto 4">
    <h3>Producto 4</h3>
    <p>$18</p>
    <button class="btn btn-primary" data-name="Producto 4" data-price="18">Añadir al carrito</button>
  </div>
  <div class="card">
    <img src="producto5.jpg" alt="Producto 5">
    <h3>Producto 5</h3>
    <p>$22</p>
    <button class="btn btn-primary" data-name="Producto 5" data-price="22">Añadir al carrito</button>
  </div>
</div>
</section>

<!-- Pedidos -->
<section id="pedidos">
<h2>Pedidos</h2>
<div id="cartItemsContainer">
<p>Aquí aparecerán tus productos añadidos al carrito y el seguimiento del pedido.</p>
<div id="cartItems"></div>
<p class="cart-total">Total: $<span id="cartTotal">0</span></p>
</div>
</section>

<!-- Políticas -->
<section id="politicas">
<h2>Políticas de privacidad</h2>
<p>Aquí puedes colocar tus políticas.</p>
</section>

<!-- Contactos -->
<section id="contactos">
<h2>Contactos</h2>
<p>WhatsApp: <a href="https://wa.me/1234567890">Enviar mensaje</a></p>
<p>Email: contacto@rayosdeluna.com</p>
</section>

<!-- FAQ -->
<section id="faq">
<h2>Preguntas frecuentes</h2>
<p>Aquí puedes colocar las preguntas frecuentes.</p>
</section>

</div>

<!-- Carrito ventana -->
<div id="cartWindow">
<h3>Carrito</h3>
<div id="cartItems"></div>
<p class="cart-total">Total: $<span id="cartTotalWindow">0</span></p>
</div>

<script>
// Cambiar de pestañas
const tabs = document.querySelectorAll('header nav a');
const sections = document.querySelectorAll('section');
tabs.forEach(tab => {
  tab.addEventListener('click', () => {
    tabs.forEach(t=>t.classList.remove('active'));
    tab.classList.add('active');
    const target = tab.getAttribute('data-tab');
    sections.forEach(sec => sec.id===target?sec.classList.add('active'):sec.classList.remove('active'));
  });
});

// Carrito
let cart = [];
const cartBtn = document.getElementById('cart');
const cartWindow = document.getElementById('cartWindow');
const cartItemsDiv = document.getElementById('cartItems');
const cartCount = document.getElementById('cartCount');
const cartTotalWindow = document.getElementById('cartTotalWindow');

document.querySelectorAll('.btn-primary').forEach(btn=>{
  btn.addEventListener('click',()=>{
    const name = btn.getAttribute('data-name');
    const price = parseFloat(btn.getAttribute('data-price'));
    const existing = cart.find(p=>p.name===name);
    if(existing){existing.qty+=1;} else {cart.push({name,price,qty:1});}
    updateCart();
  });
});

cartBtn.addEventListener('click',()=>{cartWindow.style.display = cartWindow.style.display==='block'?'none':'block';});

function updateCart(){
  cartItemsDiv.innerHTML='';
  let total=0;
  cart.forEach(item=>{
    total+=item.price*item.qty;
    cartItemsDiv.innerHTML+=`<div class="cart-item">${item.name} x ${item.qty} = $${item.price*item.qty}</div>`;
  });
  cartCount.textContent=cart.reduce((a,b)=>a+b.qty,0);
  cartTotalWindow.textContent=total;
  document.getElementById('cartTotal').textContent=total;
}
</body>
</html>
// Navegación activa
document.querySelectorAll('.navlinks a').forEach(link=>{
  link.addEventListener('click',e=>{
    document.querySelectorAll('.navlinks a').forEach(l=>l.classList.remove('active'));
    e.target.classList.add('active');
  });
});

// Carrito
let cart=[];
const cartBtn = document.getElementById('cart');
const cartWindow = document.getElementById('cartWindow');
const cartItemsDiv = document.getElementById('cartItems');
const cartCount = document.getElementById('cartCount');
const cartTotalWindow = document.getElementById('cartTotalWindow');
const checkoutBtn = document.getElementById('checkoutBtn');

document.querySelectorAll('.add-to-cart').forEach(btn=>{
  btn.addEventListener('click',()=>{
    const name = btn.getAttribute('data-name');
    const price = parseFloat(btn.getAttribute('data-price'));
    const existing = cart.find(p=>p.name===name);
    if(existing){existing.qty+=1;} else {cart.push({name,price,qty:1});}
    updateCart();
  });
});

cartBtn.addEventListener('click',()=>{cartWindow.style.display = cartWindow.style.display==='block'?'none':'block';});

// Botón WhatsApp
checkoutBtn.addEventListener('click', ()=>{
  if(cart.length===0){alert('No hay productos en el carrito'); return;}
  let mensaje="Hola, este es mi pedido por confirmar:%0A";
  cart.forEach(item=>{
    mensaje+=`- ${item.name} x ${item.qty} = $${item.price*item.qty}%0A`;
  });
  mensaje+=`Total: $${cart.reduce((a,b)=>a+b.price*b.qty,0)}`;
  window.open(`https://wa.me/1234567890?text=${mensaje}`, '_blank');
});

function updateCart(){
  cartItemsDiv.innerHTML='';
  let total=0;
  cart.forEach(item=>{
    total+=item.price*item.qty;
    cartItemsDiv.innerHTML+=`<div class="cart-item">${item.name} x ${item.qty} = $${item.price*item.qty}</div>`;
  });
  cartCount.textContent=cart.reduce((a,b)=>a+b.qty,0);
  cartTotalWindow.textContent=total;
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


  

