<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rayos de Luna | Joyas</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #ffd6e4;
      margin: 0;
      padding: 0;
      text-align: center;
    }
    header {
      background-color: #f48b9a;
      padding: 20px;
    }
    header img {
      max-width: 200px;
    }
    section {
      padding: 20px;
    }
    .productos {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 20px;
    }
    .producto {
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      padding: 15px;
    }
    .producto img {
      width: 100%;
      border-radius: 12px;
    }
    footer {
      background-color: #f48b9a;
      color: white;
      padding: 20px;
      margin-top: 20px;
    }
    h2 {
      color: #333;
    }
  </style>
</head>
<body>
  <!-- LOGO -->
  <header>
    <a href="https://imgbb.com/">
      <img src="https://i.ibb.co/dJmSGh63/logo-Rayos-de-luna.png" alt="Logo Rayos de Luna">
    </a>
  </header>

  <!-- PRODUCTOS -->
  <section>
    <h2>Nuestra Colección</h2>
    <div class="productos">
      <div class="producto">
        <img src="https://i.ibb.co/HD1bwv3t/tu-imagen.jpg" alt="Combo Estrella">
        <h3>Combo Estrella</h3>
      </div>
      <div class="producto">
        <img src="https://i.ibb.co/7tM5jJ5K/imagen.jpg" alt="Combo Doble Estrella">
        <h3>Combo Doble Estrella</h3>
      </div>
      <div class="producto">
        <a href="https://imgbb.com/">
          <img src="https://i.ibb.co/1GvnrWB1/4.png" alt="Combo Estelar">
        </a>
        <h3>Combo Estelar</h3>
      </div>
      <div class="producto">
        <img src="https://i.ibb.co/C3qcfPkk/tu-imagen.jpg" alt="Aura">
        <h3>Colección Aura</h3>
      </div>
    </div>
  </section>

  <!-- PREGUNTAS FRECUENTES -->
  <section>
    <h2>Preguntas Frecuentes</h2>
    <p><strong>¿Cómo realizo mi pedido?</strong> Escríbenos por WhatsApp y te ayudamos con el proceso.</p>
    <p><strong>¿Hacen envíos?</strong> Sí, realizamos envíos a todo el país.</p>
  </section>

  <!-- POLÍTICA -->
  <section>
    <h2>Política de la Tienda</h2>
    <p>Por favor escríbenos antes de realizar tu compra para ayudarte con el número de cuenta y confirmar disponibilidad.</p>
  </section>

  <!-- CONTACTO -->
  <footer>
    <h2>Contáctanos</h2>
    <p>WhatsApp: <a href="https://wa.me/593995372875" style="color:white;">0995372875</a></p>
    <p>Instagram: @RayosDeLuna</p>

<div class="chatbox">
  <h4>⚡ Rayito - Tu asistente virtual</h4>
  <p>Hola, soy Rayito ⚡. ¿Cómo te puedo ayudar?</p>
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
        
