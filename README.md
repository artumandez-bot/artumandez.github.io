<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Punto de Información — Ciberseguridad</title>
  <style>
    :root{
      --bg:#0b0f1a; --card:#0f1724; --accent:#00e6a8; --muted:#9aa4b2; --glass: rgba(255,255,255,0.03);
      font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    body{margin:0;background:linear-gradient(180deg,#061022 0%, #071323 100%);color:#e6eef6;min-height:100vh}
    .container{max-width:1100px;margin:32px auto;padding:24px}

    header{display:flex;align-items:center;gap:20px}
    .logo{display:flex;flex-direction:column;gap:4px}
    .title{font-size:48px;line-height:1;font-weight:700;color:var(--accent);text-shadow:0 6px 24px rgba(0,230,168,0.06)}
    .subtitle{color:var(--muted);font-size:14px}

    nav{margin-left:auto;display:flex;gap:12px;align-items:center}
    .btn{background:var(--glass);border:1px solid rgba(255,255,255,0.04);padding:10px 14px;border-radius:12px;color:var(--accent);text-decoration:none;font-weight:600;display:inline-flex;align-items:center;gap:8px}
    .btn--primary{background:linear-gradient(90deg, rgba(0,230,168,0.08), rgba(0,230,168,0.02));border-color:rgba(0,230,168,0.12)}

    main{display:grid;grid-template-columns:1fr 360px;gap:24px;margin-top:26px}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border:1px solid rgba(255,255,255,0.03);padding:18px;border-radius:14px}

    .intro h2{margin:0 0 8px 0}
    .intro p{color:var(--muted);margin:0}

    .resources-list{display:flex;flex-direction:column;gap:12px;margin-top:12px}
    .resource{padding:12px;border-radius:10px;background:rgba(255,255,255,0.01);border:1px solid rgba(255,255,255,0.02)}
    .resource h4{margin:0 0 6px 0}
    .resource p{margin:0;color:var(--muted);font-size:14px}
    .resource .meta{margin-top:8px;font-size:13px;color:#bdebd6}

    aside .contact-title{font-size:18px;margin-bottom:8px}
    label{display:block;font-size:13px;color:var(--muted);margin-bottom:6px}
    input,textarea{width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit}
    textarea{min-height:110px;resize:vertical}
    .form-actions{display:flex;gap:10px;margin-top:10px}
    .muted{color:var(--muted);font-size:13px}

    footer{margin-top:28px;color:var(--muted);font-size:13px;text-align:center}

    /* responsive */
    @media (max-width:900px){main{grid-template-columns:1fr;}.title{font-size:36px}.container{padding:16px}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="logo">
        <div class="title">Punto de Información</div>
        <div class="subtitle">Recursos y apoyo en ciberseguridad para estudiantes y docentes</div>
      </div>

      <nav>
        <a class="btn" href="mailto:info@puntodeinformacion.edu?subject=Consulta%20Punto%20de%20Informaci%C3%B3n" aria-label="Enviar correo">📧 Correo</a>
        <a class="btn btn--primary" id="waBtn" href="https://wa.me/573001234567?text=Hola%20tengo%20una%20consulta%20sobre%20Punto%20de%20Informaci%C3%B3n" target="_blank" rel="noopener">🟢 WhatsApp</a>
      </nav>
    </header>

    <main>
      <section class="card intro">
        <h2>Bienvenido</h2>
        <p>Este portal está pensado como un punto de apoyo para aprender conceptos básicos de ciberseguridad, detectar riesgos y acceder a recursos didácticos.</p>

        <div style="margin-top:18px">
          <h3>¿Qué encontrarás?</h3>
          <ul style="color:var(--muted);margin-top:8px">
            <li>Guías prácticas para proteger cuentas y dispositivos.</li>
            <li>Actividades y simuladores para reconocer intentos de phishing.</li>
            <li>Contacto directo con el docente o el equipo de soporte.</li>
          </ul>
        </div>

        <div style="margin-top:18px">
          <h3>Recursos</h3>
          <div class="resources-list" id="resources">
            <!-- Recursos inventados -->
            <article class="resource">
              <h4>Guía rápida: Contraseñas seguras</h4>
              <p>Resumen paso a paso para crear y gestionar contraseñas robustas con ejemplos y prácticas recomendadas.</p>
              <div class="meta">Formato: PDF · Duración lectura: 6 minutos · Nivel: Inicial</div>
            </article>

            <article class="resource">
              <h4>Checklist: Seguridad básica en dispositivos</h4>
              <p>Lista práctica para revisar configuración de privacidad, actualizaciones y copias de seguridad.</p>
              <div class="meta">Formato: Checklist interactivo · Nivel: Todos</div>
            </article>

            <article class="resource">
              <h4>Mini-curso: Fundamentos de Ciberseguridad</h4>
              <p>Módulos cortos con ejercicios para entender amenazas comunes y buenas prácticas.</p>
              <div class="meta">Formato: Módulos en video + PDF · 3 lecciones · Nivel: Básico</div>
            </article>

            <article class="resource">
              <h4>Simulador de phishing (demo)</h4>
              <p>Pequeña experiencia interactiva para identificar correos y mensajes sospechosos.</p>
              <div class="meta">Demo Web · Tiempo estimado: 10 minutos</div>
            </article>

            <article class="resource">
              <h4>Manual: Privacidad en redes sociales</h4>
              <p>Consejos para configurar privacidad y gestionar la información personal en plataformas sociales.</p>
              <div class="meta">E-book · Nivel: Intermedio</div>
            </article>

          </div>
        </div>

      </section>

      <aside class="card">
        <div class="contact-title">Contacto</div>
        <div class="muted">Escríbenos tu duda o solicita apoyo. También puedes usar el botón de WhatsApp o enviar un correo.</div>

        <form id="contactForm" onsubmit="handleSubmit(event)">
          <label for="name">Nombre</label>
          <input id="name" name="name" placeholder="Tu nombre" required />

          <label for="email">Correo electrónico</label>
          <input id="email" name="email" type="email" placeholder="tu@correo.com" required />

          <label for="message">Mensaje</label>
          <textarea id="message" name="message" placeholder="¿En qué podemos ayudarte?" required></textarea>

          <div class="form-actions">
            <button type="submit" class="btn btn--primary">Enviar mensaje</button>
            <a class="btn" href="mailto:info@puntodeinformacion.edu?subject=Contacto%20desde%20sitio">Enviar por correo</a>
          </div>

          <div id="formStatus" style="margin-top:10px;color:#bdebd6;display:none"></div>
        </form>

        <hr style="margin:12px 0;border:none;border-top:1px solid rgba(255,255,255,0.02)" />

        <div>
          <strong>Atención:</strong>
          <p class="muted" style="margin:6px 0">Horario de soporte: Lunes a Viernes · 8:00 - 17:00</p>
        </div>
      </aside>
    </main>

    <footer>
      © <span id="year"></span> Punto de Información · Diseño: Ciberseguridad educativa
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();

    function handleSubmit(e){
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const message = document.getElementById('message').value.trim();
      if(!name || !email || !message){alert('Por favor completa todos los campos.'); return}

      // En un sitio real aquí haríamos un envío por fetch a un endpoint. En este archivo demo mostraremos un mensaje.
      const status = document.getElementById('formStatus');
      status.style.display = 'block';
      status.textContent = 'Gracias, ' + name + '. Tu mensaje ha sido registrado. Responderemos a: ' + email;

      // Limpiar formulario
      document.getElementById('contactForm').reset();

      // (opcional) abrir correo con contenido prellenado
      // window.location.href = `mailto:info@puntodeinformacion.edu?subject=Consulta%20de%20${encodeURIComponent(name)}&body=${encodeURIComponent(message)}`;
    }
  </script>
</body>
</html>
