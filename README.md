<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
<title>Start-Ip | Preferencias app de subastas | Equipo Start-Ip</title>
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    -webkit-tap-highlight-color: transparent;
  }

  body {
    font-family: 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    background: linear-gradient(145deg, #0a2e1f 0%, #0a1f1a 100%);
    color: #f1f5f9;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 16px;
  }

  .card {
    background: rgba(18, 28, 24, 0.95);
    backdrop-filter: blur(2px);
    border-radius: 1.5rem;
    max-width: 680px;
    width: 100%;
    margin: auto;
    padding: 1.5rem;
    box-shadow: 0 25px 45px -12px rgba(0,0,0,0.6), 0 0 0 1px rgba(80, 200, 120, 0.25);
    border: 1px solid #2a5540;
  }

  h1 {
    color: #6ee7b7;
    font-size: 1.8rem;
    font-weight: 700;
    letter-spacing: -0.3px;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    flex-wrap: wrap;
  }

  h1:before {
    content: "⏱️";
    font-size: 1.6rem;
  }

  .subhead {
    text-align: center;
    border-bottom: 1px dashed #2a6b4a;
    padding-bottom: 1rem;
    margin-bottom: 1.5rem;
  }

  .team-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 8px;
    margin-top: 12px;
    margin-bottom: 8px;
  }

  .team-badge {
    background: #0f2a1e;
    border-radius: 40px;
    padding: 6px 12px;
    font-size: 0.75rem;
    font-weight: 500;
    color: #cbd5e1;
    border-left: 3px solid #6ee7b7;
    display: inline-flex;
    align-items: center;
    gap: 6px;
    flex-wrap: wrap;
  }

  .team-badge strong {
    color: #facc15;
    font-weight: 600;
  }

  .brand {
    font-weight: 700;
    color: #facc15;
    background: #1e3a2f;
    padding: 0.2rem 0.7rem;
    border-radius: 20px;
    display: inline-block;
  }

  .form-group {
    margin-bottom: 1.4rem;
    text-align: left;
  }

  .question {
    font-weight: 600;
    font-size: 1rem;
    margin-bottom: 10px;
    display: flex;
    align-items: baseline;
    gap: 8px;
    flex-wrap: wrap;
    color: #e2e8f0;
  }

  .question .q-num {
    background: #0f2a1e;
    color: #6ee7b7;
    border-radius: 30px;
    width: 26px;
    height: 26px;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    font-size: 0.8rem;
    font-weight: bold;
  }

  textarea, input, select {
    width: 100%;
    padding: 12px 14px;
    background: #0f241d;
    border: 1px solid #2a6b4a;
    border-radius: 20px;
    font-size: 0.95rem;
    color: #f8fafc;
    transition: 0.2s;
    font-family: inherit;
    resize: vertical;
  }

  textarea:focus, input:focus, select:focus {
    outline: none;
    border-color: #6ee7b7;
    box-shadow: 0 0 0 3px #6ee7b740;
  }

  .radio-group {
    display: flex;
    flex-wrap: wrap;
    gap: 0.8rem;
    align-items: center;
    background: #0f241d;
    padding: 0.7rem 0.9rem;
    border-radius: 32px;
    border: 1px solid #2a6b4a;
  }

  .radio-group label {
    display: flex;
    align-items: center;
    gap: 6px;
    font-weight: normal;
    cursor: pointer;
    font-size: 0.85rem;
    flex: 1 0 auto;
    min-width: 110px;
  }

  .radio-group input {
    width: auto;
    transform: scale(1.05);
    accent-color: #6ee7b7;
    margin: 0;
  }

  .inline-hint {
    font-size: 0.7rem;
    color: #9bbdaa;
    margin-top: 5px;
  }

  button {
    background: #0f241d;
    border: 2px solid #6ee7b7;
    color: #6ee7b7;
    padding: 14px 20px;
    font-size: 1rem;
    font-weight: bold;
    border-radius: 60px;
    cursor: pointer;
    transition: 0.2s;
    width: 100%;
    margin-top: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 12px;
    font-family: inherit;
  }

  button:hover {
    background: #6ee7b7;
    color: #0a2e1f;
    box-shadow: 0 8px 20px -8px #6ee7b7aa;
    border-color: #6ee7b7;
  }

  button:active {
    transform: scale(0.98);
  }

  .result-message {
    margin-top: 18px;
    background: #1e3a2f;
    border-radius: 32px;
    padding: 12px;
    font-size: 0.85rem;
    text-align: center;
    border-left: 4px solid #6ee7b7;
    transition: all 0.2s;
  }

  footer {
    font-size: 0.65rem;
    text-align: center;
    margin-top: 24px;
    color: #5e8b76;
  }

  .share-link-container {
    margin-top: 20px;
    padding: 12px;
    background: #0f241d80;
    border-radius: 28px;
    text-align: center;
    border: 1px dashed #6ee7b760;
  }

  .share-link-container p {
    font-size: 0.75rem;
    margin-bottom: 8px;
    color: #cbd5e1;
  }

  .link-copy-area {
    display: flex;
    align-items: center;
    gap: 8px;
    flex-wrap: wrap;
    justify-content: center;
  }

  .fake-link {
    background: #0a1f18;
    padding: 8px 12px;
    border-radius: 40px;
    font-size: 0.7rem;
    color: #a7f3d0;
    font-family: monospace;
    word-break: break-all;
    flex: 1;
    text-align: center;
    border: 1px solid #2a6b4a;
  }

  .copy-btn {
    background: #1e3a2f;
    border: 1px solid #6ee7b7;
    color: #6ee7b7;
    padding: 6px 14px;
    font-size: 0.75rem;
    border-radius: 40px;
    cursor: pointer;
    font-weight: bold;
    white-space: nowrap;
  }

  .copy-btn:active {
    background: #6ee7b7;
    color: #0a2e1f;
  }

  .destino-info {
    background: #1e3a2f;
    border-radius: 30px;
    padding: 8px 15px;
    margin-top: 10px;
    font-size: 0.75rem;
    text-align: center;
    display: inline-block;
    width: auto;
    color: #a7f3d0;
  }

  .destino-info span {
    color: #facc15;
    font-weight: bold;
  }

  @media (max-width: 550px) {
    .card {
      padding: 1.2rem;
    }
    .radio-group {
      flex-direction: column;
      align-items: flex-start;
      border-radius: 24px;
    }
    .radio-group label {
      width: 100%;
    }
    h1 {
      font-size: 1.5rem;
    }
    .team-badge {
      font-size: 0.7rem;
      padding: 4px 10px;
    }
  }
</style>
</head>
<body>

<div class="card">
  <h1>Start-Ip · Subastas</h1>
  <div class="subhead">
    <p>📦 <span class="brand">¿Qué te gustaría en una app de subastas?</span> · 10 preguntas</p>
    
    <!-- EQUIPO START-IP -->
    <div class="team-grid">
      <div class="team-badge">👑 <strong>Franklin Patzi Marce</strong> · Líder · PO/Tester</div>
      <div class="team-badge">📄 <strong>Angelica Burgos</strong> · Documentador</div>
      <div class="team-badge">🎨 <strong>Jhoao Cesar Daza Vargas</strong> · Frontend</div>
      <div class="team-badge">⚙️ <strong>Lucio Daniel Ticona</strong> · Backend</div>
    </div>
    
    <!-- DESTINO FIJO DEL CORREO -->
    <div class="destino-info">
      📧 Las respuestas se enviarán directamente a: <span>franklinys1@gmail.com</span>
    </div>
    <p style="font-size: 0.7rem; margin-top: 8px;">✨ Equipo Start-Ip — Tu opinión construye la mejor experiencia en subastas</p>
  </div>

  <form id="evalForm">
    <!-- 1. Categorías favoritas -->
    <div class="form-group">
      <div class="question"><span class="q-num">1</span> ¿Qué categorías te interesan más?</div>
      <div class="radio-group">
        <label><input type="radio" name="categoria" value="Tecnología y gadgets"> 📱 Tecnología y gadgets</label>
        <label><input type="radio" name="categoria" value="Autos y motos"> 🚗 Autos y motos</label>
        <label><input type="radio" name="categoria" value="Moda y accesorios"> 👕 Moda y accesorios</label>
        <label><input type="radio" name="categoria" value="Coleccionables y arte"> 🎨 Coleccionables/arte</label>
        <label><input type="radio" name="categoria" value="Hogar y electrodomésticos"> 🏠 Hogar</label>
      </div>
    </div>

    <!-- 2. Tipo de subasta preferida -->
    <div class="form-group">
      <div class="question"><span class="q-num">2</span> ¿Qué tipo de subasta prefieres?</div>
      <div class="radio-group">
        <label><input type="radio" name="tipo" value="Subasta tradicional (mayor oferta gana)"> ⏫ Tradicional (mayor oferta)</label>
        <label><input type="radio" name="tipo" value="Subasta inversa (precio baja hasta comprar)"> 🔻 Subasta inversa</label>
        <label><input type="radio" name="tipo" value="Subasta con tiempo límite fijo"> ⏱️ Tiempo límite fijo</label>
        <label><input type="radio" name="tipo" value="Subasta estilo 'puja oculta'"> 🕵️ Puja oculta</label>
      </div>
    </div>

    <!-- 3. Funcionalidad más importante -->
    <div class="form-group">
      <div class="question"><span class="q-num">3</span> ¿Qué funcionalidad valoras más?</div>
      <div class="radio-group">
        <label><input type="radio" name="funcion" value="Notificaciones en tiempo real"> 🔔 Notificaciones en tiempo real</label>
        <label><input type="radio" name="funcion" value="Historial de pujas y transparencia"> 📜 Historial transparente</label>
        <label><input type="radio" name="funcion" value="Chat con vendedores"> 💬 Chat integrado</label>
        <label><input type="radio" name="funcion" value="Pagos seguros y múltiples métodos"> 💳 Pagos seguros</label>
      </div>
    </div>

    <!-- 4. Frecuencia de uso estimada -->
    <div class="form-group">
      <div class="question"><span class="q-num">4</span> ¿Con qué frecuencia usarías la app?</div>
      <div class="radio-group">
        <label><input type="radio" name="frecuencia" value="A diario"> 🔥 A diario</label>
        <label><input type="radio" name="frecuencia" value="Varias veces por semana"> 📅 Varias veces/semana</label>
        <label><input type="radio" name="frecuencia" value="Una vez por semana"> 🗓️ Una vez por semana</label>
        <label><input type="radio" name="frecuencia" value="Solo cuando hay algo específico"> 🎯 Solo algo específico</label>
      </div>
    </div>

    <!-- 5. Monto de puja habitual -->
    <div class="form-group">
      <div class="question"><span class="q-num">5</span> ¿Qué rango de pujas manejas normalmente?</div>
      <div class="radio-group">
        <label><input type="radio" name="monto" value="Menos de $50"> 💰 Menos de $50</label>
        <label><input type="radio" name="monto" value="$50 - $200"> 💵 $50 - $200</label>
        <label><input type="radio" name="monto" value="$200 - $1000"> 🪙 $200 - $1000</label>
        <label><input type="radio" name="monto" value="Más de $1000"> 💎 Más de $1000</label>
      </div>
    </div>

    <!-- 6. ¿Qué te genera desconfianza en subastas online? -->
    <div class="form-group">
      <div class="question"><span class="q-num">6</span> ¿Qué te genera más desconfianza?</div>
      <div class="radio-group">
        <label><input type="radio" name="desconfianza" value="Productos falsificados"> 🧐 Productos falsificados</label>
        <label><input type="radio" name="desconfianza" value="Falta de protección al comprador"> 🛡️ Falta de protección</label>
        <label><input type="radio" name="desconfianza" value="Pujas fraudulentas o bots"> 🤖 Pujas fraudulentas</label>
        <label><input type="radio" name="desconfianza" value="Envíos lentos o dañados"> 📦 Envíos poco fiables</label>
      </div>
    </div>

    <!-- 7. Preferencia de diseño/app -->
    <div class="form-group">
      <div class="question"><span class="q-num">7</span> ¿Qué estilo de app prefieres?</div>
      <div class="radio-group">
        <label><input type="radio" name="diseno" value="Modo oscuro siempre"> 🌙 Modo oscuro</label>
        <label><input type="radio" name="diseno" value="Claro y minimalista"> ☀️ Claro y minimalista</label>
        <label><input type="radio" name="diseno" value="Con animaciones y efectos"> ✨ Animaciones / efectos</label>
        <label><input type="radio" name="diseno" value="Sencillo y rápido (sin distracciones)"> ⚡ Sencillo y rápido</label>
      </div>
    </div>

    <!-- 8. Funcionalidad social -->
    <div class="form-group">
      <div class="question"><span class="q-num">8</span> ¿Te gustaría tener funciones sociales?</div>
      <div class="radio-group">
        <label><input type="radio" name="social" value="Sí, perfiles públicos y valoraciones"> 👍 Sí, perfiles y valoraciones</label>
        <label><input type="radio" name="social" value="Seguir a otros pujadores"> 👥 Seguir pujadores destacados</label>
        <label><input type="radio" name="social" value="Solo lo necesario (cerrar ofertas)"> 🔒 Solo lo necesario</label>
        <label><input type="radio" name="social" value="No me interesa la parte social"> 🚫 Sin redes internas</label>
      </div>
    </div>

    <!-- 9. Método de pago favorito -->
    <div class="form-group">
      <div class="question"><span class="q-num">9</span> ¿Qué método de pago te gustaría integrar?</div>
      <div class="radio-group">
        <label><input type="radio" name="pago" value="Tarjeta débito/crédito"> 💳 Tarjeta</label>
        <label><input type="radio" name="pago" value="Transferencia bancaria"> 🏦 Transferencia</label>
        <label><input type="radio" name="pago" value="Criptomonedas (USDT, BTC)"> ₿ Criptomonedas</label>
        <label><input type="radio" name="pago" value="Billeteras digitales (Mercado Pago, PayPal)"> 📲 Billeteras digitales</label>
      </div>
    </div>

    <!-- 10. Recomendación adicional (texto libre) -->
    <div class="form-group">
      <div class="question"><span class="q-num">10</span> ¿Qué otra funcionalidad te gustaría ver en Start-Ip?</div>
      <textarea name="sugerencia" rows="2" placeholder="Ej: subasta con reembolso garantizado, envíos tracking, recordatorios personalizados..."></textarea>
    </div>

    <!-- Campo opcional: nombre del evaluador -->
    <div class="form-group">
      <div class="question"><span class="q-num">📝</span> Tu nombre o identificador (opcional)</div>
      <input type="text" name="evaluador" placeholder="Ej: Carlos, proveedor, usuario anónimo...">
    </div>

    <button type="button" id="sendPrivateBtn">📨 Enviar respuestas a Franklin (franklinys1@gmail.com)</button>
  </form>

  <!-- Link para compartir formulario estilo Drive -->
  <div class="share-link-container" id="shareLinkBox" style="margin-top: 1rem;">
    <p>🔗 Comparte esta encuesta (link tipo Drive):</p>
    <div class="link-copy-area">
      <span class="fake-link" id="pageUrlDisplay">Cargando enlace...</span>
      <button type="button" class="copy-btn" id="copyLinkBtn">📋 Copiar</button>
    </div>
    <p style="font-size: 0.65rem; margin-top: 8px;">✓ Enlace directo para móvil — compatible con WhatsApp, Telegram, etc.</p>
  </div>

  <div id="statusMsg" class="result-message" style="display: none;"></div>
  <footer>🏷️ Start-Ip · Franklin, Angelica, Jhoao, Lucio · Las respuestas llegan directo al líder del proyecto</footer>
</div>

<script>
  (function() {
    const sendBtn = document.getElementById('sendPrivateBtn');
    const statusDiv = document.getElementById('statusMsg');
    const copyBtn = document.getElementById('copyLinkBtn');
    const urlDisplaySpan = document.getElementById('pageUrlDisplay');

    // DESTINO FIJO
    const DESTINO_CORREO = "franklinys1@gmail.com";

    // Mostrar URL actual
    let currentUrl = window.location.href;
    if (currentUrl === 'about:blank' || currentUrl === '' || currentUrl.indexOf('file://') === 0) {
      if (currentUrl.startsWith('file:')) {
        urlDisplaySpan.innerText = '📁 Sube este archivo HTML a un hosting (o GitHub Pages)';
        urlDisplaySpan.style.color = '#facc15';
      } else {
        urlDisplaySpan.innerText = currentUrl || 'Enlace actual - copia manualmente';
      }
    } else {
      urlDisplaySpan.innerText = currentUrl;
    }

    function copyLinkToClipboard() {
      let urlToCopy = window.location.href;
      if (urlToCopy === 'about:blank' || urlToCopy === '') urlToCopy = document.URL;
      if (urlToCopy.startsWith('file:')) {
        statusDiv.style.display = 'block';
        statusDiv.innerHTML = "⚠️ Este archivo está en local. Para compartir en móvil, súbelo a un servidor web.";
        statusDiv.style.background = "#2d1f2a";
        setTimeout(() => { statusDiv.style.display = 'none'; }, 4000);
        return;
      }
      if (navigator.clipboard && navigator.clipboard.writeText) {
        navigator.clipboard.writeText(urlToCopy).then(() => {
          statusDiv.style.display = 'block';
          statusDiv.innerHTML = "✅ Enlace copiado. ¡Comparte la encuesta Start-Ip!";
          statusDiv.style.background = "#0f2e1a";
          setTimeout(() => { statusDiv.style.display = 'none'; }, 3000);
        }).catch(() => fallbackCopy(urlToCopy));
      } else {
        fallbackCopy(urlToCopy);
      }
    }

    function fallbackCopy(text) {
      const textarea = document.createElement('textarea');
      textarea.value = text;
      document.body.appendChild(textarea);
      textarea.select();
      document.execCommand('copy');
      document.body.removeChild(textarea);
      statusDiv.style.display = 'block';
      statusDiv.innerHTML = "📋 Enlace copiado al portapapeles. Comparte tu opinión.";
      statusDiv.style.background = "#1e3a2f";
      setTimeout(() => { statusDiv.style.display = 'none'; }, 3000);
    }

    copyBtn.addEventListener('click', copyLinkToClipboard);

    function getSelectedRadioValue(name) {
      const radios = document.querySelectorAll(`input[name="${name}"]`);
      for (let radio of radios) {
        if (radio.checked) return radio.value;
      }
      return '❌ No respondido';
    }

    function buildEmailBody() {
      const categoria = getSelectedRadioValue('categoria');
      const tipo = getSelectedRadioValue('tipo');
      const funcion = getSelectedRadioValue('funcion');
      const frecuencia = getSelectedRadioValue('frecuencia');
      const monto = getSelectedRadioValue('monto');
      const desconfianza = getSelectedRadioValue('desconfianza');
      const diseno = getSelectedRadioValue('diseno');
      const social = getSelectedRadioValue('social');
      const pago = getSelectedRadioValue('pago');

      let sugerencia = document.querySelector('textarea[name="sugerencia"]').value.trim();
      if (sugerencia === "") sugerencia = "(No especificó)";

      let evaluador = document.querySelector('input[name="evaluador"]').value.trim();
      if (evaluador === "") evaluador = "Anónimo";

      const now = new Date();
      const fechaHora = now.toLocaleString();

      let body = "🏷️ ENCUESTA START-IP · APP DE SUBASTAS 🏷️\n";
      body += "─────────────────────────────────────────\n";
      body += `📅 Fecha: ${fechaHora}\n`;
      body += `👤 Evaluador: ${evaluador}\n\n`;
      body += "👥 EQUIPO START-IP:\n";
      body += "• Franklin Patzi Marce - Líder / PO / Tester\n";
      body += "• Angelica Burgos - Documentador\n";
      body += "• Jhoao Cesar Daza Vargas - Frontend\n";
      body += "• Lucio Daniel Ticona - Backend\n\n";
      body += "🔹 RESPUESTAS:\n";
      body += `1. Categorías favoritas → ${categoria}\n`;
      body += `2. Tipo de subasta → ${tipo}\n`;
      body += `3. Funcionalidad más valorada → ${funcion}\n`;
      body += `4. Frecuencia de uso → ${frecuencia}\n`;
      body += `5. Monto habitual de puja → ${monto}\n`;
      body += `6. Mayor desconfianza → ${desconfianza}\n`;
      body += `7. Estilo de diseño → ${diseno}\n`;
      body += `8. Funciones sociales → ${social}\n`;
      body += `9. Método de pago favorito → ${pago}\n`;
      body += `10. Sugerencia adicional → ${sugerencia}\n\n`;
      body += "💡 ¡Gracias por ayudar a mejorar Start-Ip!\n";
      body += "─────────────────────────────────────────\n";
      return body;
    }

    function showWarningIfIncomplete() {
      const requiredRadios = ['categoria', 'tipo', 'funcion', 'frecuencia', 'monto', 'desconfianza', 'diseno', 'social', 'pago'];
      let missing = [];
      for (let req of requiredRadios) {
        const anyChecked = document.querySelector(`input[name="${req}"]:checked`);
        if (!anyChecked) missing.push(req);
      }
      if (missing.length > 0) {
        let msg = "⚠️ Algunas preguntas no tienen respuesta:\n";
        if (missing.includes('categoria')) msg += "- Pregunta 1 (categorías)\n";
        if (missing.includes('tipo')) msg += "- Pregunta 2 (tipo de subasta)\n";
        if (missing.includes('funcion')) msg += "- Pregunta 3 (funcionalidad)\n";
        if (missing.includes('frecuencia')) msg += "- Pregunta 4 (frecuencia)\n";
        if (missing.includes('monto')) msg += "- Pregunta 5 (rango de puja)\n";
        if (missing.includes('desconfianza')) msg += "- Pregunta 6 (desconfianza)\n";
        if (missing.includes('diseno')) msg += "- Pregunta 7 (diseño app)\n";
        if (missing.includes('social')) msg += "- Pregunta 8 (funciones sociales)\n";
        if (missing.includes('pago')) msg += "- Pregunta 9 (método de pago)\n";
        msg += "\n¿Deseas enviar de todas formas? (respuestas incompletas)";
        return !confirm(msg);
      }
      return false;
    }

    function sendPrivateEvaluation() {
      const cancelled = showWarningIfIncomplete();
      if (cancelled) return;

      const subject = encodeURIComponent("Start-Ip - Preferencias para app de subastas");
      let bodyText = buildEmailBody();
      // mailto con destinatario fijo
      const mailtoLink = `mailto:${DESTINO_CORREO}?subject=${subject}&body=${encodeURIComponent(bodyText)}`;

      statusDiv.style.display = 'block';
      statusDiv.innerHTML = `📧 Abriendo correo hacia <strong>${DESTINO_CORREO}</strong>...<br>✏️ Puedes editar el mensaje antes de enviar.`;
      statusDiv.style.background = "#0f2e1e";
      setTimeout(() => {
        window.location.href = mailtoLink;
      }, 200);
      setTimeout(() => {
        if (statusDiv) statusDiv.style.opacity = "0.8";
      }, 5000);
    }

    sendBtn.addEventListener('click', sendPrivateEvaluation);

    const form = document.getElementById('evalForm');
    form.addEventListener('keypress', function(e) {
      if (e.key === 'Enter' && (e.target.tagName !== 'TEXTAREA' && e.target.type !== 'text')) {
        e.preventDefault();
      }
    });

    // Mejora visual para móvil si la url es muy larga
    if (window.innerWidth <= 600) {
      let shortHint = window.location.href;
      if (shortHint.length > 70 && !shortHint.startsWith('file:')) {
        let displayShort = shortHint.substring(0, 55) + "…";
        urlDisplaySpan.innerText = displayShort;
        urlDisplaySpan.title = shortHint;
      } else if (shortHint.startsWith('file:')) {
        urlDisplaySpan.innerText = "📁 Archivo local → comparte subiendo a hosting";
      }
    }
  })();
</script>
</body>
</html>
