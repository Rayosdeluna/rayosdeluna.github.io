
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Rayos de Luna | Bisutería</title>
  <meta name="description" content="Rayos de Luna – Diseñamos joyas con cuidado y amor." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="<a href="https://ibb.co/vC6yGSm3"><img src="https://i.ibb.co/vC6yGSm3/logo-Rayos-de-luna.png" alt="logo-Rayos-de-luna" border="0"></a>" rel="stylesheet">
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

  <footer>
    <div class="container" style="display:flex;justify-content:space-between;gap:10px;flex-wrap:wrap">
      <span>© <span id="year"></span> Rayos de Luna</span>
      <a id="btnFooterWA" href="#">Escríbenos por WhatsApp</a>
    </div>
  </footer>

  <!-- Botón flotante WhatsApp -->
  <a id="btnFloatWA" class="wa-float" href="#" aria-label="">
    <svg viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M19.11 17.51c-.29-.14-1.69-.83-1.95-.93-.26-.1-.45-.14-.64.14-.19.29-.74.93-.9 1.12-.17.19-.33.22-.62.08-.29-.14-1.21-.45-2.3-1.43-.85-.76-1.42-1.69-1.59-1.98-.17-.29-.02-.45.13-.59.13-.13.29-.33.43-.5.14-.17.19-.29.29-.48.1-.19.05-.36-.02-.5-.07-.14-.64-1.55-.88-2.12-.23-.56-.47-.48-.64-.49l-.55-.01c-.19 0-.5.07-.76.36-.26.29-1 1-1 2.43s1.02 2.82 1.17 3.02c.14.19 2 3.05 4.84 4.28.68.29 1.21.46 1.62.59.68.22 1.31.19 1.8.12.55-.08 1.69-.69 1.93-1.36.24-.67.24-1.25.17-1.36-.07-.11-.26-.18-.55-.32zM16.03 4C9.93 4 5 8.93 5 15.02c0 2.28.62 4.39 1.7 6.2L5 28l6.95-1.82c1.73.95 3.72 1.48 5.84 1.48 6.1 0 11.03-4.93 11.03-11.02C28.83 8.93 22.12 4 16.03 4z"/></svg>
    WhatsApp
  </a>

  <!-- Asistente virtual Rayito interactivo -->
  <div id="rayito" style="position:fixed;bottom:90px;right:16px;width:300px;max-width:90%;background:white;border-radius:18px;box-shadow:0 8px 30px rgba(0,0,0,.15);overflow:hidden;font-family:Poppins,system-ui;-webkit-font-smoothing:antialiased;display:none;z-index:70;">
    <div style="background:var(--pink);color:white;padding:12px 16px;font-weight:600;display:flex;justify-content:space-between;align-items:center;">
      <span>Rayito ✨</span>
      <button id="closeRayito" style="background:transparent;border:none;color:white;font-size:18px;cursor:pointer;">×</button>
    </div>
    <div style="padding:12px;font-size:14px;color:var(--ink);">
      <p>¡Hola! Soy Rayito, tu asistente virtual. 😊</p>
      <p>Selecciona una opción para que te muestre información rápida y te conecte por WhatsApp:</p>
      <div style="display:flex;flex-direction:column;gap:8px;margin-top:8px;">
        <button class="rayito-option" data-msg="Quiero información sobre los *Combos* de Rayos de Luna.">Combos</button>
        <button class="rayito-option" data-msg="Quiero información sobre la *Colección Aura* de Rayos de Luna.">Colección Aura</
                                                                                         
                                                                                              
