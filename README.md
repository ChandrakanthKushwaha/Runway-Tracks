<!DOCTYPE html><html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Runway Tracks – Refer & Earn</title>
  <meta name="description" content="Runway Tracks – Stylish track pants. Refer & Earn ₹100 on every referral!" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --navy:#0e2330;
      --ink:#0b1b24;
      --off:#f7f5ef;
      --muted:#9fb3bf;
      --yellow:#f5b700;
      --orange:#ff8a00;
      --accent: linear-gradient(90deg,var(--yellow),var(--orange));
      --card:#112a39;
      --pill:#0b202d;
      --pants:#565c61; /* grey base for pants */
    }
    *{box-sizing:border-box}
    html,body{margin:0;height:100%;font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;color:var(--off);background:radial-gradient(1200px 800px at 20% -10%,#163547,var(--navy));}
    a{color:inherit;text-decoration:none}
    .container{width:min(1100px,92vw);margin-inline:auto}
    header{position:sticky;top:0;backdrop-filter:saturate(1.2) blur(6px);background:rgba(9,26,35,.6);border-bottom:1px solid rgba(255,255,255,.06);z-index:10}
    .nav{display:flex;align-items:center;justify-content:space-between;padding:.9rem 0}
    .brand{display:flex;gap:.75rem;align-items:center;font-weight:800;letter-spacing:.3px}
    .brand svg{width:40px;height:40px}
    .brand span{font-size:1.1rem}
    .cta{display:inline-flex;align-items:center;gap:.5rem;padding:.65rem 1rem;border-radius:999px;background:var(--accent);color:#0b1b24;font-weight:700;box-shadow:0 8px 24px rgba(255,166,0,.25)}/* Hero */
.hero{display:grid;grid-template-columns:1.1fr .9fr;gap:2.25rem;align-items:center;padding:clamp(2rem,6vw,5rem) 0 2rem}
.hero h1{font-size:clamp(2rem,5vw,3.5rem);line-height:1.1;margin:0 0 .6rem 0}
.lead{font-size:clamp(1rem,2.2vw,1.25rem);color:var(--muted);margin-bottom:1.2rem}
.badge{display:inline-block;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.12);padding:.35rem .7rem;border-radius:999px;font-size:.88rem;margin-bottom:.75rem}
.hero .actions{display:flex;flex-wrap:wrap;gap:.8rem}
.ghost{display:inline-flex;align-items:center;gap:.5rem;padding:.65rem 1rem;border-radius:999px;border:1px solid rgba(255,255,255,.18);background:rgba(255,255,255,.04)}

/* Pants illustration */
.mock{display:grid;place-items:center}
.card{background:var(--card);border:1px solid rgba(255,255,255,.08);border-radius:22px;padding:1.25rem;box-shadow:0 10px 30px rgba(0,0,0,.25)}
.pants svg{width:min(360px,78vw);height:auto;display:block}

/* Sections */
section{padding:3rem 0}
h2{font-size:clamp(1.4rem,3.2vw,2rem);margin:0 0 .6rem 0}
.grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1rem}
.feature{background:var(--pill);border:1px solid rgba(255,255,255,.07);padding:1rem;border-radius:18px}
.feature b{display:block;margin-bottom:.4rem}

/* Footer */
footer{padding:2.5rem 0;color:var(--muted);border-top:1px solid rgba(255,255,255,.07)}

/* Responsive */
@media (max-width:900px){
  .hero{grid-template-columns:1fr;gap:1.5rem}
  .grid{grid-template-columns:1fr}
  .brand span{font-size:1rem}
}

  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <a class="brand" href="#top" aria-label="Runway Tracks home">
        <!-- Simple circle logo with pants -->
        <svg viewBox="0 0 64 64" aria-hidden="true">
          <defs>
            <linearGradient id="g1" x1="0" x2="1">
              <stop offset="0" stop-color="#f5b700"/>
              <stop offset="1" stop-color="#ff8a00"/>
            </linearGradient>
          </defs>
          <circle cx="32" cy="32" r="30" fill="none" stroke="url(#g1)" stroke-width="4" />
          <g transform="translate(16,10)">
            <path fill="var(--pants)" d="M6 16c0-4 2-6 10-6s10 2 10 6v20c0 2-2 8-3 10h-3c-1-3-2-8-3-11-1 3-2 8-3 11h-3c-1-2-3-8-3-10V16z"/>
            <rect x="3" y="15" width="2" height="28" rx="1" fill="url(#g1)"/>
            <rect x="27" y="15" width="2" height="28" rx="1" fill="url(#g1)"/>
          </g>
        </svg>
        <span>Runway&nbsp;Tracks</span>
      </a>
      <a class="cta" href="tel:+919502907095">📞&nbsp;9502907095</a>
    </div>
  </header>  <main id="top">
    <section class="hero container">
      <div>
        <div class="badge">Street‑ready comfort</div>
        <h1>Premium Track Pants for Everyday Hustle</h1>
        <p class="lead">Refer a friend and <b>earn ₹100 on every referral</b>. Built for style, stretch and stamina — Runway Tracks keeps you moving.</p>
        <div class="actions">
          <a class="cta" href="https://wa.me/919502907095?text=Hi%20Runway%20Tracks!%20I'm%20interested%20in%20your%20track%20pants." target="_blank" rel="noopener">Message on WhatsApp</a>
          <a class="ghost" href="#how">How it works</a>
        </div>
      </div>
      <div class="mock">
        <div class="card pants" aria-label="Product mockup: track pants">
          <!-- Standalone pants illustration (grey with yellow/orange side stripes) -->
          <svg viewBox="0 0 280 420" role="img" aria-label="Grey track pants with yellow/orange side stripes">
            <defs>
              <linearGradient id="stripe" x1="0" x2="1">
                <stop offset="0" stop-color="#f5b700"/>
                <stop offset="1" stop-color="#ff8a00"/>
              </linearGradient>
            </defs>
            <!-- waistband -->
            <rect x="70" y="32" width="140" height="30" rx="6" fill="#263642" />
            <rect x="70" y="62" width="140" height="10" fill="#1b2b36" />
            <!-- body -->
            <path d="M70 72c0-10 18-20 70-20s70 10 70 20v220c0 20-18 84-28 104h-26c-8-28-14-70-22-98-8 28-14 70-22 98h-26c-10-20-28-84-28-104V72z" fill="var(--pants)" stroke="#1a2a34" stroke-width="3"/>
            <!-- stripes -->
            <rect x="60" y="88" width="10" height="260" rx="5" fill="url(#stripe)"/>
            <rect x="210" y="88" width="10" height="260" rx="5" fill="url(#stripe)"/>
            <!-- cuffs -->
            <rect x="82" y="356" width="44" height="20" rx="6" fill="#2a3a46"/>
            <rect x="154" y="356" width="44" height="20" rx="6" fill="#2a3a46"/>
          </svg>
        </div>
      </div>
    </section><section id="how">
  <div class="container">
    <h2>How the Referral Works</h2>
    <div class="grid">
      <div class="feature"><b>1) Share</b> Send your unique message or this page to a friend who loves comfy streetwear.</div>
      <div class="feature"><b>2) They Buy</b> Your friend orders a pair of Runway Tracks via call or WhatsApp.</div>
      <div class="feature"><b>3) You Earn</b> You get <b>₹100</b> instant credit for every successful referral. No limits.</div>
    </div>
  </div>
</section>

<section id="contact">
  <div class="container">
    <h2>Order or Refer Now</h2>
    <p class="lead">Call us or ping on WhatsApp. Fast responses during 9:00–20:00 IST.</p>
    <div class="actions">
      <a class="cta" href="tel:+919502907095">📞 Call 9502907095</a>
      <a class="ghost" href="https://wa.me/919502907095?text=Hi%20Runway%20Tracks!%20I'd%20like%20to%20order%20/\nrefer%20a%20friend." target="_blank" rel="noopener">💬 Chat on WhatsApp</a>
    </div>
  </div>
</section>

  </main>  <footer>
    <div class="container">
      © <span id="year"></span> Runway Tracks • All rights reserved.
    </div>
  </footer>  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script></body>
</html>
