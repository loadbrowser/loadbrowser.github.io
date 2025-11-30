<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Софт — загрузки</title>
  <meta name="description" content="Скачайте Яндекс.Браузер, Яндекс.Диск и Яндекс.Браузер с VPN. Легко. Быстро. Надежно." />
  <style>
    :root{
      --bg:#f7f9fb;
      --card:#ffffff;
      --muted:#6b7280;
      --accent:#0061ff;
      --glass: rgba(255,255,255,0.6);
      --radius:14px;
      --shadow: 0 6px 18px rgba(20,23,33,0.06);
      --maxw:1100px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      color-scheme: light;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      background:linear-gradient(180deg,var(--bg),#ffffff 60%);
      color:#0f1724;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      display:flex;
      align-items:flex-start;
      justify-content:center;
      padding:48px 20px;
    }

    .wrap{width:100%;max-width:var(--maxw)}

    header{
      display:flex;align-items:center;justify-content:space-between;margin-bottom:28px
    }
    .brand{display:flex;align-items:center;gap:14px}
    .logo{width:48px;height:48px;display:inline-grid;place-items:center;border-radius:10px;background:linear-gradient(135deg,var(--accent),#00a3ff);color:#fff;font-weight:700}
    h1{font-size:20px;margin:0}
    p.lead{margin:6px 0 0;color:var(--muted);font-size:13px}

    .hero{
      background:var(--card);
      border-radius:var(--radius);
      padding:20px;
      box-shadow:var(--shadow);
      display:flex;gap:20px;align-items:center;margin-bottom:22px
    }
    .hero-left{flex:1}
    .hero-right{width:220px;flex-shrink:0}
    .hero h2{margin:0 0 6px;font-size:18px}
    .hero p{margin:0;color:var(--muted);font-size:14px}
    .cta{display:inline-block;margin-top:12px;padding:10px 14px;border-radius:10px;background:linear-gradient(90deg,var(--accent),#00a3ff);color:#fff;text-decoration:none;font-weight:600}

    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .card{
      background:var(--card);
      border-radius:12px;padding:18px;box-shadow:var(--shadow);display:flex;flex-direction:column;gap:12px;min-height:170px
    }
    .card .icon{width:56px;height:56px;border-radius:10px;background:var(--glass);display:grid;place-items:center;font-weight:700}
    .card h3{margin:0;font-size:16px}
    .card p{margin:0;color:var(--muted);font-size:13px}
    .actions{margin-top:auto;display:flex;gap:8px}
    .btn{padding:8px 12px;border-radius:10px;text-decoration:none;font-weight:600;border:1px solid rgba(15,23,36,0.06);background:transparent;color:var(--accent)}
    .btn.primary{background:var(--accent);color:#fff;border:none}

    footer{margin-top:18px;color:var(--muted);font-size:13px;text-align:center}

    /* Responsive */
    @media (max-width:900px){
      .grid{grid-template-columns:repeat(2,1fr)}
      .hero-right{display:none}
    }
    @media (max-width:560px){
      .grid{grid-template-columns:1fr}
      header{flex-direction:column;align-items:flex-start;gap:12px}
      .hero{flex-direction:column;align-items:flex-start}
    }
  </style>
</head>
<body>
  <div class="wrap">

    <section class="block block-header">
      <header>
        <div class="brand">
          <div class="logo">SF</div>
          <div>
            <h1>Софт — быстрые загрузки</h1>
            <p class="lead">Каталог полезных утилит и браузеров. Проверенные сборки и инструкции.</p>
          </div>
        </div>
        <nav aria-label="Главное меню">
          <a href="#apps" class="btn">Перейти к загрузкам</a>
        </nav>
      </header>
    </section>

    <section class="block block-hero" role="region" aria-labelledby="hero-title">
      <div class="hero">
        <div class="hero-left">
          <h2 id="hero-title">Скачать безопасный софт для Windows и macOS</h2>
          <p>Яндекс.Браузер, Яндекс.Диск и версия Яндекс.Браузера с VPN. Инструкции по установке и ссылки на официальные страницы.</p>
          <a class="cta" href="#apps">Скачать сейчас</a>
        </div>
        <div class="hero-right">
          <picture>
            <svg width="220" height="120" viewBox="0 0 220 120" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
              <rect x="0" y="0" width="220" height="120" rx="12" fill="#f3f6fb"/>
              <rect x="12" y="18" width="196" height="84" rx="8" fill="#fff" stroke="#e6eef9"/>
              <circle cx="40" cy="60" r="20" fill="#0061ff"/>
              <rect x="74" y="40" width="120" height="40" rx="6" fill="#eef6ff"/>
            </svg>
          </picture>
        </div>
      </div>
    </section>

    <section id="apps" class="block block-apps">
      <div class="grid">
        <!-- карточки остаются как есть -->
        <article class="card" aria-labelledby="yab-title">...</article>
        <article class="card" aria-labelledby="yd-title">...</article>
        <article class="card" aria-labelledby="vpn-title">...</article>
      </div>
      <section style="margin-top:18px;background:transparent;padding:14px;border-radius:10px;">
        <p style="margin:0;color:var(--muted)">Примечание: ссылки ведут на официальные страницы сервисов.</p>
      </section>
    </section>

    <section class="block block-footer">
      <footer>
        <p>© 2025 Софт. Страница для GitHub Pages.</p>
      </footer>
    </section>

  </div>
</body>
</html>
