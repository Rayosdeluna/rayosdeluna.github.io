<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Rayos de Luna | Bisutería Ecuador</title>
<style>
  body { font-family: Arial, sans-serif; margin:0; padding:0; background:#fff8f0; color:#333;}
  header { background:#f48b9a; padding:20px; text-align:center; color:white;}
  nav { background:#ffd6e4; display:flex; justify-content:center; gap:20px; padding:10px 0;}
  nav a { text-decoration:none; color:#333; font-weight:bold; font-size:16px; }
  nav a:hover { text-decoration:underline; }
  section { padding:20px; display:none; }
  section.active { display:block; }
  h2, h3 { color:#f48b9a; }
  .btn { background:#f48b9a; color:white; padding:10px 15px; border:none; cursor:pointer; border-radius:5px; }
  .combo { border:1px solid #f48b9a; padding:15px; margin:10px 0; border-radius:8px; background:white;}
  form input, form select { padding:8px; margin:5px 0; width:100%; box-sizing:border-box; border-radius:5px; border:1px solid #ccc;}
  .pedido-status { margin-top:10px; font-weight:bold; color:#f48b9a; }
  footer { background:#f48b9a; color:white; text-align:center; padding:15px; margin-top:20px;}
  .total { font-weight:bold; font-size:18px; color:#f48b9a; }

  /* Asistente flotante */
  #asistente-container { position: fixed; bottom: 20px; right: 20px; z-index: 1000; }
  #asistente {
    background: #f48b9a;
    color: white;
    font-size: 30px;
    text-align: center;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    line-height: 60px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    cursor: pointer;
    transition: transform 0.2s;
  }
  #asistente:hover { transform: scale(1.1); }

  #chatRayito {
    display: none;
    background: white;
    border: 2px solid #f48b9a;
    border-radius: 10px;
    padding: 15px;
    margin-bottom: 10px;
    width: 220px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
  }
  #chatRayito p { margin: 0 0 10px 0; color:#f48b9a; font-weight:bold; }
  #chatRayito button {
    display: block;
    width: 100%;
    margin: 5px 0;
    padding: 8px;
    border: none;
    background: #f48b9a;
    color: white;
    border-radius: 5px;
    cursor: pointer;
  }
  #chatRayito button:hover { background:#d96c86; }


<header>
  <h1>Rayos de Luna</h1>
  <p>Joyas únicas de Ecuador con entregas a domicilio</p>
</header>

<a href="https://imgbb.com/"> <img src="https://i.ibb.co/dJmSGh63/logo-Rayos-de-luna.png" alt="logo-Rayos-de-luna" border="0"></a> 
<nav>
  <a href="#" data-tab="inicio">Inicio</a>
  <a href="#" data-tab="nosotros">Nosotros</a>
  <a href="#" data-tab="productos">Productos</a>
  <a href="#" data-tab="pedidos">Pedidos</a>
  <a href="#" data-tab="politicas">Políticas</a>
  <a href="#" data-tab="contacto">Contactos</a>
  <a href="#" data-tab="faq">FAQ</a>
</nav>

<section id="inicio" class="active">
  <h2>Bienvenido a Rayos de Luna</h2>
  <p>Somos una marca de bisutería ecuatoriana con entregas a domicilio.</p>
  <p>Ofrecemos piezas únicas y esclusivas para destacar tu estilo</p>
  <p>💖 Compra fácil, segura y sin complicaciones, desde la comodidad de tu casa.</p>
<p>👉 Solo elige tu favorito, haz tu pedido ¡y nosotros lo llevamos directo a tu puerta! 🚚
<p>📍Ecuador - Guayaquil</p>

</section>

<section id="nosotros">
  <h2>Nosotros</h2>
  <h3>Misión</h3>
  <p>Brindar piezas únicas y elegantes que realzan la belleza y personalidad de cada cliente, ofreciendo una experiencia de compra segura, 
    accesible y cercana, con atención personalizada que genera confianza y satisfacción.</p>
  <h3>Visión</h3>
  <p>Convertirnos en la marca de bisutería online preferida a nivel nacional, reconocida por la calidad de nuestros productos, la creatividad de 
    nuestros diseños y la conexión emocional con nuestros clientes, inspirando momentos especiales y memorables.</p>
  <h3>Valores</h3>
  <p>Valores: Calidad: Nos comprometemos a ofrecer productos duraderos y bien elaborados.

Creatividad: Cada pieza refleja originalidad y estilo.

Confianza: Atención cercana y honesta en cada compra.

Pasión: Amamos lo que hacemos y transmitimos esa pasión en nuestros productos.

Innovación: Buscamos siempre mejorar y sorprender a nuestros clientes con nuevas tendencias.</p>
</section>

<section id="productos">
  <h2>Productos</h2>
  <div class="combo">
      <img src="https://i.ibb.co/HD1bwv3t/tu-imagen.jpg" alt="Descripción de la imagen" width="500">
    <h3>Combo Estrella</h3>
    <p>Incluye: Un par de argollas</p>
    <button class="btn" onclick="irPedido('Combo Estrella', 15)">Comprar - $15</button>
  </div>
  <div class="combo">
   <img src="https://i.ibb.co/7tM5jJ5K/imagen.jpg" alt="Descripción de la imagen" width="500">
    <h3>Combo Doble Estrella</h3>
    <p>Incluye: Un par de argollas + Una pulsera</p>
    <button class="btn" onclick="irPedido('Combo Doble Estrella', 25)">Comprar - $25</button>
  </div>
  <div class="combo">
   <a href="https://imgbb.com/"><img src="https://i.ibb.co/1GvnrWB1/4.png" alt="4" border="0"></a> 
    <h3>Combo Estelar</h3>
    <p>Incluye: Un juego de pulseras</p>
    <button class="btn" onclick="irPedido('Combo Estelar', 20)">Comprar - $20</button>
  </div>
  <div class="colección">
   <img src="https://i.ibb.co/C3qcfPkk/tu-imagen.jpg" alt="Descripción de la imagen" width="500">
    <h3>Colección Aura</h3>
    <p>Un par de argollas únicas</p>
    <button class="btn" onclick="irPedido('Colección Aura', 30)">Comprar - $30</button>
  </div>
</section>

<section id="pedidos">
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
    <p>Total: $<span id="total" class="total">0</span></p>
    <button type="submit" class="btn">Generar Pedido</button>
  </form>
  <div id="seguimiento"></div>
</section>

<section id="politicas">
  <h2>Políticas</h2>
  <h3>Privacidad</h3>
  <p>Cuidamos tu información personal con total responsabilidad.</p>
  <h3>Pedidos y Compras</h3>
  <p>Todos los pedidos se confirman por WhatsApp. Métodos de pago: transferencia o efectivo. Tiempo de entrega: 3 días hábiles.</p>
  <h3>Devoluciones y Cambios</h3>
  <p>Aceptamos devoluciones solo por defectos de fabricación, hasta 48h después de la entrega.</p>
</section>

<section id="contacto">
  <h2>Contactos</h2>
  <p>Instagram & Facebook: @Rayos_de_luna_13</p>
  <p>Asistente virtual: Rayito ⚡</p>
  <p>Horario de atención: Lunes a Viernes 9AM - 4PM</p>
</section>

<section id="faq">
  <h2>Preguntas Frecuentes</h2>
  <p><strong>¿Cuáles son los combos?</strong> Combo Estrella, Doble Estrella, Estelar y la Colección Aura.</p>
  <p><strong>¿Cómo puedo pagar?</strong> Transferencia o efectivo.</p>
  <p><strong>Horario de atención:</strong> Lun-Vie 9AM - 4PM</p>
</section>

<footer>
  <p>© 2025 Rayos de Luna. Todos los derechos reservados.</p>
</footer>

<!-- Asistente flotante -->
<div id="asistente-container">
  <div id="asistente">⚡</div>
  <div id="chatRayito">
    <p>¡Hola! Soy Rayito ⚡. ¿En qué puedo ayudarte?</p>
    <button onclick="mostrarCombos()">Ver combos</button>
    <button onclick="mostrarHorario()">Horario de atención</button>
    <button onclick="abrirWhatsApp()">WhatsApp</button>
  </div>
</div>

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

// Función para llenar formulario de pedidos desde botón de producto
function irPedido(nombre, precio){
  document.getElementById('producto').value = nombre;
  document.getElementById('precio').value = precio;
  document.getElementById('total').textContent = precio;
  sections.forEach(sec => sec.classList.remove('active'));
  document.getElementById('pedidos').classList.add('active');
}

// Actualizar total si cambia la cantidad
document.getElementById('cantidad').addEventListener('input', function(){
  const precio = parseFloat(document.getElementById('precio').value) || 0;
  const cantidad = parseInt(this.value) || 1;
  document.getElementById('total').textContent = precio * cantidad;
});

// Asistente Rayito
const asistente = document.getElementById('asistente');
const chatRayito = document.getElementById('chatRayito');

asistente.addEventListener('click', () => {
  chatRayito.style.display = chatRayito.style.display === 'block' ? 'none' : 'block';
});

function mostrarCombos() {
  chatRayito.innerHTML = `
    <p>Estos son nuestros combos:</p>
    <ul>
      <li>Combo Estrella</li>
      <li>Combo Doble Estrella</li>
      <li>Combo Estelar</li>
      <li>Colección Aura</li>
    </ul>
    <button onclick="cerrarChat()">Cerrar</button>
  `;
}

function mostrarHorario() {
  chatRayito.innerHTML = `
    <p>Horario de atención:</p>
    <p>Lunes a Viernes 9AM - 4PM</p>
    <button onclick="cerrarChat()">Cerrar</button>
  `;
}

function abrirWhatsApp() {
  window.open('https://wa.me/5939995372875', '_blank');
}

function cerrarChat() {
  chatRayito.style.display = 'none';
  chatRayito.innerHTML = `
    <p>¡Hola! Soy Rayito ⚡. ¿En qué puedo ayudarte?</p>
    <button onclick="mostrarCombos()">Ver combos</button>
    <button onclick="mostrarHorario()">Horario de atención</button>
    <button onclick="abrirWhatsApp()">WhatsApp</button>
  `;
}
</script>
</body>
</html>


