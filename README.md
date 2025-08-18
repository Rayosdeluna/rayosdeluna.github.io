<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Rayos de Luna | Bisutería Ecuador</title>
<style>
  body { font-family: Arial, sans-serif; margin:0; padding:0; background:#fff8f9; color:#333; }
  header { background:#f48b9a; color:white; text-align:center; padding:20px; }
  nav { background:#ffd6e4; text-align:center; padding:10px 0; }
  nav a { color:#333; text-decoration:none; margin:0 15px; font-weight:bold; }
  section { padding:20px; max-width:1000px; margin:0 auto; }
  .producto { border:1px solid #e3e3e3; border-radius:12px; padding:15px; margin:15px 0; background:#fff; }
  button { background:#f48b9a; color:white; border:none; padding:10px 20px; border-radius:8px; cursor:pointer; font-weight:bold; }
  button:hover { background:#e36b81; }
  footer { background:#333; color:white; text-align:center; padding:20px; margin-top:30px; }
  .faq h3 { margin-bottom:5px; }
  input, textarea, select { width:100%; padding:8px; margin-top:5px; margin-bottom:15px; border-radius:6px; border:1px solid #ccc; }
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
  <a href="#contacto">Contacto</a>
  <a href="#faq">Preguntas Frecuentes</a>
</nav>

<section id="inicio">
  <h2>Bienvenidos</h2>
  <p>Somos Rayos de Luna, una bisutería ecuatoriana que ofrece piezas únicas, elegantes y de calidad. Disfruta de nuestras entregas rápidas y seguras en todo el país.</p>
</section>

<section id="quienes">
  <h2>Quiénes Somos</h2>
  <p><strong>Misión:</strong> Ofrecer bisutería de calidad que inspire confianza y elegancia.</p>
  <p><strong>Visión:</strong> Ser reconocidos como la bisutería ecuatoriana de mayor prestigio por nuestro diseño y cercanía con los clientes.</p>
  <p><strong>Valores:</strong> Confianza, Responsabilidad y Creatividad.</p>
</section>

<section id="productos">
  <h2>Nuestros Productos</h2>
  <div class="producto"> 
      <img src="https://i.ibb.co/HD1bwv3t/tu-imagen.jpg" alt="Descripción de la imagen" width="500"> 
    <h3>Combo Estrella</h3>
    <p>Un par de argollas.</p>
    <button onclick="agregarPedido('Combo Estrella', 20)">Comprar</button>
  </div>
  <div class="producto">
    <img src="https://i.ibb.co/7tM5jJ5K/imagen.jpg" alt="Descripción de la imagen" width="500"> 
    <h3>Combo Doble Estrella</h3>
    <p>Un par de argollas + una pulsera.</p>
    <button onclick="agregarPedido('Combo Doble Estrella', 35)">Comprar</button>
  </div>
  <div class="producto">
    <a href="https://imgbb.com/"><img src="https://i.ibb.co/1GvnrWB1/4.png" alt="4" border="0"></a> 
    <h3>Combo Estelar</h3>
    <p>Un juego de pulseras.</p>
    <button onclick="agregarPedido('Combo Estelar', 25)">Comprar</button>
  </div>
  <div class="producto">
    <img src="https://i.ibb.co/C3qcfPkk/tu-imagen.jpg" alt="Descripción de la imagen" width="500">
    <h3>Colección Aura</h3>
    <p>Un par de argollas únicas.</p>
    <button onclick="agregarPedido('Colección Aura', 40)">Comprar</button>
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
<section id="contacto">
  <h2>Contacto</h2>
  <p><strong>Correo:</strong> rayo_de_luna_13@hotmail.com</p>
  <p><strong>Instagram & Facebook:</strong> @Rayos_de_luna_13</p>
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


<div class="chatbox">
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
  <p>&copy; 2025 Rayos de Luna | Bisutería Ecuador</p>
</footer>

<script>
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


