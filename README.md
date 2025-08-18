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
    form input, form textarea, form select { width: 100%; padding: 8px; margin: 8px 0; border: 1px solid #f48b9a; border-radius: 5px; }
</style>
</head>
<body>

<header>
    <img src="https://i.ibb.co/dJmSGh63/logo-Rayos-de-luna.png" alt="logo-Rayos-de-luna" width="80">
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
    <button class="boton-compra" onclick="mostrarSeccion('productos')">Ver catálogo</button>
    <button class="boton-compra" onclick="mostrarSeccion('pedidos')">Comprar</button>
</section>

<!-- Productos -->
<section id="productos">
    <h2>Productos / Combos</h2>
    <div class="productos">
        <div class="producto">
          <img src="combo-estrella.jpg" alt="Combo Estrella"> <h3>Combo Estrella</h3> <p>Un par de argollas</p> <p>$10</p> 
            <button class="boton-compra" onclick="comprar('Combo Estrella')">Comprar</button> </div> <div
                                                                                                                                                                                                                        class="producto"><img src="combo-doble-estrella.jpg" alt="Combo Doble Estrella"> <h3>Combo Doble Estrella</h3> <p>Un par de argollas + una pulsera</p> <p>$15</p>
                <button class="boton-compra" onclick="comprar('Combo Doble Estrella')">Comprar</button> </div> <div class="producto"> 
                    <img src="combo-estelar.jpg" alt="Combo Estelar"> <h3>Combo Estelar</h3> <p>Dos pulseras a juego</p> <p>$13</p>
                    <button class="boton-compra" onclick="comprar('Combo Estelar')">Comprar</button> </div> <div
                                                                                                                                                                                                                                class="producto"> <img src="aura.jpg" alt="Colección Aura">
                        <h3>Colección Aura</h3> <p>Un par de argollas únicas</p> <p>$10</p> <button class="boton-compra" onclick="comprar('Colección Aura')">Comprar</button>

<!-- Pedidos -->
<section id="pedidos">
    <h2>Formulario de Pedido</h2>
    <form id="form-pedido">
        <label>Producto seleccionado:</label>
        <input type="text" id="producto" name="producto" readonly required>
        
 <label>Total a pagar:</label>
        <input type="text" id="total" name="total" readonly required>

   <label>Nombre completo:</label>
        <input type="text" name="nombre" required>

  <label>Correo electrónico:</label>
        <input type="email" name="correo" required>

   <label>Dirección de entrega:</label>
        <textarea name="direccion" required></textarea>

   <label>Método de pago:</label>
        <select name="pago" required>
            <option value="Transferencia">Transferencia</option>
            <option value="Efectivo">Efectivo</option>
        </select>

  <button type="submit" class="boton-compra">Enviar pedido</button>
    </form>
</section>

<!-- Footer -->
<footer>
    <p>© 2025 Rayos de Luna ⚡ | Todos los derechos reservados</p>
</footer>
