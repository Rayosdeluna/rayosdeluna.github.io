<html  lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Rayos de Luna | Bisutería</title>
  <meta name="description" content="Bisutería hechas con amor en Ecuador. Entregas a domicilio. Combos y colección Aura. Pedidos con seguimiento." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --brand:#f48b9a;          /* Color principal */
      --brand-soft:#ffd6e4;     /* Fondo suave */
      --ink:#2b2b2b;            /* Texto principal */
      --muted:#6b7280;          /* Texto secundario */
      --white:#ffffff;
      --card:#fff7fa;
      --ok:#10b981;
      --warn:#f59e0b;
      --danger:#ef4444;
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{font-family:Poppins, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Noto Sans", "Apple Color Emoji","Segoe UI Emoji"; margin:0; color:var(--ink); background:linear-gradient(180deg, var(--brand-soft), #fff)}
    a{color:var(--brand); text-decoration:none}
    img{max-width:100%; display:block}

    /* Header */
    header{position:sticky; top:0; z-index:50; backdrop-filter:saturate(1.2) blur(6px); background:rgba(255,255,255,.8); border-bottom:1px solid rgba(0,0,0,.05)}
    .nav{max-width:1100px; margin:auto; display:flex; align-items:center; justify-content:space-between; padding:10px 16px}
    .brand{display:flex; align-items:center; gap:10px}
    .logo{width:40px; height:40px; border-radius:12px; background:conic-gradient(from 220deg, var(--brand), var(--brand-soft)); display:grid; place-items:center; font-weight:800; color:var(--white)}
    .brand h1{font-size:18px; margin:0}
    .menu{display:flex; gap:14px; flex-wrap:wrap}
    .menu a{padding:8px 12px; border-radius:999px; font-weight:500; color:#1f2937}
    .menu a:hover{background:var(--brand-soft)}

    /* Hero */
    .hero{max-width:1100px; margin:28px auto; padding:0 16px; display:grid; grid-template-columns:1.1fr .9fr; gap:24px; align-items:center}
    .card{background:var(--card); border:1px solid rgba(0,0,0,.05); border-radius:20px; padding:20px; box-shadow:0 10px 20px rgba(244,139,154,.12)}
    .badge{display:inline-flex; gap:8px; align-items:center; background:var(--white); border:1px solid rgba(0,0,0,.06); padding:6px 10px; border-radius:999px; font-size:12px}
    .cta{display:flex; gap:12px; margin-top:16px; flex-wrap:wrap}
    .btn{background:var(--brand); color:var(--white); border:none; padding:10px 16px; border-radius:12px; font-weight:600; cursor:pointer}
    .btn.secondary{background:#111827;}
    .btn.ghost{background:transparent; color:var(--brand); border:2px solid var(--brand)}
    .btn:disabled{opacity:.6; cursor:not-allowed}

    /* Sections */
    section{max-width:1100px; margin:36px auto; padding:0 16px}
    section h2{margin:0 0 14px; font-size:28px}
    .grid{display:grid; gap:16px}
    .grid.cols-3{grid-template-columns:repeat(3,1fr)}
    .grid.cols-2{grid-template-columns:repeat(2,1fr)}
    @media (max-width:900px){.hero{grid-template-columns:1fr}.grid.cols-3{grid-template-columns:1fr}.grid.cols-2{grid-template-columns:1fr}}

    .product{display:flex; flex-direction:column; gap:10px}
    .product .price{font-weight:700; font-size:18px}

    /* Pedidos */
    .form-row{display:grid; grid-template-columns:1fr 1fr; gap:12px}
    .form-row.single{grid-template-columns:1fr}
    label{font-size:14px; color:#374151}
    input, select, textarea{width:100%; padding:10px 12px; border-radius:12px; border:1px solid rgba(0,0,0,.12); background:#fff}
    textarea{min-height:88px}
    .items-table{width:100%; border-collapse:collapse; background:#fff; border-radius:14px; overflow:hidden}
    .items-table th, .items-table td{padding:10px; border-bottom:1px solid rgba(0,0,0,.06); text-align:left}
    .items-table tfoot td{font-weight:700}
    .status-chip{display:inline-flex; align-items:center; gap:6px; padding:6px 10px; border-radius:999px; font-size:12px; border:1px solid rgba(0,0,0,.06); background:#fff}
    .status-Por\ aprobar{border-color:var(--warn);}
    .status-Por\ preparar{border-color:#3b82f6}
    .status-Por\ enviar{border-color:#8b5cf6}
    .status-En\ tránsito{border-color:#06b6d4}
    .status-Entregado{border-color:var(--ok)}
    .status-Anulado{border-color:var(--danger)}
    .orders{overflow:auto}

    /* Footer */
    footer{margin-top:40px; padding:20px 16px; background:#111827; color:#e5e7eb}

    /* Rayito - Asistente flotante */
    .rayito{position:fixed; right:18px; bottom:18px; z-index:60}
    .rayito-toggle{display:flex; gap:8px; align-items:center; background:var(--brand); color:#fff; border:none; padding:12px 14px; border-radius:999px; font-weight:700; box-shadow:0 10px 20px rgba(244,139,154,.3); cursor:pointer}
    .rayito-window{position:fixed; right:18px; bottom:78px; width:320px; max-height:70vh; background:#fff; border:1px solid rgba(0,0,0,.08); border-radius:16px; box-shadow:0 20px 40px rgba(0,0,0,.12); display:none; flex-direction:column; overflow:hidden}
    .rayito-header{padding:10px 12px; background:var(--brand); color:#fff; display:flex; align-items:center; justify-content:space-between}
    .rayito-body{padding:12px; display:flex; flex-direction:column; gap:8px; overflow:auto}
    .rayito-msg{background:var(--brand-soft); padding:8px 10px; border-radius:12px; font-size:14px}
    .rayito-actions{display:flex; gap:8px; flex-wrap:wrap}
    .rayito-actions a, .rayito-actions button{padding:8px 10px; border-radius:999px; border:1px solid rgba(0,0,0,.08); background:#fff; cursor:pointer}
    .rayito-input{display:flex; gap:6px; padding:10px; border-top:1px solid rgba(0,0,0,.06)}
    .rayito-input input{flex:1}
     .carrito-btn {
      cursor: pointer;
      font-size: 20px;
      background: white;
      border: none;
      padding: 8px 12px;
      border-radius: 6px;
      color: #f48b9a;
      font-weight: bold;
  </style>
</head>
<body>
  <header>
     <!-- Carrito lateral -->
  <div id="carrito" class="carrito">
    <button class="cerrar" onclick="toggleCarrito()">X</button>
    <h2>🛒 Tu Carrito</h2>
    <ul id="lista-carrito"></ul>
    <p class="total">Total: $<span id="total">0</span></p>
    <a id="pagar" href="#" class="pagar-btn" target="_blank">Pagar por WhatsApp</a>
  </div>

  <script>
    let carrito = [];
    let total = 0;

    function añadirCarrito(nombre, precio) {
      carrito.push({ nombre, precio });
      total += precio;
      actualizarCarrito();
    }

    function actualizarCarrito() {
      let lista = document.getElementById("lista-carrito");
      lista.innerHTML = "";
      carrito.forEach((item, index) => {
        lista.innerHTML += `<li>${item.nombre} - $${item.precio}</li>`;
      });
      document.getElementById("total").textContent = total;

      let mensaje = "Hola, quiero confirmar mi pedido:%0A";
      carrito.forEach(item => {
        mensaje += `- ${item.nombre} $${item.precio}%0A`;
      });
      mensaje += `%0ATotal: $${total}`;
      document.getElementById("pagar").href = `https://wa.me/593999999999?text=${mensaje}`;
    }

    function toggleCarrito() {
      document.getElementById("carrito").classList.toggle("abierto");
    }
  </script>
</body>
 <h1>Rayos de Luna Bisutería</h1>
  <div class="menu">
    <a href="#inicio">Inicio</a>
    <a href="#nosotros">Nosotros</a>
    <a href="#productos">Productos</a>
    <a href="#pedidos">Pedidos</a>
    <a href="#politicas">Política de privacidad</a>
    <a href="#contacto">Contacto</a>
    <a href="#faq">Preguntas frecuentes</a>
  </div>
  </header>
 <!-- INICIO -->
  <section id="inicio" class="hero">
    <div class="card">
      <span class="badge">🇪🇨 Somos de Ecuador • Entregas a domicilio</span>
      <h2>Brilla con <span style="color:var(--brand)">rayos de Luna</span></h2>
      <p>Diseñamos bisutería hecha con cariño para tu día a día. Explora nuestros <strong>Combos</strong> y la exclusiva <strong>Colección Aura</strong> ✨.</p>
      <div class="cta">
        <a class="btn" href="#productos">Ver combos</a>
        <a class="btn ghost" href="https://wa.me/593995372875?text=Hola%20Rayos%20de%20Luna%2C%20vengo%20desde%20la%20web%20y%20quiero%20hacer%20un%20pedido" target="_blank" rel="noopener">WhatsApp</a>
      </div>
    </div>
    <div class="card">
    <img src="https://i.ibb.co/27MR6yxh/El-texto-del-p-rrafo-1.png" alt="El-texto-del-p-rrafo-1" border="0">
    </div>
  </section>
  
  <!-- NOSOTROS -->
  <section id="nosotros">
    <h2>Nosotros</h2>
    <div class="grid cols-2">
      <div class="card">
        <h3>¿Quiénes somos?</h3>
        <p>Somos <strong>Rayos de Luna</strong>, una marca ecuatoriana enfocada en piezas modernas, delicadas y accesibles. Entregamos a domicilio y confirmamos cada pedido por WhatsApp para tu tranquilidad.</p>
      </div>
      <div class="card">
        <h3>Misión</h3>
        <p>Diseñar empaques y piezas que reflejen el valor y la identidad de nuestras clientas, ofreciendo experiencias de compra claras y confiables.</p>
      </div>
      <div class="card">
        <h3>Visión</h3>
        <p>Ser la marca de referencia en bisutería de calidad en Ecuador, con servicio cercano y entregas puntuales.</p>
      </div>
      <div class="card">
        <h3>Valores</h3>
        <ul>
          <li>Calidad y detalle</li>
          <li>Transparencia y confianza</li>
          <li>Respeto por tus datos</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- PRODUCTOS -->
  <section id="productos">
    <h2>Productos</h2>
    <div class="grid cols-3">
      <article class="card product" data-sku="combo-estrella">
       <img src="https://i.ibb.co/bgqCwhDs/combo-estrella.png" alt="combo-estrella" width="120" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2);  display:flex; flex-direction:column; justify-content:center; align-items:center;">
        <h3>Combo Estrella</h3>
        <p>Un par de argollas.</p>
        <div class="price">$<span class="price-val">10.00</span></div>
        <div class="cta">
          <button class="btn add-to-order" data-sku="combo-estrella">Comprar estrella</button>
        </div>
      </article>
      <article class="card product" data-sku="combo-doble estrella">
       <img src="https://i.ibb.co/Xx0gjZgt/2.png" alt="combo-doble-estrella" width="120" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2);  display:flex; flex-direction:column; justify-content:center; align-items:center;">
        <h3>Combo Doble Estrella</h3>
        <p>Un par de argollas + una pulsera.</p>
        <div class="price">$<span class="price-val">15.00</span></div>
        <div class="cta">
          <button class="btn add-to-order" data-sku="combo-doble">Comprar doble estrella</button>
        </div>
      </article>
      <article class="card product" data-sku="combo-estelar">
<img src="https://i.ibb.co/1GvnrWB1/4.png" alt="combo-estelar" width="120" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2);  display:flex; flex-direction:column; justify-content:center; align-items:center;">
        <h3>Combo Estelar</h3>
        <p>Juego de pulseras.</p>
        <div class="price">$<span class="price-val">13.00</span></div>
        <div class="cta">
          <button class="btn add-to-order" data-sku="combo-estelar">Comprar Estelar</button>
        </div>
      </article>
      <article class="card product" data-sku="aura">
         <img src="https://i.ibb.co/8LJCHYWW/3.png" alt="colección Aura" width="120" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2); display:flex; flex-direction:column; justify-content:center; align-items:center;">
  <h3>Colección Aura</h3>
        <p>Un par de argollas únicas.</p>
        <div class="price">$<span class="price-val">10.00</span></div>
        <div class="cta">
          <button class="btn add-to-order" data-sku="aura" title="Este botón te lleva a Pedidos con Aura seleccionado">Comprar Aura</button>
        </div>
     </article>
            <article class="card product" data-sku="stella-bags">
  <img src="https://i.ibb.co/4nFS1rgp/Logo-Servicios-Profesionales-Moderno-Ilustrado-Rosado.png" alt="stella-bags"  width="120" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2); display:flex; flex-direction:column; justify-content:center; align-items:center;">
  <h3>Stella Bags</h3>
  <p>Carteras de ensueño.</p>
  <div class="price">$20.00</div>
  <div class="cta">
    <button class="btn add-to-order" data-sku="stella-bags" title="Este botón te lleva a Pedidos con Stella Bags seleccionado">Comprar Stella Bags</button>
        </div>
</article>
       <!-- BOTÓN CATALOGO -->
<div class="cta">
  <a class="btn" href="https://www.canva.com/design/DAGvc_2MElU/qVUR8dLijXOCEZZoHOpr8A/view?utm_content=DAGvc_2MElU&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=hc23b1edaf1" target="_blank" rel="noopener">Ver catálogo completo</a>

<!-- BOTÓN CATÁLOGO Stella Bags -->
<div class="cta">
  <a class="btn" href="https://www.canva.com/design/DAGw2zJWdKY/gUHcSTCXBe0ttl_0_bYkag/view?utm_content=DAGw2zJWdKY&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=hb9ec7dedc2" target="_blank" rel="noopener">Ver catálogo Stella Bags</a> 

  <!-- PEDIDOS -->
  <section id="pedidos">
    <h2>Pedidos</h2>
    <div class="card">
      <form id="order-form">
        <div class="form-row">
          <div>
            <label>Nombre y apellido</label>
            <input required name="nombre" placeholder="Tu nombre" />
          </div>
          <div>
            <label>WhatsApp</label>
            <input required name="whatsapp" placeholder="0991234567" />
          </div>
        </div>
        <div class="form-row single">
          <div>
            <label>Dirección de entrega</label>
            <input required name="direccion" placeholder="Calle, número, referencia" />
          </div>
        </div>
         <h3 style="margin:14px 0 8px">Selecciona tus productos</h3>
        <table class="items-table" id="items-table">
          <thead>
            <tr><th>Producto</th><th>Precio</th><th>Cantidad</th><th>Subtotal</th></tr>
          </thead>
          <tbody><!-- filas dinámicas --></tbody>
          <tfoot>
            <tr>
              <td colspan="3" style="text-align:right">Total</td>
              <td id="total-cell">$0.00</td>
            </tr>
          </tfoot>
        </table>
     <div class="form-row" style="margin-top:12px">
          <div>
            <label>Método de pago</label>
            <select required name="pago">
              <option value="Transferencia">Transferencia</option>
              <option value="Efectivo">Efectivo</option>
            </select>
          </div>
          <div>
            <label>Notas</label>
            <input name="notas" placeholder="Instrucciones adicionales" />
          </div>
        </div>
    <p style="font-size:13px;color:var(--muted);margin:10px 0">Todos los pedidos se <strong>confirman por WhatsApp</strong>. Tiempo de entrega estimado: <strong>3 días hábiles</strong>.</p>

  <div class="cta">
          <button class="btn" type="submit">Generar pedido</button>
          <a class="btn secondary" id="whatsapp-confirm" href="#" target="_blank" rel="noopener" title="Abrir WhatsApp con el detalle" aria-disabled="true">Confirmar por WhatsApp</a>
        </div>
      </form>
    </div>

 <div class="card" style="margin-top:16px">
      <h3>Seguimiento de pedidos</h3>
      <div class="form-row">
        <div>
          <label>ID de pedido</label>
          <input id="track-id" placeholder="Ej: RL-2025-0001" />
        </div>
        <div>
          <label>&nbsp;</label>
          <button class="btn" id="btn-track" type="button">Ver estado</button>
        </div>
      </div>
      <div id="track-result" style="margin-top:10px"></div>

   <h4 style="margin-top:16px">Todos los pedidos (local)</h4>
      <div class="orders">
        <table class="items-table" id="orders-table">
          <thead>
            <tr><th>ID</th><th>Cliente</th><th>Total</th><th>Estado</th><th>Actualizar</th></tr>
          </thead>
          <tbody><!-- dinámico --></tbody>
        </table>
      </div>
      <p style="font-size:12px;color:var(--muted)">*Esta tabla se guarda en tu navegador con <em>localStorage</em> para uso del negocio.</p>
    </div>
  </section>

  <!-- POLÍTICAS -->
  <section id="politicas">
    <h2>Política de privacidad, pedidos y devoluciones</h2>
    <div class="grid cols-3">
      <div class="card">
        <h3>Privacidad</h3>
        <p>Cuidamos tu información personal con total responsabilidad. Los datos se usan solo para procesar pedidos y promociones.</p>
      </div>
      <div class="card">
        <h3>Pedidos y Compras</h3>
        <p>Todos los pedidos se confirman por WhatsApp. Métodos de pago: transferencia o efectivo. Tiempo de entrega: <strong>3 días hábiles</strong>.</p>
      </div>
      <div class="card">
        <h3>Devoluciones y Cambios</h3>
        <p>Aceptamos devoluciones solo por defectos de fabricación, hasta <strong>48h</strong> después de la entrega.</p>
      </div>
    </div>
  </section>

  <!-- CONTACTO -->
  <section id="contacto">
    <h2>Contacto</h2>
    <div class="grid cols-2">
      <div class="card">
        <p><strong>Correo:</strong> <a href="mailto:rayo_de_luna_13@hotmail.com">rayo_de_luna_13@hotmail.com</a></p>
        <p><strong>Instagram & Facebook:</strong> <a href="https://instagram.com/Rayos_de_luna_13" target="_blank" rel="noopener">@Rayos_de_luna_13</a></p>
        <p><strong>WhatsApp:</strong> <a href="https://wa.me/593995372875" target="_blank" rel="noopener">099 537 2875</a></p>
        <p><strong>Horario de atención:</strong> Lun–Vie 9:00 AM – 4:00 PM</p>
      </div>
      <div class="card">
        <h3>¿Cómo comprar?</h3>
        <ol>
          <li>Elige tus productos en <a href="#productos">Productos</a>.</li>
          <li>Completa el <a href="#pedidos">formulario de pedidos</a>.</li>
          <li>Confirma por WhatsApp y recibe en casa.</li>
        </ol>
      </div>
    </div>
  </section>

  <!-- FAQ -->
  <section id="faq">
    <h2>Preguntas frecuentes</h2>
    <div class="grid cols-2">
      <div class="card">
        <h3>¿Cuáles son los combos?</h3>
        <p>Combo Estrella, Doble Estrella, Estelar y la Colección Aura.</p>
      </div>
      <div class="card">
        <h3>¿Cómo puedo pagar?</h3>
        <p>Aceptamos <strong>Transferencia</strong> o <strong>Efectivo</strong>.</p>
      </div>
      <div class="card">
        <h3>¿Horario de atención?</h3>
        <p>Lunes a Viernes, 9:00 AM a 4:00 PM.</p>
      </div>
      <div class="card">
        <h3>¿Hacen envíos?</h3>
        <p>Sí, realizamos entregas a domicilio dentro de Ecuador.</p>
      </div>
    </div>
 <footer>
    <p>&copy; 2025 Rayos de Luna | Todos los derechos reservados</p>
  </footer>
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

<div class="⚡">
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
