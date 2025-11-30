<html lang="ru">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Яндекс Софт</title>
  <meta name="description" content="Скачайте Яндекс.Браузер, Яндекс.Диск и Яндекс.Браузер с VPN. Стиль Яндекс.Браузера.">
  <style>
    :root {
      --bg: #f8f9fa;
      --primary: #ff4500;
      --secondary: #ffffff;
      --text: #1c1c1c;
      --muted: #6b7280;
      --radius: 12px;
      --shadow: 0 6px 18px rgba(0,0,0,0.08);
      --maxw: 1200px;
      font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }
    body { background: var(--bg); color: var(--text); display: flex; justify-content: center; font-size: 16px; line-height: 1.5; }
    .wrap { max-width: var(--maxw); width: 100%; padding: 40px 20px; }

    /* Header */
    header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 50px; flex-wrap: wrap; }
    .logo { font-weight: bold; font-size: 26px; color: var(--primary); }
    nav a { text-decoration: none; color: #fff; background: var(--primary); padding: 12px 24px; border-radius: var(--radius); font-weight: 600; white-space: nowrap; transition: background 0.3s; }
    nav a:hover { background: #e03e00; }

    /* Hero */
    .hero { background: var(--secondary); border-radius: var(--radius); box-shadow: var(--shadow); display: flex; gap: 30px; padding: 50px; margin-bottom: 50px; flex-wrap: wrap; align-items: center; }
    .hero-text { flex: 1; min-width: 300px; }
    .hero-text h1 { font-size: 34px; margin-bottom: 16px; color: var(--text); }
    .hero-text p { color: var(--muted); margin-bottom: 24px; font-size: 16px; }
    .hero-text a { text-decoration: none; color: #fff; background: var(--primary); padding: 14px 28px; border-radius: var(--radius); font-weight: 600; white-space: nowrap; transition: background 0.3s; }
    .hero-text a:hover { background: #e03e00; }

    /* Apps Grid */
    .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 25px; margin-bottom: 50px; }
    .card { background: var(--secondary); border-radius: var(--radius); box-shadow: var(--shadow); padding: 30px; display: flex; flex-direction: column; gap: 15px; transition: transform 0.3s, box-shadow 0.3s; }
    .card:hover { transform: translateY(-6px); box-shadow: 0 10px 25px rgba(0,0,0,0.12); }
    .card h3 { font-size: 22px; margin-bottom: 10px; color: var(--text); }
    .card p { color: var(--muted); font-size: 15px; flex: 1; }
    .card .actions { display: flex; gap: 12px; margin-top: 15px; flex-wrap: wrap; }
    .card .actions a { text-decoration: none; padding: 12px 20px; border-radius: var(--radius); font-weight: 600; border: 1px solid rgba(0,0,0,0.1); white-space: nowrap; transition: background 0.3s, color 0.3s; }
    .card .actions a.primary { background: var(--primary); color: #fff; border: none; }
    .card .actions a.primary:hover { background: #e03e00; }
    .card .actions a:hover { opacity: 0.9; }

    /* Footer */
    footer { text-align: center; color: var(--muted); font-size: 14px; padding: 25px 0; }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="logo">Яндекс Софт</div>
      <nav>
        <a href="#apps">Загрузки</a>
      </nav>
    </header>

    <section class="hero">
      <div class="hero-text">
        <h1>Скачайте приложения Яндекс</h1>
        <p>Яндекс.Браузер, Яндекс.Диск и Яндекс.Браузер с VPN. Стиль Яндекс, удобство и безопасность.</p>
        <a href="#apps">Скачать</a>
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
      © 2025 Яндекс Софт. GitHub Pages.
    </footer>
  </div>
</body>
</html>
