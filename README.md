<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rayos de Luna | Bisutería Ecuador</title>
  <style>
    body { font-family: Arial, sans-serif; margin:0; padding:0; background:#fff8f0; color:#333;}
    header { background:#f48b9a; padding:15px; text-align:center; color:white;}
    nav { background:#ffd6e4; display:flex; justify-content:center; gap:20px; padding:10px 0;}
    nav a { text-decoration:none; color:#333; font-weight:bold; }
    section { padding:20px; display:none; }
    section.active { display:block; }
    h2 { color:#f48b9a; }
    .btn { background:#f48b9a; color:white; padding:10px 15px; border:none; cursor:pointer; border-radius:5px; }
    .combo { border:1px solid #f48b9a; padding:15px; margin:10px 0; border-radius:8px; }
    form input, form select { padding:8px; margin:5px 0; width:100%; box-sizing:border-box; }
    .pedido-status { margin-top:10px; font-weight:bold; }
    footer { background:#f48b9a; color:white; text-align:center; padding:15px; margin-top:20px;}
  </style>
</head>
<body>

<header>
  <a href="https://imgbb.com/"><img src="https://i.ibb.co/dJmSGh63/logo-Rayos-de-luna.png" alt="logo-Rayos-de-luna" border="0"></a>
  <h1>Rayos de Luna</h1>
  <p>Bisutería únicas de Ecuador con entregas a domicilio</p>
</header>

<nav>
  <a href="#" data-tab="inicio">Inicio</a>
  <a href="#" data-tab="nosotros">Nosotros</a>
  <a href="#" data-tab="productos">Productos</a>
  <a href="#" data-tab="pedidos">Pedidos</a>
  <a href="#" data-tab="politicas">Políticas</a>
  <a href="#" data-tab="contacto">Contacto</a>
  <a href="#" data-tab="faq">Preguntas Frecuentes</a>
</nav>

<section id="inicio" class="active">
  <h2>Bienvenido a Rayos de Luna</h2>
  <p>Somos una marca de Bisutería ecuatoriana, entregamos tus pedidos a domicilio y ofrecemos productos de alta calidad para resaltar tu estilo.</p>
<p>Ofrecemos joyas únicas y exclusivas para destacar tu estilo. Aquí cada detalle está pensado para ti. Encuentra productos únicos, de la mejor calidad y a precios que se ajustan a lo que buscas.</p>
<p>💖 Compra fácil, segura y sin complicaciones, desde la comodidad de tu casa.</p>
<p>👉 Solo elige tu favorito, haz tu pedido ¡y nosotros lo llevamos directo a tu puerta! 🚚
<p>📍Ecuador - Guayaquil</p>
</nav>

<section id="productos" 
  <h2>Productos</h2>
  <div class="combo">
      <img src="https://i.ibb.co/HD1bwv3t/tu-imagen.jpg" alt="Descripción de la imagen" width="500"> 
    <h3>Combo Estrella</h3>
    <p>Incluye: Un par de argollas</p>
    <button class="btn" onclick="irPedido('Combo Estrella', $10)">Comprar</button>
  </div>
  <div class="combo">
    <img src="https://i.ibb.co/7tM5jJ5K/imagen.jpg" alt="Descripción de la imagen" width="500"> 
    <h3>Combo Doble Estrella</h3>
    <p>Incluye: Un par de argollas + Una pulsera</p>
    <button class="btn" onclick="irPedido('Combo Doble Estrella', $15)">Comprar</button>
  </div>
  <div class="combo">
    <a href="https://imgbb.com/"><img src="https://i.ibb.co/1GvnrWB1/4.png" alt="4" border="0"></a>
    <h3>Combo Estelar</h3>
    <p>Incluye: Un juego de pulseras</p>
    <button class="btn" onclick="irPedido('Combo Estelar', $13)">Comprar</button>
  </div>
  <div class="combo">
    <img src="https://i.ibb.co/C3qcfPkk/tu-imagen.jpg" alt="Descripción de la imagen" width="500">
    <h3>Colección Aura</h3>
    <p>Un par de argollas únicas</p>
    <button class="btn" onclick="irPedido('Colección Aura', $10)">Comprar</button>
  </div>
</section>

<section id="pedidos" 
  <h2>Pedidos</h2>
  <form id="formPedido">
    <label>Nombre:</label>
    <input type="text" name="nombre" required>
    <label>Teléfono / WhatsApp:</label>
    <input type="text" name="telefono" required>
    <label>Producto:</label>
    <input type="text" id="producto" name="producto" readonly>
    <label>Precio:</label>
    <input type="number" id="precio" name="precio" readonly>
    <label>Cantidad:</label>
    <input type="number" id="cantidad" name="cantidad" value="1" min="1">
    <label>Método de pago:</label>
    <select name="pago" required>
      <option value="transferencia">Transferencia</option>
      <option value="efectivo">Efectivo</option>
    </select>
    <p>Total: $<span id="total">0</span></p>
    <button type="submit" class="btn">Generar Pedido</button>
  </form>
  <div id="seguimiento"></div>
</section>

<section id="politicas" 
  <h2>Políticas</h2>
  <h3>Privacidad</h3>
  <p>Cuidamos tu información personal con total responsabilidad. Los datos se usan solo para procesar pedidos y promociones.</p>
  <h3>Pedidos y Compras</h3>
  <p>Todos los pedidos se confirman por WhatsApp. Métodos de pago: transferencia o efectivo. Tiempo de entrega: 3 días hábiles.</p>
  <h3>Devoluciones y Cambios</h3>
  <p>Aceptamos devoluciones solo por defectos de fabricación, hasta 48h después de la entrega. Contacto: rayo_de_luna_13@hotmail.com</p>
</section>

<section id="contacto" 
  <h2>Contacto</h2>
  <p>Instagram & Facebook: @Rayos_de_luna_13</p>
  <p>Asistente virtual: Rayito ⚡</p>
  <p>Horario de atención: Lunes a Viernes 9AM - 4PM</p>
</section>

<section id="faq" 
  <h2>FAQ</h2>
  <p><strong>¿Cuáles son los combos?</strong> Combo Estrella, Doble Estrella, Estelar y la Colección Aura.</p>
  <p><strong>¿Cómo puedo pagar?</strong> Transferencia o efectivo.</p>
  <p><strong>Horario de atención:</strong> Lun-Vie 9AM - 4PM</p>
</section>

<footer>
  <p>© 2025 Rayos de Luna. Todos los derechos reservados.</p>
</footer>

<script>
  const tabs = document.querySelectorAll('nav a');
  const sections = document.querySelectorAll('section');

  tabs.forEach(tab => {
    tab.addEventListener('click', function(e){
      e.preventDefault();
      const target = this.dataset.tab;
      sections.forEach(sec => sec.classList.remove('active'));
      document.getElementById(target).classList.add('active');
    });
  });

  const form = document.getElementById('formPedido');
  const totalSpan = document.getElementById('total');
  const cantidadInput = document.getElementById('cantidad');
  let precioBase = 0;

  function irPedido(producto, precio){
    document.getElementById('producto').value = producto;
    document.getElementById('precio').value = precio;
    precioBase = precio;
    totalSpan.textContent = precio;
    document.getElementById('pedidos').classList.add('active');
    sections.forEach(sec => {
      if(sec.id !== 'pedidos') sec.classList.remove('active');
    });
  }

  cantidadInput.addEventListener('input', () => {
    let cantidad = parseInt(cantidadInput.value);
    totalSpan.textContent = precioBase * cantidad;
  });

  form.addEventListener('submit', (e) => {
    e.preventDefault();
    const nombre = form.nombre.value;
    const telefono = form.telefono.value;
    const producto = form.producto.value;
    const cantidad = form.cantidad.value;
    const total = totalSpan.textContent;
    const pago = form.pago.value;

    const seguimiento = document.getElementById('seguimiento');
    seguimiento.innerHTML = `
      <p class="pedido-status">Pedido Generado: ${producto} x${cantidad} - Total: $${total} - Pago: ${pago}</p>
      <p class="pedido-status">Estado del pedido: Por aprobar</p>
    `;
    alert('Pedido generado con éxito. Nos comunicaremos por WhatsApp.');
    form.reset();
    totalSpan.textContent = 0;
 
