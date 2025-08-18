
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Rayos de Luna | Joyas</title>
<style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #fff8f0; }
    header { background: #f48b9a; color: white; padding: 15px; text-align: center; }
    nav { display: flex; justify-content: center; background: #ffd6e4; flex-wrap: wrap; }
    nav button { background: transparent; border: none; padding: 15px 20px; cursor: pointer; font-weight: bold; }
    nav button:hover { background: #f48b9a; color: white; }
    section { display: none; padding: 20px; max-width: 1000px; margin: auto; }
    section.active { display: block; }
    .productos { display: flex; gap: 20px; flex-wrap: wrap; justify-content: center; }
    .producto { border: 1px solid #f48b9a; border-radius: 10px; padding: 10px; width: 220px; text-align: center; background: #fff0f5; }
    .producto img { width: 100%; border-radius: 10px; }
    .boton-compra { background: #f48b9a; color: white; border: none; padding: 10px; margin-top: 10px; cursor: pointer; border-radius: 5px; }
    .boton-compra:hover { background: #ffd6e4; color: #f48b9a; }
    footer { background: #f48b9a; color: white; text-align: center; padding: 15px; margin-top: 20px; }
    #rayito { position: fixed; bottom: 20px; right: 20px; background: #ffd6e4; padding: 15px; border-radius: 12px; width: 250px; box-shadow: 0 0 10px rgba(0,0,0,0.2); }
    #rayito h3 { margin-top: 0; }
    #rayito button { background: #f48b9a; color: white; border: none; padding: 8px 10px; cursor: pointer; border-radius: 5px; margin-top: 5px; width: 100%; }
    #rayito button:hover { background: #ffd6e4; color: #f48b9a; }
</style>
</head>
<body>

<header>
<a href="https://imgbb.com/"><img src="https://i.ibb.co/dJmSGh63/logo-Rayos-de-luna.png" alt="logo-Rayos-de-luna" border="0"></a>
    <h1>Rayos de Luna 💖</h1>
    <p>Bisutería únicas y especiales</p>
</header>

<nav>
    <button onclick="mostrarSeccion('inicio')">Inicio</button>
    <button onclick="mostrarSeccion('nosotros')">Nosotros</button>
    <button onclick="mostrarSeccion('productos')">Productos</button>
    <button onclick="mostrarSeccion('pedidos')">Pedidos</button>
    <button onclick="mostrarSeccion('politicas')">Políticas</button>
    <button onclick="mostrarSeccion('contacto')">Contacto</button>
    <button onclick="mostrarSeccion('faq')">FAQ</button>
</nav>

<!-- Inicio -->
<section id="inicio" class="active">
    <h2>Bienvenidos a Rayos de Luna </h2>
    <p>Ofrecemos joyas únicas y exclusivas para destacar tu estilo.</p>
    <p>Aquí cada detalle está pensado para ti. Encuentra productos únicos, de la mejor calidad y a precios que se ajustan a lo que buscas.</p>
     <p>💖 Compra fácil, segura y sin complicaciones, desde la comodidad de tu casa.</p>
     <p>👉 Solo elige tu favorito, haz tu pedido ¡y nosotros lo llevamos directo a tu puerta! 🚚✨</p>
      <p> 📍Ecuador - Guayaquil</p>


    <button class="boton-compra" onclick="mostrarSeccion('productos')">Ver catálogo</button>
    <button class="boton-compra" onclick="mostrarSeccion('pedidos')">Comprar</button>
    <button class="boton-compra" onclick="mostrarSeccion('contacto')">Contáctanos</button>
</section>

<!-- Nosotros -->
<section id="nosotros">
    <h2>Quiénes somos</h2>
    <p>En Rayos de Luna somos una marca de joyería apasionada por crear piezas únicas que reflejan elegancia, estilo y personalidad. Cada una de nuestras joyas está diseñada pensando en ti, para que puedas expresar tu esencia en cada momento especial.

Nos caracterizamos por combinar calidad, creatividad y atención personalizada , ofreciendo no solo productos, sino experiencias que iluminan tu día a día. Nuestra misión es acercarte joyas que enamoran y te hagan sentir especial en cada ocasión.</p>

<p><b>Misión:</b> Brindar piezas únicas y elegantes que realzan la belleza y personalidad de cada cliente, ofreciendo una experiencia de compra segura, accesible y cercana, con atención personalizada que genera confianza y satisfacción.</p>

  <p><b>Visión:</b> Convertirnos en la marca de bisutería online preferida a nivel nacional, reconocida por la calidad de nuestros productos, la creatividad de nuestros diseños y la conexión emocional con nuestros clientes, inspirando momentos especiales y memorables. </p>

 <p><b>Valores:</b>Calidad: Nos comprometemos a ofrecer productos duraderos y bien elaborados.</p>


<p>Creatividad: Cada pieza refleja originalidad y estilo.</p>


<p>Confianza: Atención cercana y honesta en cada compra.</p>


<p>Pasión: Amamos lo que hacemos y transmitimos esa pasión en nuestros productos.</p>


<p>Innovación: Buscamos siempre mejorar y sorprender a nuestros clientes con nuevas tendencias..</p>
</section>

<!-- Productos -->
<section id="productos">
    <h2>Productos / Combos</h2>
    <div class="productos">
        <div class="producto">
        <img src="https://i.ibb.co/HD1bwv3t/tu-imagen.jpg" alt="Descripción de la imagen" width="500">

 <h3>Combo Estrella</h3>
            <p>Un par de argollas</p>
            <p>$10</p>
            <button class="boton-compra" onclick="comprar('Combo Estrella')">Comprar</button>
        </div>
        <div class="producto">
            <img src="https://i.ibb.co/7tM5jJ5K/imagen.jpg" alt="Descripción de la imagen" width="500">
            
 <h3>Combo Doble Estrella</h3>
            <p>Un par de argollas + una pulsera</p>
            <p>$15</p>
            <button class="boton-compra" onclick="comprar('Combo Doble Estrella')">Comprar</button>
        </div>
        <div class="producto">
     <a href="https://imgbb.com/"><img src="https://i.ibb.co/1GvnrWB1/4.png" alt="4" border="0"></a>
            
   <h3>Combo Estelar</h3>
            <p>Dos pulseras a juego</p>
            <p>$13</p>
            <button class="boton-compra" onclick="comprar('Combo Estelar')">Comprar</button>
        </div>
        <div class="producto">
<img src="https://i.ibb.co/C3qcfPkk/tu-imagen.jpg" alt="Descripción de la imagen" width="500">
                 <h3>Colección Aura</h3>
            <p>Un par de argollas únicas</p>
            <p>$10</p>
            <button class="boton-compra" onclick="comprar('Colección Aura')">Comprar</button>
        </div>
    </div> <button type="submit">Confirmar Pedido</button>
  </form>

</section>

<!-- Pedidos -->
<section id="pedidos">
    <h2>Cómo comprar / Pedidos</h2>
    <p>Para realizar tu pedido, puedes usar nuestro WhatsApp o llenar el formulario:</p>
    <ul>

<li>Métodos de pago: Transferencia o efectivo</li>
<li>Envíos: Nacionales, según disponibilidad</li>
    </ul>
   <h1>Formulario de Pedido</h1>

  <form id="pedidoForm">
    <label>Producto:</label>
    <input type="text" id="producto" name="producto" readonly>

 <label>Precio:</label>
    <input type="text" id="precio" name="precio" readonly>

  <label>Nombre:</label>
    <input type="text" name="nombre" required>

<label>Dirección:</label>
    <input type="text" name="direccion" required>

<label>Teléfono:</label>
    <input type="text" name="telefono" required>

 <label>Cantidad:</label>
    <input type="number" id="cantidad" name="cantidad" value="1" min="1" required>

<label>Total:</label>
    <input type="text" id="total" name="total" readonly>


  <script>
    // Capturar los parámetros de la URL
    const urlParams = new URLSearchParams(window.location.search);
    const producto = urlParams.get("producto");
    const precio = parseFloat(urlParams.get("precio"));

    document.getElementById("producto").value = producto;
    document.getElementById("precio").value = `$${precio.toFixed(2)}`;
    document.getElementById("total").value = `$${precio.toFixed(2)}`;

    // Actualizar total cuando cambie cantidad
    document.getElementById("cantidad").addEventListener("input", function() {
      const cantidad = this.value;
      const total = precio * cantidad;
      document.getElementById("total").value = `$${total.toFixed(2)}`;
    });

    // Manejo del formulario
    document.getElementById("pedidoForm").addEventListener("submit", function(e) {
      e.preventDefault();
      alert("✅ Pedido realizado con éxito. Te contactaremos pronto.");
      window.location.href = "productos.html";
       
    </a>
</section>

<!-- Políticas -->
<section id="politicas">
    <h2>Políticas</h2>
    <h3>Política de Privacidad</h3>
    <p>Cuidamos tu información personal con total responsabilidad. Los datos se usan solo para procesar pedidos y promociones.</p>

 <h3>Pedidos y Compras</h3>
    <p>Todos los pedidos se confirman por WhatsApp. Métodos de pago: transferencia o efectivo. Tiempo de entrega: 3 días hábiles.</p>

<h3>Devoluciones y Cambios</h3>
    <p>Aceptamos devoluciones solo por defectos de fabricación, hasta 48h después de la entrega.</p>
</section>

<!-- Contacto -->
<section id="contacto">
    <h2>Contacto</h2>
    <p>Correo: <b>rayo_de_luna_13@hotmail.com</b></p>
    <p>Instagram & Facebook: <b>@Rayos_de_luna_13</b></p>
    <a href="https://wa.me/593995372875" target="_blank">
        <button class="boton-compra">WhatsApp</button>
    </a>
    <form>
        <input type="text" placeholder="Nombre" required><br><br>
        <input type="email" placeholder="Correo" required><br><br>
        <textarea placeholder="Mensaje" required></textarea><br><br>
        <button type="submit" class="boton-compra">Enviar</button>
    </form>
</section>

<!-- Preguntas Frecuentes -->
<section id="faq">
    <h2>Preguntas Frecuentes</h2>
    <p><b>¿Cuáles son los combos?</b> Combo Estrella, Doble Estrella, Estelar y la colección Aura.</p>
    <p><b>¿Cómo puedo pagar?</b> Transferencia o efectivo.</p>
    <p><b>¿Horario de atención?</b> Lun-Vie 9AM - 6PM.</p>
</section>

<!-- Asistente Rayito -->
 <a href="https://wa.me/0995372875" target="_blank" class="rayito-flotante">
   <button class="rayito-boton" onclick="window.open('https://wa.me/0995372875','_blank')">
    <img src="https://i.ibb.co/your-rayito-icon.png" alt="Rayito">
</button>
    <h3>Rayito ⚡</h3>
    <p>¡Hola! Soy Rayito, tu asistente virtual 😊 ¿En qué puedo ayudarte?</p>
    <button onclick="mostrarSeccion('productos')">Ver combos</button>
    <button onclick="alert('Nuestro horario es Lun-Vie 9AM-6PM')">Horario de atención</button>
    <button onclick="window.open('https://wa.me/593995372875','_blank')">WhatsApp</button>

<!-- Footer -->
<footer>
    <p>© 2025 Rayos de Luna  | Todos los derechos reservados</p>
</footer>

<script>
    function mostrarSeccion(id){
        document.querySelectorAll('section').forEach(sec => sec.classList.remove('active'));
        document.getElementById(id).classList.add('active');
    }

    function comprar(producto){
        window.open('https://wa.me/593995372875?text=Hola,+quiero+comprar+' + encodeURIComponent(producto),'_blank');
    }
</script>

</body>
</html>
