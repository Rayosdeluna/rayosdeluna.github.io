<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Rayos de Luna | Joyas</title>
  <meta name="description" content="Rayos de Luna – Diseñamos joyas con cuidado y amor." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Playfair+Display:ital,wght@0,600;1,600&display=swap" rel="stylesheet">
  <style>
    :root{
      --pink:#f48b9a;
      --blush:#ffd6e4;
      --ink:#1f2937;
      --muted:#6b7280;
      --radius:18px;
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:Poppins,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,'Helvetica Neue',Arial,sans-serif;color:var(--ink);background:var(--blush);} 
    img{max-width:100%;display:block}
    a{color:inherit;text-decoration:none}
    .container{max-width:1100px;margin:0 auto;padding:0 20px}
    header{position:sticky;top:0;z-index:50;background:rgba(255,214,228,.85);backdrop-filter:saturate(1.2) blur(6px);border-bottom:1px solid rgba(244,139,154,.35)}
    .nav{display:flex;align-items:center;gap:16px;padding:14px 0}
    .brand{display:flex;align-items:center;gap:12px}
    .brand img{width:44px;height:44px;border-radius:50%;border:1px solid var(--pink);object-fit:cover}
    .brand h1{font-size:18px;margin:0;font-weight:600;letter-spacing:.3px}
    .brand p{margin:0;color:var(--muted);font-size:12px;margin-top:-2px}
    .navlinks{margin-left:auto;display:flex;gap:14px}
    .btn{display:inline-flex;align-items:center;justify-content:center;gap:8px;padding:10px 16px;border-radius:999px;border:1px solid rgba(244,139,154,.5);background:white;cursor:pointer;font-weight:600}
    .btn-primary{background:var(--pink);color:white;border-color:var(--pink)}
    .btn-outline{background:white;color:var(--pink)}
    .btn-link{border:none;background:transparent;color:var(--ink);padding:8px}
    .hero{padding:56px 0}
    .hero-grid{display:grid;grid-template-columns:1.2fr .8fr;gap:28px;align-items:center}
    .title{font-family:"Playfair Display",serif;font-weight:600;font-size:46px;line-height:1.1;margin:0}
    .subtitle{color:var(--muted);margin:12px 0 18px}
    .tags{display:flex;gap:10px;flex-wrap:wrap}
    .tag{background:rgba(244,139,154,.12);color:#a31f3b;border:1px solid rgba(244,139,154,.35);padding:6px 10px;border-radius:999px;font-size:12px}
    .hero-card{position:relative;border-radius:var(--radius);overflow:hidden;border:1px solid rgba(244,139,154,.35);box-shadow:0 10px 30px rgba(244,139,154,.2)}
    .hero-card img{height:100%;width:100%;object-fit:cover}
    .section{padding:36px 0}
    .section h2{font-size:28px;margin:0 0 14px;color:var(--pink)}
    .grid{display:grid;gap:18px}
    .grid-3{grid-template-columns:repeat(3,1fr)}
    .grid-2{grid-template-columns:repeat(2,1fr)}
    @media(max-width:920px){.hero-grid{grid-template-columns:1fr}.grid-3{grid-template-columns:repeat(2,1fr)}}
    @media(max-width:640px){.grid-3,.grid-2{grid-template-columns:1fr}.title{font-size:34px}}
    .card{border:1px solid rgba(244,139,154,.35);border-radius:var(--radius);background:white;overflow:hidden;display:flex;flex-direction:column}
    .card-img{aspect-ratio:1/1;object-fit:cover;background:#fff4f7}
    .card-body{padding:14px}
    .card h3{margin:0 0 6px;font-size:18px;color:var(--pink)}
    .card p{margin:0;color:var(--muted);font-size:14px}
    .card .price{margin-top:8px;font-weight:700;font-size:18px;color:var(--ink)}
    .card .actions{margin-top:12px;display:flex;gap:10px}
    .about{display:grid;grid-template-columns:1fr 1fr;gap:24px;align-items:center}
    @media(max-width:920px){.about{grid-template-columns:1fr}}
    footer{padding:28px 0;color:var(--muted)}
    .wa-float{position:fixed;right:16px;bottom:16px;background:var(--pink);color:white;border-radius:999px;padding:12px 16px;box-shadow:0 8px 30px rgba(244,139,154,.55);display:flex;align-items:center;gap:10px;font-weight:700;z-index:60}
    .wa-float svg{width:18px;height:18px;fill:white}
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">
        <img src="logo.png" alt="Rayos de Luna" />
        <div>
          <h1>Rayos de Luna</h1>
          <p>Diseñamos joyas con cuidado y amor</p>
        </div>
      </div>
      <nav class="navlinks">
        <a class="btn-link" href="#combos">Combos</a>
        <a class="btn-link" href="#aura">Colección Aura</a>
        <a class="btn-link" href="#catalogo">Catálogo</a>
        <a class="btn btn-outline" id="btnHeaderWA" href="#">WhatsApp</a>
      </nav>
    </div>
  </header>

  <main>
    <!-- HERO -->
    <section class="hero">
      <div class="container hero-grid">
        <div>
          <h2 class="title">Brilla con la magia lunar</h2>
          <p class="subtitle">Piezas delicadas, materiales de calidad y diseño atemporal. Cada detalle pensado para iluminar tu estilo.</p>
          <div class="tags">
            <span class="tag">Hipoalergénico</span>
            <span class="tag">Hecho con amor</span>
            <span class="tag">Garantía 30 días</span>
          </div>
          <div style="margin-top:18px;display:flex;gap:10px;flex-wrap:wrap">
            <a class="btn btn-primary" href="#catalogo">Ver catálogo</a>
            <a class="btn btn-outline" id="btnHeroWA" href="#">Pedir por WhatsApp</a>
          </div>
        </div>
        <div class="hero-card">
          <img src="hero.jpg" alt="Joyas Rayos de Luna" />
        </div>
      </div>
    </section>

    <!-- COMBOS -->
    <section id="combos" class="section">
      <div class="container">
        <h2>Combos</h2>
        <div class="grid grid-3">
          <article class="card">
            <img class="card-img" src="combo-estrellas.jpg" alt="Combo Estrellas" />
            <div class="card-body">
              <h3>Combo Estrellas</h3>
              <p>Un par de argollas medianas/pequeñas.</p>
              <div class="actions">
                <a class="btn btn-primary" data-product="Combo Estrellas" href="#">Consultar por WhatsApp</a>
              </div>
            </div>
          </article>
          <article class="card">
            <img class="card-img" src="combo-doble-estrella.jpg" alt="Combo Doble Estrella" />
            <div class="card-body">
              <h3>Combo Doble Estrella</h3>
              <p>Un par de argollas + una pulsera.</p>
              <div class="actions">
                <a class="btn btn-primary" data-product="Combo Doble Estrella" href="#">Consultar por WhatsApp</a>
              </div>
            </div>
          </article>
          <article class="card">
            <img class="card-img" src="combo-estelar.jpg" alt="Combo Estelar" />
            <div class="card-body">
              <h3>Combo Estelar</h3>
              <p>Dos pulseras a juego.</p>
              <div class="actions">
                <a class="btn btn-primary" data-product="Combo Estelar" href="#">Consultar por WhatsApp</a>
              </div>
            </div>
          </article>
        </div>
      </div>
    </section>

    <!-- COLECCIÓN AURA -->
    <section id="aura" class="section" style="background:white">
      <div class="container">
        <h2>Colección Aura</h2>
        <div class="grid grid-2">
          <article class="card">
            <img class="card-img" src="aura-1.jpg" alt="Colección Aura" />
            <div class="card-body">
              <h3>Pieza Aura 01</h3>
              <p>Describe brevemente la pieza.</p>
              <div class="actions">
                <a class="btn btn-primary" data-product="Colección Aura – Pieza 01" href="#">Consultar por WhatsApp</a>
              </div>
            </div>
          </article>
          <article class="card">
            <img class="card-img" src="aura-2.jpg" alt="Colección Aura" />
            <div class="card-body">
              <h3>Pieza Aura 02</h3>
              <p>Describe brevemente la pieza.</p>
              <div class="actions">
                <a class="btn btn-primary" data-product="Colección Aura – Pieza 02" href="#">Consultar por WhatsApp</a>
              </div>
            </div>
          </article>
        </div>
        <p style="margin-top:10px;color:var(--muted);font-size:14px">Puedes duplicar estas tarjetas para añadir más piezas.</p>
      </div>
    </section>

    <!-- CATÁLOGO GENERAL -->
    <section id="catalogo" class="section">
      <div class="container">
        <h2>Catálogo</h2>
        <p class="subtitle" style="margin-top:-2px">Sube aquí tus fotos de productos. Solo reemplaza las imágenes y los textos.</p>
        <div class="grid grid-3" id="catalogoGrid">
          <article class="card">
            <img class="card-img" src="producto-1.jpg" alt="Nombre del producto" />
            <div class="card-body">
              <h3>Nombre del producto</h3>
              <p>Descripción corta.</p>
              <div class="actions">
                <a class="btn btn-outline" data-product="Producto 1" href="#">Preguntar por WhatsApp</a>
              </div>
            </div>
          </article>
          <article class="card">
            <img class="card-img" src="producto-2.jpg" alt="Nombre del producto" />
            <div class="card-body">
              <h3>Nombre del producto</h3>
              <p>Descripción corta.</p>
              <div class="actions">
                <a class="btn btn-outline" data-product="Producto 2" href="#">Preguntar por WhatsApp</a>
              </div>
            </div>
          </article>
          <article class="card">
            <img class="card-img" src="producto-3.jpg" alt="Nombre del producto" />
            <div class="card-body">
              <h3>Nombre del producto</h3>
              <p>Descripción corta.</p>
              <div class="actions">
                <a class="btn btn-outline" data-product="Producto 3" href="#">Preguntar por WhatsApp</a>
              </div>
            </div>
          </article>
        </div>
      </div>
    </section>

    <!-- ABOUT -->
    <section class="section" style="background:white">
      <div class="container about">
        <div>
          <h2>Nuestra esencia</h2>
          <p class="subtitle">Rayos de Luna nace para celebrar la feminidad y el brillo interior. Trabajamos con materiales hipoalergénicos y acabados de alta calidad para acompañarte todos los días.</p>
          <ul style="margin:0;padding-left:18px;color:var(--muted)">
            <li>Combos exclusivos y colección Aura</li>
            <li>Empaques listos para regalo</li>
            <li>Atención por WhatsApp y envío a todo Ecuador</li>
          </ul>
        </div>
        <div class="hero-card">
          <img src="about.jpg" alt="Rayos de Luna – Taller" />
        </div>
      </div>
    </section>
  </main>
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

<div class="rayito">
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


  

