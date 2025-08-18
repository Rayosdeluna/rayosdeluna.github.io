
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

