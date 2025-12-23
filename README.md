<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>JDStyle — Press Kit / Promo</title>
  <meta name="description" content="One-page imprimible para promocionar la música de JDStyle." />
  <style>
    :root{
      --bg:#0b0f1a;
      --card:#0f1629;
      --ink:#eaf0ff;
      --muted:#a9b6d6;
      --line:rgba(255,255,255,.12);
      --accent:#7c5cff;
      --accent2:#19d3ff;
      --good:#2ee59d;
      --shadow: 0 18px 60px rgba(0,0,0,.45);
      --radius: 18px;
    }

    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji";
      color:var(--ink);
      background:
        radial-gradient(1200px 600px at 15% 10%, rgba(124,92,255,.22), transparent 55%),
        radial-gradient(900px 600px at 85% 25%, rgba(25,211,255,.18), transparent 55%),
        radial-gradient(900px 700px at 55% 95%, rgba(46,229,157,.12), transparent 55%),
        var(--bg);
      line-height:1.4;
    }

    /* Layout */
    .page{
      max-width: 1080px;
      margin: 0 auto;
      padding: 28px 18px 60px;
    }

    .topbar{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
      margin-bottom:22px;
    }

    .brand{
      display:flex;
      align-items:center;
      gap:14px;
      min-width: 240px;
    }

    .logo{
      width:44px;height:44px;border-radius:14px;
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      box-shadow: 0 10px 24px rgba(124,92,255,.25);
      position:relative;
      overflow:hidden;
    }
    .logo:after{
      content:"";
      position:absolute; inset:-30% -30% auto auto;
      width:80px;height:80px;
      background: rgba(255,255,255,.18);
      transform: rotate(25deg);
      filter: blur(0px);
    }

    .brand h1{
      font-size: 18px;
      margin:0;
      letter-spacing:.3px;
    }
    .brand p{margin:2px 0 0;color:var(--muted);font-size:12.5px}

    .actions{
      display:flex;
      gap:10px;
      flex-wrap:wrap;
      justify-content:flex-end;
    }

    .btn{
      appearance:none;
      border:1px solid var(--line);
      background: rgba(255,255,255,.05);
      color: var(--ink);
      padding: 10px 12px;
      border-radius: 999px;
      text-decoration:none;
      font-size: 12.5px;
      display:inline-flex;
      align-items:center;
      gap:8px;
      cursor:pointer;
      transition: transform .12s ease, background .12s ease, border-color .12s ease;
    }
    .btn:hover{transform: translateY(-1px);background: rgba(255,255,255,.08);border-color: rgba(255,255,255,.20)}
    .btn.primary{
      border-color: transparent;
      background: linear-gradient(135deg, rgba(124,92,255,.95), rgba(25,211,255,.85));
      color:#071022;
      font-weight: 650;
    }

    /* Hero */
    .hero{
      display:grid;
      grid-template-columns: 1.25fr .75fr;
      gap:18px;
      align-items:stretch;
    }

    .card{
      background: linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.03));
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      overflow:hidden;
    }

    .hero-main{padding:22px}

    .eyebrow{
      display:inline-flex;
      align-items:center;
      gap:10px;
      padding: 6px 10px;
      border: 1px solid rgba(255,255,255,.14);
      border-radius: 999px;
      background: rgba(255,255,255,.04);
      color: var(--muted);
      font-size: 12px;
      margin-bottom:14px;
    }
    .dot{
      width:8px;height:8px;border-radius:99px;
      background: var(--good);
      box-shadow: 0 0 0 6px rgba(46,229,157,.10);
    }

    .title{
      font-size: 40px;
      line-height:1.05;
      margin: 0 0 10px;
      letter-spacing: -0.7px;
    }
    .subtitle{color:var(--muted);margin:0 0 18px;font-size:15px;max-width: 68ch}

    .badges{display:flex;flex-wrap:wrap;gap:10px;margin: 12px 0 18px}
    .badge{
      font-size:12px;
      color: var(--ink);
      border:1px solid rgba(255,255,255,.14);
      background: rgba(255,255,255,.04);
      padding: 7px 10px;
      border-radius: 999px;
    }

    .grid2{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:14px;
      margin-top: 14px;
    }

    .mini{
      padding:14px;
      border-radius: 16px;
      border: 1px solid rgba(255,255,255,.12);
      background: rgba(11,15,26,.40);
    }
    .mini h3{margin:0 0 8px;font-size: 13.5px;letter-spacing:.2px}
    .mini p{margin:0;color:var(--muted);font-size:12.5px}

    .hero-side{display:flex;flex-direction:column}

    .photo{
      height: 100%;
      min-height: 260px;
      display:flex;
      align-items:flex-end;
      justify-content:space-between;
      padding: 16px;
      position:relative;
      background:
        radial-gradient(700px 420px at 10% 10%, rgba(124,92,255,.35), transparent 60%),
        radial-gradient(700px 420px at 90% 40%, rgba(25,211,255,.25), transparent 60%),
        linear-gradient(180deg, rgba(15,22,41,.55), rgba(15,22,41,.90));
    }

    .avatar{
      width: 92px;height: 92px;
      border-radius: 22px;
      border: 1px solid rgba(255,255,255,.18);
      background: rgba(255,255,255,.06);
      display:grid;
      place-items:center;
      font-weight: 800;
      letter-spacing:.6px;
      color: rgba(234,240,255,.9);
    }

    .photo .meta{
      text-align:right;
      max-width: 55%;
    }
    .photo .meta .name{font-weight:800;font-size: 15px;margin:0}
    .photo .meta .tag{color:var(--muted);font-size: 12.5px;margin:4px 0 0}

    /* Content sections */
    .sections{
      margin-top: 18px;
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap: 18px;
    }

    .section{padding:18px}
    .section h2{margin:0 0 10px;font-size: 15px;letter-spacing:.3px}
    .section p{margin:0;color:var(--muted);font-size: 13px}

    .list{
      margin: 12px 0 0;
      padding: 0;
      list-style:none;
      display:flex;
      flex-direction:column;
      gap:10px;
    }
    .list li{
      display:flex;
      align-items:flex-start;
      justify-content:space-between;
      gap:10px;
      padding: 10px 12px;
      border: 1px solid rgba(255,255,255,.12);
      border-radius: 14px;
      background: rgba(11,15,26,.35);
    }
    .list strong{font-size:13px}
    .list span{color:var(--muted);font-size:12.5px; text-align:right}

    .links{
      display:grid;
      grid-template-columns: 1fr;
      gap:10px;
      margin-top: 12px;
    }

    .linkrow{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:10px;
      padding: 10px 12px;
      border-radius: 14px;
      border: 1px solid rgba(255,255,255,.12);
      background: rgba(11,15,26,.35);
    }

    .linkrow a{
      color: var(--ink);
      text-decoration:none;
      font-size: 13px;
      overflow:hidden;
      text-overflow:ellipsis;
      white-space:nowrap;
      max-width: 70%;
    }
    .pill{
      font-size: 11.5px;
      color:#08101e;
      background: linear-gradient(135deg, rgba(46,229,157,.95), rgba(25,211,255,.75));
      padding: 6px 9px;
      border-radius: 999px;
      font-weight: 700;
      white-space:nowrap;
    }

    .footer{
      margin-top: 18px;
      padding: 16px 18px;
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:12px;
      flex-wrap:wrap;
      color: var(--muted);
      font-size: 12.5px;
    }

    .qr{
      display:flex;
      align-items:center;
      gap:12px;
    }
    .qrcard{
      width: 86px;height: 86px;
      border-radius: 16px;
      border: 1px dashed rgba(255,255,255,.25);
      background: rgba(255,255,255,.04);
      display:grid;
      place-items:center;
      color: rgba(234,240,255,.75);
      font-weight: 800;
      letter-spacing:.3px;
      text-align:center;
      font-size: 10.5px;
      padding: 10px;
    }

    /* Responsive */
    @media (max-width: 920px){
      .hero{grid-template-columns: 1fr}
      .sections{grid-template-columns: 1fr}
      .title{font-size: 34px}
      .photo{min-height: 220px}
    }

    /* Print styles */
    @page { margin: 12mm; }
    @media print{
      body{background: #fff; color:#111;}
      .page{padding:0; max-width:none;}
      .btn, .actions{display:none !important;}
      .card{box-shadow:none; border-color:#ddd; background:#fff;}
      .logo{box-shadow:none;}
      .photo{background:#f7f7f7;}
      .avatar{border-color:#ddd; background:#fff; color:#111;}
      .eyebrow{border-color:#ddd; background:#fff; color:#444;}
      .dot{box-shadow:none;}
      .subtitle, .brand p, .mini p, .section p, .list span, .footer{color:#333 !important;}
      .badge, .mini, .list li, .linkrow{border-color:#ddd; background:#fff;}
      .pill{background:#111; color:#fff;}
      a{color:#111; text-decoration:none;}
      .qrcard{border-color:#bbb;}
    }
  </style>
</head>
<body>
  <div class="page">
    <header class="topbar">
      <div class="brand">
        <div class="logo" aria-hidden="true"></div>
        <div>
          <h1>JDStyle</h1>
          <p>Press Kit / Promo — página moderna e imprimible</p>
        </div>
      </div>

      <div class="actions" aria-label="Acciones">
        <a class="btn" href="#links" title="Ir a enlaces">🔗 Enlaces</a>
        <a class="btn" href="#contact" title="Ir a contacto">✉️ Contacto</a>
        <button class="btn primary" onclick="window.print()" title="Imprimir o guardar como PDF">🖨️ Imprimir / Guardar PDF</button>
      </div>
    </header>

    <section class="hero">
      <div class="card hero-main">
        <div class="eyebrow"><span class="dot"></span>Disponible para shows • colaboraciones • bookings</div>
        <h2 class="title">Tu música, con presencia <span style="background:linear-gradient(135deg,var(--accent),var(--accent2)); -webkit-background-clip:text; background-clip:text; color:transparent;">PRO</span>.</h2>
        <p class="subtitle">
          Plantilla lista para usar como <b>one‑page</b> de promoción. Ideal para enviar por WhatsApp, pegar en bio o imprimir como flyer.
          Solo cambia los textos entre corchetes.
        </p>

        <div class="badges" aria-label="Géneros">
          <span class="badge">🎧 Reggaetón / Urbano</span>
          <span class="badge">🥁 Dembow</span>
          <span class="badge">🎸 Bachata</span>
          <span class="badge">🕺 Cumbia</span>
          <span class="badge">🔥 Trap</span>
        </div>

        <div class="grid2">
          <div class="mini">
            <h3>Lo que ofrezco</h3>
            <p>[Shows en vivo / DJ set / Producción / Featurings / Spots comerciales]</p>
          </div>
          <div class="mini">
            <h3>Zona</h3>
            <p>[Dallas, TX • USA] (puedes cambiarlo)</p>
          </div>
        </div>
      </div>

      <aside class="card hero-side">
        <div class="photo">
          <div class="avatar">TU
FOTO</div>
          <div class="meta">
            <p class="name">JDStyle</p>
            <p class="tag">"JDStyle on the beat" • Artista / Productor</p>
          </div>
        </div>
      </aside>
    </section>

    <section class="sections">
      <div class="card section">
        <h2>Bio (corta)</h2>
        <p>
          [Escribe una bio de 2–4 líneas. Ejemplo: Artista y productor con sonido urbano latino,
          letras directas y melodías románticas. Música hecha en home studio con energía de calle y corazón.] 
        </p>

        <ul class="list" aria-label="Highlights">
          <li><strong>🎶 Último lanzamiento</strong><span>[Nombre del tema] • [Año]</span></li>
          <li><strong>📈 Meta / Logro</strong><span>[Ej: +100k streams / playlist / radio]</span></li>
          <li><strong>🎛️ Sonido</strong><span>[Oscuro / romántico / bailable / moderno]</span></li>
        </ul>
      </div>

      <div class="card section" id="links">
        <h2>Escúchame / Sígueme</h2>
        <p>Reemplaza los enlaces por los tuyos. Consejo: usa un Link-in-bio (Beacons, Linktree, etc.).</p>

        <div class="links" role="list">
          <div class="linkrow" role="listitem">
            <a href="https://open.spotify.com" target="_blank" rel="noreferrer">https://open.spotify.com/artist/[tu-perfil]</a>
            <span class="pill">Spotify</span>
          </div>
          <div class="linkrow" role="listitem">
            <a href="https://music.apple.com" target="_blank" rel="noreferrer">https://music.apple.com/[tu-perfil]</a>
            <span class="pill">Apple Music</span>
          </div>
          <div class="linkrow" role="listitem">
            <a href="https://youtube.com" target="_blank" rel="noreferrer">https://www.youtube.com/@JDStyle-y2g</a>
            <span class="pill">YouTube</span>
          </div>
          <div class="linkrow" role="listitem">
            <a href="https://instagram.com" target="_blank" rel="noreferrer">https://www.instagram.com/jdstyle_05/</a>
            <span class="pill">Instagram</span>
          </div>
          <div class="linkrow" role="listitem">
            <a href="https://tiktok.com" target="_blank" rel="noreferrer">https://www.tiktok.com/@jdstyle_5?lang=es</a>
            <span class="pill">TikTok</span>
          </div>
        </div>
      </div>

      <div class="card section">
        <h2>Servicios</h2>
        <p>Selecciona los que aplican y ajusta precios si quieres (para impresión se ve elegante).</p>
        <ul class="list">
          <li><strong>🎤 Booking (shows)</strong><span>[Desde $___ / evento]</span></li>
          <li><strong>🎧 DJ Set</strong><span>[Desde $___ / hora]</span></li>
          <li><strong>🎚️ Producción (beats)</strong><span>[Exclusivo / Lease]</span></li>
          <li><strong>🤝 Featurings</strong><span>[Condiciones / % splits]</span></li>
        </ul>
      </div>

      <div class="card section" id="contact">
        <h2>Contacto</h2>
        <p>Deja 2–3 opciones máximo para que sea rápido.</p>
        <ul class="list">
          <li><strong>📱 WhatsApp</strong><span>[+1 (___) ___‑____]</span></li>
          <li><strong>✉️ Email</strong><span>jdstyle32@gmail.com</span></li>
          <li><strong>🌐 Link</strong><span>[tu link-in-bio]</span></li>
        </ul>

        <div class="qr" style="margin-top:12px">
          <div class="qrcard">Pega aquí
QR
(impresión)</div>
          <div>
            <p style="margin:0 0 6px; font-weight:750; font-size:13px">Tip rápido</p>
            <p style="margin:0; color:var(--muted); font-size:12.5px">
              Genera un QR con tu link-in-bio y reemplaza este cuadro por una imagen. (En impresión queda pro.)
            </p>
          </div>
        </div>
      </div>
    </section>

    <div class="card footer">
      <div>
        <b>JDStyle</b> • Press Kit • <span style="color:var(--muted)">Actualiza: [mes/año]</span>
      </div>
      <div style="display:flex; gap:10px; flex-wrap:wrap">
        <span style="padding:6px 10px; border:1px solid rgba(255,255,255,.12); border-radius:999px; background:rgba(11,15,26,.35)">#Urbano</span>
        <span style="padding:6px 10px; border:1px solid rgba(255,255,255,.12); border-radius:999px; background:rgba(11,15,26,.35)">#Latino</span>
        <span style="padding:6px 10px; border:1px solid rgba(255,255,255,.12); border-radius:999px; background:rgba(11,15,26,.35)">#Producer</span>
      </div>
    </div>
  </div>

  <script>
    // Opcional: reemplaza "TU FOTO" pegando una imagen.
    // 1) Sustituye el div .avatar por <img class="avatarImg" src="tu-foto.jpg" alt="Foto de JDStyle" />
    // 2) Agrega este CSS:
    // .avatarImg{width:92px;height:92px;border-radius:22px;object-fit:cover;border:1px solid rgba(255,255,255,.18)}
  </script>
</body>
</html>
