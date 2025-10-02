<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>ClimaPro | Instalación, Reparación y Mantención de Aire Acondicionado</title>
  <meta name="description" content="Servicio profesional de instalación, reparación y mantención de aire acondicionado. Atención rápida, garantía y presupuesto en el día." />
  <meta name="theme-color" content="#0a66c2">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #0a66c2; /* azul confianza */
      --primary-600: #0959a8;
      --bg: #f7f9fc; /* gris muy claro */
      --text: #0f172a; /* gris-azul oscuro */
      --muted: #64748b; /* gris medio */
      --white: #ffffff;
      --ok: #16a34a;
      --warn: #d97706;
      --danger: #dc2626;
      --radius: 16px;
      --shadow: 0 10px 25px rgba(2, 6, 23, 0.08);
    }
    * { box-sizing: border-box; }
    html, body { margin: 0; padding: 0; font-family: 'Inter', system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif; color: var(--text); background: var(--bg); }
    a { color: var(--primary); text-decoration: none; }
    img { max-width: 100%; height: auto; }
    .container { width: 100%; max-width: 1100px; margin: 0 auto; padding: 0 20px; }

    /* Header */
    header { position: sticky; top: 0; z-index: 50; background: rgba(255,255,255,0.8); backdrop-filter: blur(10px); border-bottom: 1px solid #e2e8f0; }
    .nav { display: flex; align-items: center; justify-content: space-between; padding: 14px 0; }
    .brand { display: flex; align-items: center; gap: 10px; font-weight: 800; letter-spacing: 0.4px; }
    .brand .logo { width: 36px; height: 36px; border-radius: 10px; background: linear-gradient(135deg, var(--primary), #60a5fa); display: grid; place-items: center; color: white; font-weight: 900; box-shadow: var(--shadow); }
    .nav a { font-weight: 500; }
    .menu { display: flex; align-items: center; gap: 18px; }
    .cta { background: var(--primary); color: var(--white); padding: 10px 16px; border-radius: calc(var(--radius) - 8px); display: inline-flex; align-items: center; gap: 8px; font-weight: 600; box-shadow: var(--shadow); border: 1px solid rgba(255,255,255,0.5); }
    .cta:hover { background: var(--primary-600); }
    .hamb { display:none; }

    /* Hero */
    .hero { padding: 64px 0 32px; }
    .hero .wrap { display: grid; grid-template-columns: 1.2fr 1fr; gap: 32px; align-items: center; }
    .badge { display:inline-block; background: #e6f2ff; color: var(--primary); padding: 6px 10px; border-radius: 999px; font-size: 12px; font-weight: 700; letter-spacing: .3px; }
    h1 { font-size: clamp(28px, 4.5vw, 46px); line-height: 1.08; margin: 12px 0 8px; }
    .lead { color: var(--muted); font-size: clamp(15px, 2.5vw, 18px); }
    .hero-cta { display: flex; gap: 12px; margin-top: 18px; flex-wrap: wrap; }
    .ghost { border: 1px solid #cbd5e1; padding: 10px 16px; border-radius: calc(var(--radius) - 8px); font-weight: 600; background: white; }
    .ghost:hover { border-color: var(--primary); color: var(--primary); }
    .hero-card { background: white; border: 1px solid #e2e8f0; border-radius: var(--radius); padding: 18px; box-shadow: var(--shadow); display: grid; gap: 10px; }
    .hero-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 12px; }
    .hero-item { background: #f8fafc; padding: 14px; border-radius: 12px; border: 1px solid #e2e8f0; display:flex; gap:10px; align-items:center; }

    /* Services */
    section { padding: 56px 0; }
    h2 { font-size: clamp(22px, 3.6vw, 32px); margin: 0 0 16px; }
    .subtitle { color: var(--muted); margin-bottom: 24px; }
    .grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 18px; }
    .card { background: white; border: 1px solid #e2e8f0; border-radius: var(--radius); padding: 20px; box-shadow: var(--shadow); }
    .card h3 { margin-top: 8px; margin-bottom: 8px; }
    .check { color: var(--ok); font-weight: 700; margin-right: 6px; }

    /* About */
    .about { display: grid; grid-template-columns: 1fr 1fr; gap: 28px; align-items: center; }

    /* CTA strip */
    .strip { background: linear-gradient(135deg, var(--primary), #60a5fa); color: white; border-radius: var(--radius); padding: 24px; display: grid; grid-template-columns: 1fr auto; gap: 12px; align-items: center; box-shadow: var(--shadow); }
    .strip .cta { background: white; color: var(--primary); border-color: rgba(0,0,0,0.05); }

    /* Contact */
    form { display: grid; gap: 12px; }
    input, textarea, select { width: 100%; padding: 12px 14px; border: 1px solid #cbd5e1; border-radius: 12px; font: inherit; background: #fff; }
    textarea { min-height: 110px; resize: vertical; }
    .two { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }

    /* Footer */
    footer { margin-top: 40px; padding: 24px 0 48px; color: #475569; }
    .foot-grid { display: grid; grid-template-columns: 1.2fr 1fr 1fr; gap: 20px; }
    .mini { font-size: 13px; color: #64748b; }

    /* Responsive */
    @media (max-width: 960px) {
      .hero .wrap { grid-template-columns: 1fr; }
      .grid { grid-template-columns: 1fr; }
      .about { grid-template-columns: 1fr; }
      .strip { grid-template-columns: 1fr; }
      .two { grid-template-columns: 1fr; }
      .menu { display:none; }
      .hamb { display:inline-flex; background: white; border: 1px solid #e2e8f0; padding: 8px 12px; border-radius: 12px; }
      .mobile-menu { display:none; position: absolute; top: 62px; left: 0; right: 0; background: white; border-bottom: 1px solid #e2e8f0; box-shadow: var(--shadow); }
      .mobile-menu a { display:block; padding: 14px 20px; border-top: 1px solid #f1f5f9; }
    }
  </style>
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "LocalBusiness",
    "name": "ClimaPro",
    "image": "",
    "url": "",
    "telephone": "+56 9 1234 5678",
    "address": {
      "@type": "PostalAddress",
      "addressLocality": "Santiago",
      "addressCountry": "CL"
    },
    "areaServed": "Región Metropolitana",
    "priceRange": "$$",
    "servesCuisine": "",
    "description": "Instalación, reparación y mantención de aire acondicionado con atención rápida y garantía."
  }
  </script>
</head>
<body>
  <!-- Header -->
  <header>
    <div class="container nav">
      <div class="brand">
        <div class="logo">❄️</div>
        <span>ClimaPro</span>
      </div>
      <nav class="menu">
        <a href="#servicios">Servicios</a>
        <a href="#nosotros">Nosotros</a>
        <a href="#contacto">Contacto</a>
        <a class="cta" href="https://wa.me/56911111111?text=Hola%20ClimaPro%2C%20necesito%20un%20presupuesto" target="_blank" rel="noopener">WhatsApp</a>
      </nav>
      <button class="hamb" id="hamb">Menú</button>
    </div>
    <div class="mobile-menu" id="mobileMenu">
      <a href="#servicios">Servicios</a>
      <a href="#nosotros">Nosotros</a>
      <a href="#contacto">Contacto</a>
      <a href="https://wa.me/56911111111?text=Hola%20ClimaPro%2C%20necesito%20un%20presupuesto" target="_blank" rel="noopener">WhatsApp</a>
    </div>
  </header>

  <!-- Hero -->
  <section class="hero">
    <div class="container wrap">
      <div>
        <span class="badge">Instalación • Reparación • Mantención</span>
        <h1>Clima perfecto todo el año, <br/>servicio técnico de confianza</h1>
        <p class="lead">Atención en el día, técnicos certificados y garantía por escrito. Cotiza la instalación, reparación o mantención de tu aire acondicionado split, multisplit o central.</p>
        <div class="hero-cta">
          <a class="cta" href="#contacto">Solicitar presupuesto</a>
          <a class="ghost" href="#servicios">Ver servicios</a>
        </div>
        <div class="hero-grid" style="margin-top:16px;">
          <div class="hero-item">✅ Garantía 6–12 meses</div>
          <div class="hero-item">⚡ Respuesta rápida</div>
          <div class="hero-item">🧰 Técnicos certificados</div>
          <div class="hero-item">📍 Cobertura RM</div>
        </div>
      </div>
      <div class="hero-card">
        <strong>Agenda una visita técnica</strong>
        <form id="quickForm" onsubmit="return sendWhatsApp(this)">
          <div class="two">
            <input name="nombre" placeholder="Tu nombre" required>
            <input name="telefono" placeholder="Teléfono" required>
          </div>
          <select name="servicio" required>
            <option value="Instalación">Instalación</option>
            <option value="Reparación">Reparación</option>
            <option value="Mantención">Mantención</option>
          </select>
          <input name="comuna" placeholder="Comuna" required>
          <textarea name="detalle" placeholder="Cuéntanos brevemente el equipo o problema"></textarea>
          <button class="cta" type="submit">Enviar por WhatsApp</button>
        </form>
        <span class="mini">Respuesta entre 9:00–19:00 hrs.</span>
      </div>
    </div>
  </section>

  <!-- Servicios -->
  <section id="servicios">
    <div class="container">
      <h2>Nuestros servicios</h2>
      <p class="subtitle">Soluciones integrales en climatización para hogares, oficinas y comercios.</p>
      <div class="grid">
        <article class="card">
          <div>🧩</div>
          <h3>Instalación</h3>
          <p>Instalación de equipos Split, Multi Split, Cassette y VRF. Evaluación de carga térmica y selección del equipo adecuado.</p>
          <ul>
            <li><span class="check">✓</span> Visita técnica y cotización</li>
            <li><span class="check">✓</span> Tuberías, drenajes y fijaciones</li>
            <li><span class="check">✓</span> Puesta en marcha y capacitación</li>
          </ul>
        </article>
        <article class="card">
          <div>🛠️</div>
          <h3>Reparación</h3>
          <p>Diagnóstico y reparación de fallas eléctricas, de refrigeración y control. Repuestos originales y garantía.</p>
          <ul>
            <li><span class="check">✓</span> Diagnóstico en 24–48h</li>
            <li><span class="check">✓</span> Carga de gas refrigerante</li>
            <li><span class="check">✓</span> Cambio de tarjetas y sensores</li>
          </ul>
        </article>
        <article class="card">
          <div>🧼</div>
          <h3>Mantención</h3>
          <p>Mantenciones preventivas y correctivas para extender la vida útil y mejorar eficiencia energética.</p>
          <ul>
            <li><span class="check">✓</span> Limpieza profunda de unidades</li>
            <li><span class="check">✓</span> Revisión eléctrica y de drenes</li>
            <li><span class="check">✓</span> Planes trimestrales y semestrales</li>
          </ul>
        </article>
      </div>
    </div>
  </section>

  <!-- Nosotros -->
  <section id="nosotros">
    <div class="container about">
      <div>
        <h2>Experiencia, rapidez y garantía</h2>
        <p class="subtitle">Somos un equipo técnico con más de 8 años en climatización residencial y comercial. Trabajamos con marcas líderes y estándares de seguridad.</p>
        <ul class="mini">
          <li>• Técnicos certificados SEC / manipulador de gases</li>
          <li>• Garantía por escrito en cada servicio</li>
          <li>• Facturación y contrato de mantenciones para empresas</li>
        </ul>
      </div>
      <div class="card">
        <strong>¿Por qué elegirnos?</strong>
        <ul>
          <li><span class="check">✓</span> Atención el mismo día (según disponibilidad)</li>
          <li><span class="check">✓</span> Soporte post‑servicio por WhatsApp</li>
          <li><span class="check">✓</span> Cobertura en toda la RM</li>
          <li><span class="check">✓</span> Transparencia de precios</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- Tira CTA -->
  <section>
    <div class="container">
      <div class="strip">
        <div>
          <h3 style="margin:0 0 6px">¿Necesitas una visita técnica?</h3>
          <p style="margin:0; opacity:.95">Agenda hoy mismo y recibe tu presupuesto en el día.</p>
        </div>
        <a class="cta" href="https://wa.me/56911111111?text=Hola%20ClimaPro%2C%20quisiera%20agendar%20una%20visita%20t%C3%A9cnica" target="_blank" rel="noopener">Escribir por WhatsApp</a>
      </div>
    </div>
  </section>

  <!-- Contacto -->
  <section id="contacto">
    <div class="container">
      <h2>Contacto</h2>
      <p class="subtitle">Cuéntanos qué necesitas y te responderemos a la brevedad.</p>
      <div class="grid" style="grid-template-columns: 1fr 1fr;">
        <div class="card">
          <form id="contactForm" onsubmit="return sendWhatsApp(this)">
            <div class="two">
              <input name="nombre" placeholder="Nombre" required>
              <input name="telefono" placeholder="Teléfono" required>
            </div>
            <input name="email" type="email" placeholder="Email (opcional)">
            <select name="servicio" required>
              <option value="Instalación">Instalación</option>
              <option value="Reparación">Reparación</option>
              <option value="Mantención">Mantención</option>
              <option value="Otro">Otro</option>
            </select>
            <textarea name="detalle" placeholder="Mensaje"></textarea>
            <button class="cta" type="submit">Enviar por WhatsApp</button>
          </form>
        </div>
        <div>
          <div class="card" style="margin-bottom:12px;">
            <strong>Datos de contacto</strong>
            <p class="mini">Teléfono: <a href="tel:+56911111111">+56 9 1111 1111</a><br>Correo: <a href="mailto:contacto@climapro.cl">contacto@climapro.cl</a><br>Horario: Lun–Sáb 9:00–19:00</p>
          </div>
          <div class="card">
            <strong>Cobertura</strong>
            <p class="mini">Santiago y comunas aledañas. Para regiones, consultar disponibilidad.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container foot-grid">
      <div>
        <div class="brand"><div class="logo">❄️</div><span>ClimaPro</span></div>
        <p class="mini">© <span id="year"></span> ClimaPro. Todos los derechos reservados.</p>
      </div>
      <div>
        <strong>Enlaces</strong>
        <ul class="mini" style="list-style:none; padding:0;">
          <li><a href="#servicios">Servicios</a></li>
          <li><a href="#nosotros">Nosotros</a></li>
          <li><a href="#contacto">Contacto</a></li>
        </ul>
      </div>
      <div>
        <strong>Legal</strong>
        <p class="mini">Términos y condiciones · Política de privacidad</p>
      </div>
    </div>
  </footer>

  <a href="https://wa.me/56911111111?text=Hola%20ClimaPro%2C%20necesito%20un%20presupuesto" target="_blank" rel="noopener" aria-label="WhatsApp" style="position:fixed; right:16px; bottom:16px; background:#25D366; color:white; border-radius:999px; padding:14px 16px; box-shadow: var(--shadow); font-weight:700;">WhatsApp</a>

  <script>
    // Año dinámico
    document.getElementById('year').textContent = new Date().getFullYear();

    // Menú móvil
    const hamb = document.getElementById('hamb');
    const mobile = document.getElementById('mobileMenu');
    if (hamb) hamb.addEventListener('click', () => mobile.style.display = mobile.style.display === 'block' ? 'none' : 'block');

    // Enviar formularios a WhatsApp
    function sendWhatsApp(form) {
      const data = new FormData(form);
      const nombre = data.get('nombre') || '';
      const telefono = data.get('telefono') || '';
      const servicio = data.get('servicio') || '';
      const comuna = data.get('comuna') || '';
      const detalle = data.get('detalle') || '';

      const base = 'https://wa.me/56911111111'; // <-- Reemplaza con tu número en formato internacional sin «+»
      const msg = `Hola, soy ${nombre}.\n` +
                  (telefono ? `Teléfono: ${telefono}\n` : '') +
                  (servicio ? `Servicio: ${servicio}\n` : '') +
                  (comuna ? `Comuna: ${comuna}\n` : '') +
                  (detalle ? `Detalle: ${detalle}` : '');

      const url = `${base}?text=${encodeURIComponent(msg)}`;
      window.open(url, '_blank');
      form.reset();
      return false;
    }
  </script>
</body>
</html>
