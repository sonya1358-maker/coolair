<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Cool Air Solutions</title>
  <meta name="description" content="Reliable air conditioning installation, repair, and maintenance." />
  <style>
    :root{
      --bg:#ffffff;
      --text:#0b1b2b;
      --muted:#5b6b7a;
      --line:#e6eef7;
      --brand:#1976d2;
      --brand2:#43a7ff;
      --card:#f7fbff;
      --shadow: 0 10px 30px rgba(16, 60, 120, .10);
      --radius:16px;
    }

    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial, sans-serif;
      background: var(--bg);
      color: var(--text);
    }
    a{color:inherit}

    .wrap{
      max-width: 560px;
      margin: 0 auto;
      padding: 14px 16px 40px;
    }

    /* Top */
    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:12px;
      padding: 6px 2px 10px;
    }
    .brand{
      font-weight:800;
      letter-spacing:.2px;
      font-size: 18px;
      color: var(--brand);
      white-space:nowrap;
    }
    .tag{
      font-size:12px;
      color:var(--muted);
      text-align:right;
      line-height:1.2;
    }

    /* Hero */
    .hero{
      border: 1px solid var(--line);
      border-radius: var(--radius);
      overflow:hidden;
      box-shadow: var(--shadow);
      background: linear-gradient(180deg, rgba(25,118,210,.10), rgba(67,167,255,.06));
    }

    .hero-img{
      height: 180px;
      background:
        radial-gradient(900px 240px at 10% 10%, rgba(67,167,255,.55), transparent 60%),
        radial-gradient(700px 240px at 90% 0%, rgba(25,118,210,.45), transparent 55%),
        linear-gradient(135deg, rgba(255,255,255,.85), rgba(255,255,255,.10)),
        url("https://images.unsplash.com/photo-1569428034239-f9565e32e224?auto=format&fit=crop&w=1400&q=60");
      background-size: cover;
      background-position: center;
      position:relative;
    }

    .hero-img::after{
      content:"";
      position:absolute; inset:0;
      background: linear-gradient(180deg, rgba(255,255,255,.10), rgba(255,255,255,.92));
    }

    .hero-body{
      padding: 14px 16px 16px;
    }
    h1{
      margin: 2px 0 6px;
      font-size: 22px;
      line-height:1.2;
    }
    .sub{
      margin:0;
      color: var(--muted);
      line-height:1.5;
      font-size: 14px;
    }

    /* Main buttons */
    .nav{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
      padding: 14px 16px 16px;
    }
    .btn{
      display:flex;
      align-items:center;
      justify-content:center;
      padding: 14px 12px;
      min-height: 48px;
      border-radius: 14px;
      border: 1px solid var(--line);
      background: #fff;
      font-weight: 800;
      text-decoration:none;
      box-shadow: 0 8px 18px rgba(25,118,210,.08);
      user-select:none;
      -webkit-tap-highlight-color: transparent;
    }
    .btn:active{ transform: translateY(1px); }

    /* Sections */
    section{
      margin-top: 14px;
      border: 1px solid var(--line);
      border-radius: var(--radius);
      background: #fff;
      box-shadow: var(--shadow);
      overflow:hidden;
    }
    .sec-h{
      padding: 14px 16px 10px;
      border-bottom: 1px solid var(--line);
      background: var(--card);
      font-weight: 900;
      letter-spacing:.2px;
    }
    .sec-b{ padding: 14px 16px 16px; }
    .grid{
      display:grid;
      gap:10px;
    }
    .card{
      border:1px solid var(--line);
      border-radius: 14px;
      padding: 12px 12px;
      background: #fff;
    }
    .card b{ display:block; margin-bottom:6px; }
    .small{ color: var(--muted); font-size: 13px; line-height:1.45; margin:0; }

    /* Order */
    form{
      display:grid; gap:10px;
    }
    input, textarea{
      width:100%;
      border:1px solid var(--line);
      border-radius: 12px;
      padding: 12px 12px;
      font-size: 14px;
      outline:none;
    }
    textarea{ min-height: 110px; resize: vertical; }
    .submit{
      border:none;
      border-radius: 14px;
      padding: 14px 12px;
      font-weight: 900;
      background: linear-gradient(90deg, var(--brand), var(--brand2));
      color:#fff;
      cursor:pointer;
      box-shadow: 0 10px 22px rgba(25,118,210,.22);
    }

    /* Contact quick links */
    .quick{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:10px;
      margin-top: 10px;
    }
    .pill{
      display:flex; align-items:center; justify-content:center;
      padding:12px 10px;
      border-radius: 999px;
      border:1px solid var(--line);
      text-decoration:none;
      font-weight:800;
      background:#fff;
    }

    footer{
      text-align:center;
      color: var(--muted);
      font-size: 12px;
      margin-top: 14px;
      padding: 10px 0 0;
    }
  </style>
</head>

<body>
  <div class="wrap">
    <header>
      <div class="brand">Cool Air Solutions</div>
      <div class="tag">AC Installation · Repair · Maintenance</div>
    </header>

    <div class="hero">
      <div class="hero-img" aria-label="cool hero image"></div>
      <div class="hero-body">
        <h1>Stay cool. Fast, clean, reliable.</h1>
        <p class="sub">Simple dummy site for mobile. Replace phone/email and portfolio images later.</p>
      </div>

      <!-- Main Buttons -->
      <nav class="nav" aria-label="Main navigation">
        <a class="btn" href="#about">About Company</a>
        <a class="btn" href="#portfolio">Portfolio</a>
        <a class="btn" href="#order">Order</a>
        <a class="btn" href="#contact">Contact</a>
      </nav>
    </div>

    <!-- ABOUT -->
    <section id="about">
      <div class="sec-h">About Company</div>
      <div class="sec-b">
        <div class="grid">
          <div class="card">
            <b>Who we are</b>
            <p class="small">We provide air conditioning installation, repair, and seasonal maintenance for homes and small businesses.</p>
          </div>
          <div class="card">
            <b>What we do</b>
            <p class="small">New installs · Tune-ups · Filter replacement · Thermostat setup · Emergency repair (dummy text).</p>
          </div>
          <div class="card">
            <b>Service area</b>
            <p class="small">Your city + nearby areas (edit later).</p>
          </div>
        </div>
      </div>
    </section>

    <!-- PORTFOLIO -->
    <section id="portfolio">
      <div class="sec-h">Portfolio</div>
      <div class="sec-b">
        <div class="grid">
          <div class="card">
            <b>Residential Install</b>
            <p class="small">Mini-split installation (before/after photos can go here).</p>
          </div>
          <div class="card">
            <b>Commercial Maintenance</b>
            <p class="small">Seasonal HVAC service for small office.</p>
          </div>
          <div class="card">
            <b>Emergency Repair</b>
            <p class="small">Same-day troubleshooting and part replacement.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- ORDER -->
    <section id="order">
      <div class="sec-h">Order</div>
      <div class="sec-b">
        <p class="small" style="margin:0 0 10px;">
          Dummy request form (does not submit anywhere). You can connect it later.
        </p>
        <form onsubmit="event.preventDefault(); alert('Dummy site: request saved (not really).');">
          <input type="text" placeholder="Name" aria-label="Name" />
          <input type="tel" placeholder="Phone" aria-label="Phone" />
          <input type="email" placeholder="Email" aria-label="Email" />
          <textarea placeholder="What do you need? (install / repair / maintenance)" aria-label="Message"></textarea>
          <button class="submit" type="submit">Submit Request</button>
        </form>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact">
      <div class="sec-h">Contact</div>
      <div class="sec-b">
        <div class="grid">
          <div class="card">
            <b>Contact info</b>
            <p class="small" style="margin:0 0 8px;">Phone: (410) 555-1234</p>
            <p class="small" style="margin:0 0 8px;">Email: info@coolairsolutions.com</p>
            <p class="small" style="margin:0;">Address: 123 Main St, Your City</p>

            <div class="quick">
              <a class="pill" href="tel:+14105551234">📞 Call</a>
              <a class="pill" href="sms:+14105551234">💬 Text</a>
              <a class="pill" href="mailto:info@coolairsolutions.com?subject=Service%20Request">✉️ Email</a>
              <a class="pill" href="https://maps.google.com/?q=123%20Main%20St%20Your%20City" target="_blank" rel="noopener">🗺️ Map</a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <footer>© 2025 Cool Air Solutions. Dummy website.</footer>
  </div>
</body>
</html>
