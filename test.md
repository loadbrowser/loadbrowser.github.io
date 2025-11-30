<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Софт — загрузки</title>
  <meta name="description" content="Скачайте Яндекс.Браузер, Яндекс.Диск и Яндекс.Браузер с VPN. Легко. Быстро. Надежно.">
  <style>
    :root {
      --bg: #f5f7fa;
      --card: #ffffff;
      --accent: #0061ff;
      --muted: #6b7280;
      --radius: 12px;
      --shadow: 0 4px 12px rgba(0,0,0,0.08);
      --maxw: 1100px;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }
    body { background: var(--bg); color: #111; display: flex; justify-content: center; font-size: 16px; line-height: 1.5; }

    .wrap { max-width: var(--maxw); width: 100%; padding: 40px 20px; }

    /* Header */
    header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 40px; flex-wrap: wrap; }
    .logo { font-weight: bold; font-size: 22px; color: var(--accent); }
    nav a { text-decoration: none; color: #fff; background: var(--accent); padding: 10px 16px; border-radius: var(--radius); font-weight: 600; }

    /* Hero */
    .hero { background: var(--card); border-radius: var(--radius); box-shadow: var(--shadow); display: flex; gap: 20px; padding: 30px; margin-bottom: 40px; flex-wrap: wrap; }
    .hero-text { flex: 1; min-width: 280px; }
    .hero-text h1 { font-size: 28px; margin-bottom: 12px; }
    .hero-text p { color: var(--muted); margin-bottom: 16px; }
    .hero-text a { text-decoration: none; color: #fff; background: var(--accent); padding: 10px 16px; border-radius: var(--radius); font-weight: 600; }
    .hero-img { flex: 1; min-width: 220px; display: flex; justify-content: center; align-items: center; }
    .hero-img svg { width: 220px; height: 140px; }

    /* Apps Grid */
    .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-bottom: 40px; }
    .card { background: var(--card); border-radius: var(--radius); box-shadow: var(--shadow); padding: 20px; display: flex; flex-direction: column; gap: 12px; }
    .card h3 { font-size: 20px; margin-bottom: 6px; }
    .card p { color: var(--muted); font-size: 14px; flex: 1; }
    .card .actions { display: flex; gap: 10px; margin-top: 12px; }
    .card .actions a { text-decoration: none; padding: 8px 14px; border-radius: var(--radius); font-weight: 600; border: 1px solid rgba(0,0,0,0.1); }
    .card .actions a.primary { background: var(--accent); color: #fff; border: none; }

    /* Footer */
    footer { text-align: center; color: var(--muted); font-size: 14px; padding: 20px 0; }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="logo">Софт</div>
      <nav>
        <a href="#apps">Загрузки</a>
      </nav>
    </header>

    <section class="hero">
      <div class="hero-text">
        <h1>Безопасный софт для Windows и macOS</h1>
        <p>Скачайте Яндекс.Браузер, Яндекс.Диск и Яндекс.Браузер с VPN. Легко, быстро, надежно.</p>
        <a href="#apps">Скачать</a>
      </div>
      <div class="hero-img">
        <svg viewBox="0 0 220 140" fill="none" xmlns="http://www.w3.org/2000/svg">
          <rect x="0" y="0" width="220" height="140" rx="12" fill="#e3ebf6"/>
          <circle cx="60" cy="70" r="30" fill="#0061ff"/>
          <rect x="110" y="50" width="100" height="40" rx="6" fill="#cce0ff"/>
        </svg>
      </div>
    </section>

    <main id="apps" class="grid">
      <div class="card">
        <h3>Яндекс.Браузер</h3>
        <p>Быстрый браузер с защитой от фишинга и встроенными сервисами. Поддержка расширений.</p>
        <div class="actions">
          <a class="primary" href="https://browser.yandex.ru/" target="_blank" rel="noopener">Официальный сайт</a>
          <a href="#">Инструкция</a>
        </div>
      </div>
      <div class="card">
        <h3>Яндекс.Диск</h3>
        <p>Облачное хранилище для файлов. Синхронизация между устройствами и резервные копии.</p>
        <div class="actions">
          <a class="primary" href="https://disk.yandex.ru/" target="_blank" rel="noopener">Официальный сайт</a>
          <a href="#">Поддержка</a>
        </div>
      </div>
      <div class="card">
        <h3>Яндекс.Браузер с VPN</h3>
        <p>Версия браузера с включенным VPN для приватного просмотра и обхода геоблокировок.</p>
        <div class="actions">
          <a class="primary" href="https://browser.yandex.ru/features/vpn/" target="_blank" rel="noopener">Официальная страница</a>
          <a href="#">Как включить VPN</a>
        </div>
      </div>
    </main>

    <footer>
      © 2025 Софт. GitHub Pages.
    </footer>
  </div>
</body>
</html>
