<!doctype html>
<html lang="de">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>VOXchains – Vocal Presets & Vocal Chains für Musiker</title>
  <meta name="description" content="Professionelle Vocal Presets & Chains für Musiker | Einfache Installation, sofortiger Klang-Boost" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg1: #0f0426; /* dunkler Lila-Ton */
      --accent1: #7afcff; /* türkis */
      --accent2: #ff66c4; /* pink */
      --accent3: #7b61ff; /* violett */
      --glass: rgba(255,255,255,0.06);
      --card-shadow: 0 10px 30px rgba(11,8,30,0.6);
      --radius: 18px;
      --max-width: 1200px;
      font-size: 16px;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: 'Poppins', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
      background: radial-gradient(1200px 400px at 10% 20%, rgba(123,97,255,0.15), transparent),
                  linear-gradient(180deg, #0b0530 0%, #160833 40%, #1f0b3a 100%);
      color:#e9eef8;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      padding-bottom:60px;
    }
    .container{
      max-width:var(--max-width);
      margin:40px auto;
      padding:24px;
    }
    header{
      display:flex;
      justify-content:space-between;
      align-items:center;
      padding:20px 0;\    }
    .brand{
      display:flex;align-items:center;gap:12px;
    }
    .logo{
      width:54px;height:54px;border-radius:12px;background:linear-gradient(135deg,var(--accent1),var(--accent2));
      display:flex;align-items:center;justify-content:center;font-weight:800;color:#08192a;box-shadow:0 6px 20px rgba(122,252,255,0.08);
    }
    .brand h1{margin:0;font-size:1.125rem;letter-spacing:0.6px}
    nav a{color:rgba(233,238,248,0.8);text-decoration:none;margin-left:18px;font-weight:600}
    nav a.cta{background:linear-gradient(90deg,var(--accent1),var(--accent2));color:#071223;padding:10px 16px;border-radius:12px}

    /* Hero */
    .hero{
      display:grid;grid-template-columns:1fr 460px;gap:28px;align-items:center;margin-top:18px;
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:28px;border-radius:20px;box-shadow:var(--card-shadow);
      border:1px solid rgba(255,255,255,0.03);
    }
    .hero-left{padding:12px}
    .kicker{color:var(--accent1);font-weight:700;letter-spacing:2px;font-size:0.85rem}
    .headline{font-size:2.1rem;line-height:1.05;margin:14px 0;font-weight:800;color:white}
    .sub{color:rgba(233,238,248,0.75);margin-bottom:18px}
    .cta-row{display:flex;gap:12px;align-items:center}
    .btn-primary{background:linear-gradient(90deg,var(--accent1),var(--accent3));border:none;padding:14px 20px;border-radius:14px;font-weight:700;color:#041225;cursor:pointer;box-shadow:0 12px 30px rgba(123,97,255,0.12)}
    .btn-ghost{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:12px 18px;border-radius:12px;color:rgba(233,238,248,0.9);cursor:pointer}

    .hero-right{
      position:relative;height:320px;background:linear-gradient(135deg, rgba(255,255,255,0.03), rgba(255,255,255,0.01));border-radius:14px;overflow:hidden;display:flex;align-items:center;justify-content:center;
    }
    .device-card{width:420px;height:260px;border-radius:12px;background:linear-gradient(180deg,#03102a,#0b1b3a);transform:rotate(-8deg);box-shadow:0 20px 40px rgba(0,0,0,0.6);border:1px solid rgba(255,255,255,0.03);display:flex;flex-direction:column;justify-content:center;align-items:center}
    .device-card .chip{width:100%;padding:10px 18px;display:flex;justify-content:space-between;align-items:center}
    .chip .title{font-weight:700}

    /* Features */
    .features{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:28px}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:18px;border-radius:14px;border:1px solid rgba(255,255,255,0.03)}
    .card h4{margin:0 0 8px 0}
    .price{font-weight:800;font-size:1.6rem;color:var(--accent1)}

    /* Audio Preview */
    .preview{margin-top:22px;padding:18px;border-radius:12px;background:linear-gradient(90deg, rgba(123,97,255,0.06), rgba(122,252,255,0.02));display:flex;gap:14px;align-items:center}
    audio{width:100%;outline:none}

    /* Testimonials */
    .testimonials{margin-top:28px;display:flex;gap:14px}
    .testimonial{flex:1;padding:16px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border:1px solid rgba(255,255,255,0.03)}

    /* Kontakt */
    .contact{display:flex;gap:20px;margin-top:28px}
    .contact form{flex:1;padding:18px;border-radius:12px;background:var(--glass);border:1px solid rgba(255,255,255,0.03)}
    input,textarea{width:100%;padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,0.06);background:transparent;color:white;margin-bottom:12px}
    input::placeholder,textarea::placeholder{color:rgba(233,238,248,0.5)}
    .contact .info{width:320px;padding:18px;border-radius:12px;background:linear-gradient(90deg, rgba(123,97,255,0.04), rgba(122,252,255,0.02));}

    footer{margin-top:40px;text-align:center;color:rgba(233,238,248,0.6)}

    /* Responsive */
    @media (max-width:980px){.hero{grid-template-columns:1fr;}.features{grid-template-columns:1fr 1fr}.contact{flex-direction:column}.hero-right{height:260px}.device-card{transform:none}}
    @media (max-width:600px){.features{grid-template-columns:1fr}.headline{font-size:1.6rem}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">VC</div>
        <div>
          <h1>VOXchains</h1>
          <div style="font-size:0.85rem;color:rgba(233,238,248,0.6);margin-top:3px">Vocal Presets & Chains für Musiker</div>
        </div>
      </div>
      <nav>
        <a href="#features">Leistungen</a>
        <a href="#preview">Preview</a>
        <a href="#preise">Preise</a>
        <a href="#kontakt" class="cta">Jetzt kaufen</a>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div class="hero-left">
          <div class="kicker">Made for Vocals • Ready to Use</div>
          <h2 class="headline">Booste deinen Gesang – professionelle Vocal Chains, die sofort funktionieren</h2>
          <p class="sub">Fertige Presets & Chains für Studio und Live. Schnelle Installation, klarer Sound, perfektes Finish für deine Stimme.</p>
          <div class="cta-row">
            <button class="btn-primary" onclick="document.getElementById('kontakt').scrollIntoView({behavior:'smooth'})">Jetzt kaufen</button>
            <button class="btn-ghost" onclick="document.getElementById('preview').scrollIntoView({behavior:'smooth'})">Kostenlose Demo hören</button>
          </div>

          <div class="preview" id="preview" style="margin-top:18px">
            <div style="width:76px;text-align:center;font-weight:700;color:#071225;background:linear-gradient(90deg,var(--accent1),var(--accent2));padding:12px;border-radius:10px">Demo</div>
            <div style="flex:1">
              <div style="font-weight:700">Vocal Preset Demo</div>
              <audio controls>
                <source src="demo-vocal-presets.mp3" type="audio/mpeg">
                Ihr Browser unterstützt das Audio-Element nicht.
              </audio>
            </div>
          </div>
        </div>

        <div class="hero-right">
          <div class="device-card">
            <div class="chip"><div class="title">VOXchains • Premium Vocal Chain</div><div style="opacity:0.6">v1.0</div></div>
            <div style="text-align:center;padding:16px;color:rgba(255,255,255,0.92)">
              <div style="font-size:1.4rem;font-weight:800">Klarer, voller Sound</div>
              <div style="margin-top:8px;opacity:0.8">EQ • Kompressor • De-Esser • Saturation • Reverb</div>
            </div>
          </div>
        </div>
      </section>

      <section id="features" class="features">
        <div class="card">
          <h4>Ein-Klick-Installation</h4>
          <p>Importiere unsere Presets in deine DAW (Ableton, Logic, FL Studio) – fertig.</p>
        </div>
        <div class="card">
          <h4>Mix Ready</h4>
          <p>Optimiert für Broadcast, Streaming und professionelle Produktionen.</p>
        </div>
        <div class="card">
          <h4>Flexibel & Skalierbar</h4>
          <p>Feinjustierbare Module: mehr Saturation, weniger Reverb — ganz nach Geschmack.</p>
        </div>
      </section>

      <section id="preise" style="margin-top:20px">
        <div style="display:flex;gap:14px;flex-wrap:wrap">
          <div class="card" style="flex:1;min-width:220px">
            <h4>Starter</h4>
            <p>1 Vocal Chain • geeignet für Home-Recording</p>
            <div class="price">9,99 €</div>
            <button class="btn-primary" style="margin-top:12px" onclick="openCheckout('Starter')">Kaufen</button>
          </div>
          <div class="card" style="flex:1;min-width:220px">
            <h4>Pro</h4>
            <p>3 Vocal Chains • Mixing-Routinen • EQ-Templates</p>
            <div class="price">24,99 €</div>
            <button class="btn-primary" style="margin-top:12px" onclick="openCheckout('Pro')">Kaufen</button>
          </div>
          <div class="card" style="flex:1;min-width:220px">
            <h4>Ultimate</h4>
            <p>Alle Chains • persönliches Preset-Feedback (1x)</p>
            <div class="price">59,99 €</div>
            <button class="btn-primary" style="margin-top:12px" onclick="openCheckout('Ultimate')">Kaufen</button>
          </div>
        </div>

        <div class="testimonials">
          <div class="testimonial">
            <strong>Anna, Sängerin</strong>
            <p>„Endlich ein Preset, das meine Stimme nicht verhält — klingt sofort warm und präsent.“</p>
          </div>
          <div class="testimonial">
            <strong>Lukas, Producer</strong>
            <p>„Perfekt für schnelle Sessions. Spart mir Stunden im Mix.“</p>
          </div>
        </div>
      </section>

      <section id="kontakt" class="contact">
        <form onsubmit="event.preventDefault();submitForm()">
          <h3 style="margin-top:0">Kauf / Kontakt</h3>
          <input type="text" id="name" placeholder="Dein Name" required />
          <input type="email" id="email" placeholder="E-Mail" required />
          <select id="produkt" style="padding:12px;border-radius:10px;margin-bottom:12px;background:transparent;color:white">
            <option value="Starter">Starter – 9,99 €</option>
            <option value="Pro">Pro – 24,99 €</option>
            <option value="Ultimate">Ultimate – 59,99 €</option>
          </select>
          <textarea id="message" rows="4" placeholder="Nachricht / spezielle Wünsche (optional)"></textarea>
          <button class="btn-primary" type="submit">Bestellen / Anfrage senden</button>
        </form>
        <div class="info">
          <h4>Warum VOXchains?</h4>
          <p>Professionelle Chains für Studio & Live. Kompatibel mit allen gängigen DAWs. Schnell einsetzbar, sofort hörbare Verbesserung.</p>
          <h4 style="margin-top:12px">Zahlung & Lieferung</h4>
          <p>Nach Zahlung erhältst du einen Download-Link per E-Mail. Demo-Versionen sind kostenlos.</p>
          <h4 style="margin-top:12px">Support</h4>
          <p>support@voxchains.example</p>
        </div>
      </section>

    </main>

    <footer>
      <p>© 2025 VOXchains – Vocal Presets & Chains für Musiker • Made with ❤️</p>
    </footer>
  </div>

  <script>
    function openCheckout(plan){
      // Platzhalter-Funktion: Hier könnt ihr euren Checkout integrieren (PayPal, Stripe, Gumroad etc.)
      alert('Checkout: ' + plan + '\nIntegriere hier deinen Zahlungsanbieter (PayPal / Stripe / Gumroad).');
    }
    function submitForm(){
      const name = document.getElementById('name').value;
      const email = document.getElementById('email').value;
      const produkt = document.getElementById('produkt').value;
      // Beispiel: statt echten Versand -> einfach Email anzeigen
      alert('Vielen Dank, ' + name + '!\nWir haben deine Anfrage für: ' + produkt + ' erhalten.\nWir kontaktieren dich per E-Mail: ' + email);
      // TODO: Hier könnt ihr fetch() nutzen, um Daten an euren Server zu senden.
      document.getElementById('name').value='';
      document.getElementById('email').value='';
      document.getElementById('message').value='';
    }
  </script>
</body>
</html>
