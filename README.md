<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Rayos de Luna | Bisutería</title>
  <meta name="description" content="Bisutería y joyas hechas con amor en Ecuador. Entregas a domicilio. Combos y colección Aura. Pedidos con seguimiento." />
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
  </style>
</head>
<body>
  <header>
        <h1>Rayos de Luna Bisutería</h1>
      </div>
      <div class="menu">
        <a href="#inicio">Inicio</a>
        <a href="#nosotros">Nosotros</a>
        <a href="#productos">Productos</a>
        <a href="#pedidos">Pedidos</a>
        <a href="#politicas">Política de privacidad</a>
        <a href="#contacto">Contacto</a>
        <a href="#faq">Preguntas frecuentes</a>
      </div>
    </nav>
  </header>

  <!-- INICIO -->
  <section id="inicio" class="hero">
    <div class="card">
      <span class="badge">🇪🇨 Somos de Ecuador • Entregas a domicilio</span>
      <h2>Brilla con <span style="color:var(--brand)">Rayos de Luna</span></h2>
      <p>Diseñamos bisutería y joyas con cariño para tu día a día. Explora nuestros <strong>Combos</strong> y la exclusiva <strong>Colección Aura</strong> ✨.</p>
      <div class="cta">
        <a class="btn" href="#productos">Ver combos</a>
        <a class="btn ghost" href="https://wa.me/593995372875?text=Hola%20Rayos%20de%20Luna%2C%20vengo%20desde%20la%20web%20y%20quiero%20hacer%20un%20pedido" target="_blank" rel="noopener">WhatsApp</a>
      </div>
    </div>
    <div class="card">
      <a href="https://imgbb.com/">
  <img src="https://i.ibb.co/dJmSGh63/logo-Rayos-de-luna.png" 
       alt="logo-Rayos-de-luna" 
       style="width:120px; height:auto; border:0;" />
</a>
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
        <p>Diseñar empaques y joyas que reflejen el valor y la identidad de nuestras clientas, ofreciendo experiencias de compra claras y confiables.</p>
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
    <p style="margin-bottom:8px">Precios editables en el código (ver <code>CATALOGO</code> en JavaScript).</p>
    <div class="grid cols-3">
      <article class="card product" data-sku="combo-estrella">
        <a href="https://imgbb.com/"><img src="https://i.ibb.co/bgqCwhDs/combo-estrella.png" alt="combo-estrella" border="0"></a>
        <h3>Combo Estrella</h3>
        <p>Un par de argollas.</p>
        <div class="price">$<span class="price-val">10.00</span></div>
        <div class="cta">
          <button class="btn add-to-order" data-sku="combo-estrella">Comprar</button>
        </div>
      </article>
      <article class="card product" data-sku="combo-doble estrella">
       <img src="https://i.ibb.co/bgqCwhDs/combo-estrella.png" alt="combo-estrella" width="120" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2);">
        <h3>Combo Doble Estrella</h3>
        <p>Un par de argollas + una pulsera.</p>
        <div class="price">$<span class="price-val">15.00</span></div>
        <div class="cta">
          <button class="btn add-to-order" data-sku="combo-doble">Comprar</button>
        </div>
      </article>
      <article class="card product" data-sku="combo-estelar">
        <img src="https://i.ibb.co/Xx0gjZgt/2.png" alt="2" width="120" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2);">
  </a>
        <h3>Combo Estelar</h3>
        <p>Juego de pulseras.</p>
        <div class="price">$<span class="price-val">13.00</span></div>
        <div class="cta">
          <button class="btn add-to-order" data-sku="combo-estelar">Comprar</button>
        </div>
      </article>
      <article class="card product" data-sku="aura">
         <img src="https://i.ibb.co/1GvnrWB1/4.png" alt="4" width="120" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2);">
  </a>
        <h3>Colección Aura</h3>
        <p>Un par de argollas únicas.</p>
        <div class="price">$<span class="price-val">10.00</span></div>
        <div class="cta">
          <button class="btn add-to-order" data-sku="aura" title="Este botón te lleva a Pedidos con Aura seleccionado">Comprar Aura</button>
        </div>
      </article>
    </div>
  </section>

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
  </section>

  <!-- FOOTER -->
  <footer>
    <div style="max-width:1100px; margin:auto; display:flex; justify-content:space-between; gap:16px; flex-wrap:wrap">
      <p>© <span id="year"></span> Rayos de Luna · Joyas</p>
      <p>Hecho con ♥ para brillar contigo</p>
    </div>
  </footer>

  <!-- RAYITO: asistente flotante -->
  <div class="rayito">
    <button class="rayito-toggle" id="rayito-toggle">⚡ Rayito</button>
  </div>
  <div class="rayito-window" id="rayito-window" aria-hidden="true">
    <div class="rayito-header">
      <strong>Rayito</strong>
      <button id="rayito-close" class="btn" style="padding:6px 10px; background:rgba(255,255,255,.2); border:1px solid rgba(255,255,255,.5)">✕</button>
    </div>
    <div class="rayito-body" id="rayito-body">
      <div class="rayito-msg">¡Hola! Soy <strong>Rayito</strong> ⚡ ¿En qué puedo ayudarte?</div>
      <div class="rayito-actions">
        <a href="#productos">Ver combos</a>
        <button data-action="horario">Horarios</button>
        <a href="#faq">FAQ</a>
        <a href="https://wa.me/593995372875?text=Hola%20Rayitos%20de%20Luna%2C%20necesito%20ayuda%20con%20mi%20compra" target="_blank" rel="noopener">WhatsApp</a>
      </div>
    </div>
    <div class="rayito-input">
      <input id="rayito-input" placeholder="Escribe aquí... (ej: combos, horario, pagar)"/>
      <button class="btn" id="rayito-send" style="padding:8px 12px">Enviar</button>
    </div>
  </div>

  <script>
    // ======= UTILIDADES =======
    const $ = (sel, ctx=document) => ctx.querySelector(sel);
    const $$ = (sel, ctx=document) => Array.from(ctx.querySelectorAll(sel));
    const formatMoney = n => '$' + n.toFixed(2);

    // ======= CATÁLOGO (edita precios y nombres aquí) =======
    const CATALOGO = {
      'combo-estrella': { nombre: 'Combo Estrella', precio: 12.00 },
      'combo-doble':    { nombre: 'Combo Doble Estrella', precio: 18.00 },
      'combo-estelar':  { nombre: 'Combo Estelar', precio: 20.00 },
      'aura':           { nombre: 'Colección Aura (argollas únicas)', precio: 15.00 },
    };

    // Rellena precios en cards por si se cambian arriba
    $$('#productos .product').forEach(card => {
      const sku = card.dataset.sku; const p = CATALOGO[sku]?.precio ?? 0;
      const priceEl = card.querySelector('.price-val'); if(priceEl) priceEl.textContent = p.toFixed(2);
    });

    // ======= PEDIDOS (tabla dinámica) =======
    const itemsBody = $('#items-table tbody');
    const totalCell = $('#total-cell');
    const whatsappBtn = $('#whatsapp-confirm');

    function crearFila(sku) {
      const prod = CATALOGO[sku]; if(!prod) return;
      const tr = document.createElement('tr'); tr.dataset.sku = sku;
      tr.innerHTML = `
        <td>${prod.nombre}</td>
        <td>${formatMoney(prod.precio)}</td>
        <td>
          <input type="number" min="0" value="1" style="width:80px" aria-label="Cantidad" />
        </td>
        <td class="subtotal">${formatMoney(prod.precio)}</td>
      `;
      const qty = tr.querySelector('input');
      qty.addEventListener('input', () => { if(qty.value < 0) qty.value = 0; actualizarTotal(); });
      itemsBody.appendChild(tr);
      actualizarTotal();
    }

    function actualizarTotal(){
      let total = 0;
      $$('#items-table tbody tr').forEach(tr => {
        const sku = tr.dataset.sku; const precio = CATALOGO[sku].precio; const qty = Number(tr.querySelector('input').value || 0);
        const sub = precio * qty; tr.querySelector('.subtotal').textContent = formatMoney(sub); total += sub;
      });
      totalCell.textContent = formatMoney(total);
      // Habilitar/enlazar WhatsApp
      const data = obtenerDatosFormulario(false);
      if(total > 0 && data.nombre && data.whatsapp){
        const texto = encodeURIComponent(
          `Hola Rayos de Luna, quiero confirmar mi pedido.\n`+
          `Nombre: ${data.nombre}\nWhatsApp: ${data.whatsapp}\nDirección: ${data.direccion}\n`+
          `Pago: ${data.pago || '-'}\n`+
          `Productos:\n`+
          $$('#items-table tbody tr').map(tr=>{
            const sku = tr.dataset.sku; const q = tr.querySelector('input').value; return `- ${CATALOGO[sku].nombre} x${q}`;
          }).join('\n') + `\nTotal: ${totalCell.textContent}`
        );
        whatsappBtn.href = `https://wa.me/593995372875?text=${texto}`;
        whatsappBtn.removeAttribute('aria-disabled');
      } else {
        whatsappBtn.href = '#';
        whatsappBtn.setAttribute('aria-disabled','true');
      }
    }

    function obtenerDatosFormulario(includeItems=true){
      const form = $('#order-form');
      const fd = new FormData(form);
      const data = Object.fromEntries(fd.entries());
      data.items = includeItems ? $$('#items-table tbody tr').map(tr=>({
        sku: tr.dataset.sku,
        nombre: CATALOGO[tr.dataset.sku].nombre,
        precio: CATALOGO[tr.dataset.sku].precio,
        cantidad: Number(tr.querySelector('input').value || 0),
      })) : [];
      data.total = $$('#items-table tbody tr').reduce((acc,tr)=>{
        const sku = tr.dataset.sku; return acc + CATALOGO[sku].precio * Number(tr.querySelector('input').value||0)
      },0);
      return data;
    }

    // Añadir productos desde cards
    $$('.add-to-order').forEach(btn => btn.addEventListener('click', () => {
      const sku = btn.dataset.sku; const existente = $(`#items-table tbody tr[data-sku="${sku}"]`);
      if(!existente){ crearFila(sku); } else {
        const qty = existente.querySelector('input'); qty.value = Number(qty.value||0) + 1; actualizarTotal();
      }
      // Ir a Pedidos
      location.hash = '#pedidos';
    }));

    // Render inicial: todas las filas con cantidad 0 para que el cliente elija
    Object.keys(CATALOGO).forEach(sku=>{ crearFila(sku); const row = $(`#items-table tbody tr[data-sku="${sku}"]`); if(row){ row.querySelector('input').value = 0; }});
    actualizarTotal();

    // ======= GENERAR PEDIDO =======
    const ORD_KEY = 'rayosdluna_pedidos_v1';
    const leerPedidos = () => JSON.parse(localStorage.getItem(ORD_KEY) || '[]');
    const guardarPedidos = (arr) => localStorage.setItem(ORD_KEY, JSON.stringify(arr));

    function generarId(){
      const hoy = new Date();
      const year = hoy.getFullYear();
      const num = (leerPedidos().length + 1).toString().padStart(4,'0');
      return `RL-${year}-${num}`;
    }

    function renderTablaPedidos(){
      const pedidos = leerPedidos();
      const tbody = $('#orders-table tbody');
      tbody.innerHTML = '';
      pedidos.forEach(p => {
        const tr = document.createElement('tr');
        tr.innerHTML = `
          <td>${p.id}</td>
          <td>${p.nombre}</td>
          <td>${formatMoney(p.total)}</td>
          <td><span class="status-chip status-${p.estado.replaceAll(' ','\ ')}">${p.estado}</span></td>
          <td>
            <select data-id="${p.id}">
              ${['Por aprobar','Por preparar','Por enviar','En tránsito','Entregado','Anulado'].map(s=>`<option ${s===p.estado?'selected':''}>${s}</option>`).join('')}
            </select>
          </td>`;
        tbody.appendChild(tr);
      });
      // listeners de cambio de estado
      $$('#orders-table select').forEach(sel=> sel.addEventListener('change', e=>{
        const pedidos = leerPedidos();
        const id = sel.dataset.id; const idx = pedidos.findIndex(x=>x.id===id);
        if(idx>-1){ pedidos[idx].estado = sel.value; guardarPedidos(pedidos); renderTablaPedidos(); renderTrack(); }
      }));
    }

    function renderTrack(){
      const id = $('#track-id').value.trim();
      const pedidos = leerPedidos();
      const p = pedidos.find(x=>x.id===id);
      const out = $('#track-result');
      if(!id){ out.innerHTML = '<p style="color:var(--muted)">Ingresa un ID de pedido para ver el estado.</p>'; return; }
      if(!p){ out.innerHTML = '<p style="color:var(--danger)">No encontramos ese pedido. Verifica el ID.</p>'; return; }
      out.innerHTML = `
        <div class="card" style="background:#fff">
          <p><strong>Pedido:</strong> ${p.id}</p>
          <p><strong>Cliente:</strong> ${p.nombre}</p>
          <p><strong>Total:</strong> ${formatMoney(p.total)}</p>
          <p><strong>Estado:</strong> <span class="status-chip status-${p.estado.replaceAll(' ','\ ')}">${p.estado}</span></p>
        </div>`;
    }

    $('#btn-track').addEventListener('click', renderTrack);

    $('#order-form').addEventListener('submit', e => {
      e.preventDefault();
      const data = obtenerDatosFormulario();
      if(data.total <= 0){ alert('Selecciona al menos un producto.'); return; }

      const nuevo = {
        id: generarId(),
        fecha: new Date().toISOString(),
        estado: 'Por aprobar',
        ...data,
      };
      const pedidos = leerPedidos(); pedidos.push(nuevo); guardarPedidos(pedidos);
      renderTablaPedidos();

      alert(`¡Pedido generado! ID: ${nuevo.id}. Ahora confirma por WhatsApp.`);
      $('#track-id').value = nuevo.id; renderTrack();
      actualizarTotal();
    });

    renderTablaPedidos();

    // Footer year
    $('#year').textContent = new Date().getFullYear();

    // ======= RAYITO =======
    const rayitoWin = $('#rayito-window');
    $('#rayito-toggle').addEventListener('click', ()=>{ rayitoWin.style.display = 'flex'; rayitoWin.setAttribute('aria-hidden','false'); });
    $('#rayito-close').addEventListener('click', ()=>{ rayitoWin.style.display = 'none'; rayitoWin.setAttribute('aria-hidden','true'); });

    function rayitoResponder(text){
      const body = $('#rayito-body');
      const bubble = (msg, mine=false)=>{
        const div = document.createElement('div');
        div.className = 'rayito-msg';
        div.style.background = mine ? '#eef2ff' : 'var(--brand-soft)';
        div.textContent = msg; body.appendChild(div); body.scrollTop = body.scrollHeight;
      };
      bubble(text, true);
      const t = text.toLowerCase();
      let resp = 'Puedo ayudarte a ver combos, horario, métodos de pago y preguntas frecuentes.';
      if(t.includes('combo')) resp = 'Tenemos: Combo Estrella, Doble Estrella, Estelar y Colección Aura. Mira en Productos.';
      else if(t.includes('hora')) resp = 'Atendemos Lun–Vie de 9AM a 4PM.';
      else if(t.includes('pagar') || t.includes('pago')) resp = 'Puedes pagar por Transferencia o Efectivo. Confirmamos por WhatsApp.';
      else if(t.includes('whatsapp')) resp = 'Escríbenos al 099 537 2875 o usa el botón de WhatsApp.';
      setTimeout(()=> bubble(resp), 300);
    }

    $('[data-action="horario"]').addEventListener('click', ()=> rayitoResponder('Horario: Lun–Vie 9AM a 4PM.'));
    $('#rayito-send').addEventListener('click', ()=>{
      const input = $('#rayito-input'); if(!input.value.trim()) return; rayitoResponder(input.value.trim()); input.value='';
    });
    $('#rayito-input').addEventListener('keydown', e=>{ if(e.key==='Enter'){ e.preventDefault(); $('#rayito-send').click(); }});
  </script>
</body>
</html>
