<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Rayos de Luna | Bisutería Ecuador</title>
<style>
  body { font-family: Arial, sans-serif; margin:0; padding:0; background:#fff8f9; color:#333; }
  header { background:#f48b9a; color:white; text-align:center; padding:20px; }
  nav { background:#ffd6e4; text-align:center; padding:10px 0; position: sticky; top:0; }
  nav a { color:#333; text-decoration:none; margin:0 15px; font-weight:bold; }
  section { padding:20px; max-width:1000px; margin:0 auto; }
  .producto { border:1px solid #e3e3e3; border-radius:12px; padding:15px; margin:15px 0; background:#fff; }
  button { background:#f48b9a; color:white; border:none; padding:10px 20px; border-radius:8px; cursor:pointer; font-weight:bold; }
  button:hover { background:#e36b81; }
  footer { background:#333; color:white; text-align:center; padding:20px; margin-top:30px; }
  .faq h3 { margin-bottom:5px; }
  input, textarea, select { width:100%; padding:8px; margin-top:5px; margin-bottom:15px; border-radius:6px; border:1px solid #ccc;}
  ul { padding-left:20px; }
  .chatbox { position:fixed; bottom:20px; right:20px; width:250px; background:#ffd6e4; border-radius:15px; padding:15px; box-shadow:0 4px 6px rgba(0,0,0,0.2); }
</style>
</head>
<body>

<header>
  <a href="https://imgbb.com/"><img src="https://i.ibb.co/dJmSGh63/logo-Rayos-de-luna.png" alt="logo-Rayos-de-luna" border="0"></a>
  <h1>Rayos de Luna ✨</h1>
  <p>Bisutería desde Ecuador con entregas a domicilio</p>
</header>

<nav>
  <a href="#inicio">Inicio</a>
  <a href="#quienes">Quiénes Somos</a>
  <a href="#productos">Productos</a>
  <a href="#pedidos">Pedidos</a>
  <a href="#politicas">Políticas</a>
  <a href="#faq">Preguntas Frecuentes</a>
  <a href="#contacto">Contacto</a>
</nav>

<section id="inicio">
  <h2>Bienvenidos a Rayos de luna</h2>
  <p>Somos Rayos de Luna, una bisutería ecuatoriana que ofrece piezas únicas, elegantes y de calidad. Disfruta de nuestras entregas rápidas y seguras en todo el país.</p>
</section>

<section id="nosotros">
  <h2>Nosotros</h2>
   <p><strong>¿Quiénes somos?:</strong> En Rayos de Luna somos marca de bisutería apasionada por crear puezas únicas que reflejan elegancia, estilo y personalidad. Cada una de nuestras piezas está diseñada pensando en ti, para que puedas expresar tú esencia en cada momento especial. Nos caraterizamos por combinar calidad, creatividad y atención personalizada, ofrecemos no solo un producto, sino experiencias que iluminan tu día a día. Nuestra misión es es acercarte a piezas que enamoran y te hagan sentir especial en cada ocasión.</p>
  <p><strong>Misión:</strong> Brindar piezas únicas y elegantes que realzan la belleza y personalidad de cada cliente, ofreciendo una experiencia de compra segura, accesible y cercana, con atención personalizada que genera confianza y satisfacción.</p>
  <p><strong>Visión:</strong> Convertirnos en la marca de bisutería online preferida a nivel nacional, reconocida por la calidad de nuestros productos, la creatividad de nuestros diseños y la conexión emocional con nuestros clientes, inspirando momentos especiales y memorables.</p>
  <p><strong>Valores:</strong> Calidad: Nos comprometemos a ofrecer productos duraderos y bien elaborados.
Creatividad: Cada pieza refleja originalidad y estilo.
Confianza: Atención cercana y honesta en cada compra.
Pasión: Amamos lo que hacemos y transmitimos esa pasión en nuestros productos.
Innovación: Buscamos siempre mejorar y sorprender a nuestros clientes con nuevas tendencias.</p>
</section>

<section id="productos">
  <h2>Nuestros Productos</h2>
  <div class="producto">
    <h3>Combo Estrella</h3>
    <a href="https://imgbb.com/"><img src="https://i.ibb.co/bgqCwhDs/combo-estrella.png" alt="combo-estrella" border="0"></a>
    <p>Un par de argollas.</p>
    <button onclick="agregarPedido('Combo Estrella', 10)">Comprar</button>
  </div>
  <div class="producto">
    <a href="https://imgbb.com/"><img src="https://i.ibb.co/Xx0gjZgt/2.png" alt="2" border="0"></a>
    <h3>Combo Doble Estrella</h3>
    <p>Un par de argollas + una pulsera.</p>
    <button onclick="agregarPedido('Combo Doble Estrella', 15)">Comprar</button>
  </div>
  <div class="producto">
    <a href="https://imgbb.com/"><img src="https://i.ibb.co/1GvnrWB1/4.png" alt="4" border="0"></a> 
    <h3>Combo Estelar</h3>
    <p>Un juego de pulseras.</p>
    <button onclick="agregarPedido('Combo Estelar', 13)">Comprar</button>
  </div>
  <div class="producto">
    <a href="https://imgbb.com/"><img src="https://i.ibb.co/8LJCHYWW/3.png" alt="3" border="0"></a>
    <h3>Colección Aura</h3>
    <p>Un par de argollas únicas.</p>
    <button onclick="agregarPedido('Colección Aura', 10)">Comprar</button>
  </div>
</section>

<section id="pedidos">
  <h2>Realiza tu Pedido</h2>
  <form id="formPedido">
    <label>Nombre Completo:</label>
    <input type="text" id="nombre" required>
    <label>Teléfono:</label>
    <input type="tel" id="telefono" required>
    <label>Dirección:</label>
    <textarea id="direccion" required></textarea>
    <label>Método de pago:</label>
    <select id="pago">
      <option value="Transferencia">Transferencia</option>
      <option value="Efectivo">Efectivo</option>
    </select>
    <h3>Resumen de compra:</h3>
    <ul id="listaPedidos"></ul>
    <p><strong>Total: $<span id="total">0</span></strong></p>
    <button type="submit">Confirmar Pedido</button>
  </form>
  <div id="seguimiento" style="display:none;">
    <h3>Estado de tu pedido:</h3>
    <p id="estadoPedido">Por aprobar ✅</p>
  </div>
</section>

<section id="politicas">
  <h2>Políticas</h2>
  <h3>Privacidad</h3>
  <p>Cuidamos tu información personal con total responsabilidad. Los datos se usan solo para procesar pedidos y promociones.</p>
  <h3>Pedidos y Compras</h3>
  <p>Todos los pedidos se confirman por WhatsApp. Métodos de pago: transferencia o efectivo. Tiempo de entrega: 3 días hábiles.</p>
  <h3>Devoluciones y Cambios</h3>
  <p>Aceptamos devoluciones solo por defectos de fabricación, hasta 48h después de la entrega.</p>
</section>

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

<section id="contacto">
  <h2>Contacto</h2>
  <p><strong>Correo:</strong> rayo_de_luna_13@hotmail.com</p>
  <p><strong>Instagram & Facebook:</strong> @Rayos_de_luna_13</p>
</section>

<div class="chatbox">
  <h4>🤖 Rayito - Tu asistente virtual</h4>
  <p>Hola, soy Rayito. ¿Cómo te puedo ayudar?</p>
  <ul>
    <li><a href="#productos">Ver Combos</a></li>
    <li><a href="#faq">Preguntas Frecuentes</a></li>
    <li><a href="#contacto">Contáctanos</a></li>
  </ul>
  <p>O escríbenos directamente por WhatsApp 📲</p>
</div>

<footer>
  <p>&copy; 2025 Rayos de Luna | Bisutería Ecuador</p>
</footer>

<script>
let pedidos = [];
let total = 0;

function agregarPedido(producto, precio) {
  pedidos.push({producto, precio});
  total += precio;
  mostrarPedidos();
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

document.getElementById("formPedido").addEventListener("submit", function(e){
  e.preventDefault();
  if(pedidos.length === 0){
    alert("Agrega al menos un producto antes de confirmar tu pedido.");
    return;
  }
  document.getElementById("seguimiento").style.display = "block";
  document.getElementById("estadoPedido").textContent = "Por aprobar ✅";
  alert("Tu pedido ha sido registrado. Te contactaremos por WhatsApp para confirmarlo.");
});
</script>
        
