<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Яндекс Софт</title>
  <meta name="description" content="Скачайте Яндекс.Браузер, Яндекс.Диск и Яндекс.Браузер с VPN. Стиль Яндекс.Браузера.">
  <style>
    :root {
      --bg: #f8f9fa;
      --primary: #333333;
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
    .wrap { max-width: var(--maxw); width: 100%; padding: 0 20px; }

    header { display: flex; justify-content: space-between; align-items: center; padding: 25px 0; flex-wrap: wrap; }
    .logo { font-weight: bold; font-size: 28px; color: var(--primary); }
    nav a { text-decoration: none; color: #fff; background: var(--primary); padding: 12px 28px; border-radius: var(--radius); font-weight: 600; white-space: nowrap; transition: background 0.3s; }
    nav a:hover { background: #555; }

    .hero { background: linear-gradient(135deg, #f0f0f0, #e0e0e0); border-radius: var(--radius); box-shadow: 0 10px 30px rgba(0,0,0,0.15); display: flex; gap: 30px; padding: 60px 40px; margin-bottom: 50px; flex-wrap: wrap; align-items: center; border: 1px solid #ddd; }
    .hero-text { flex: 1; min-width: 300px; }
    .hero-text h1 { font-size: 36px; margin-bottom: 18px; color: var(--primary); font-weight: 700; }
    .hero-text p { color: var(--muted); margin-bottom: 28px; font-size: 17px; }
    .hero-text a { text-decoration: none; color: #fff; background: #555; padding: 14px 30px; border-radius: var(--radius); font-weight: 600; white-space: nowrap; transition: background 0.3s; cursor: pointer; }
    .hero-text a:hover { background: #333; }

    .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 25px; margin-bottom: 50px; }
    .card { background: var(--secondary); border-radius: var(--radius); box-shadow: var(--shadow); padding: 30px; display: flex; flex-direction: column; gap: 15px; transition: transform 0.3s, box-shadow 0.3s; }
    .card:hover { transform: translateY(-6px); box-shadow: 0 12px 28px rgba(0,0,0,0.12); }
    .card h3 { font-size: 22px; margin-bottom: 10px; color: var(--primary); }
    .card p { color: var(--muted); font-size: 15px; flex: 1; }
    .card .actions { display: flex; gap: 12px; margin-top: 15px; flex-wrap: wrap; }
    .card .actions a { text-decoration: none; padding: 12px 20px; border-radius: var(--radius); font-weight: 600; border: 1px solid rgba(0,0,0,0.1); white-space: nowrap; transition: background 0.3s, color 0.3s; cursor: pointer; }
    .card .actions a.primary { background: #555; color: #fff; border: none; }
    .card .actions a.primary:hover { background: #333; }
    .card .actions a:hover { opacity: 0.9; }

    h2.section-title { font-size: 28px; margin: 50px 0 25px 0; text-align: center; color: var(--primary); }

    footer { text-align: center; color: var(--muted); font-size: 14px; padding: 25px 0; }

    .modal { display: none; position: fixed; z-index: 1000; left: 0; top: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.6); justify-content: center; align-items: center; }
    .modal.active { display: flex; }
    .modal-content { background: var(--secondary); padding: 30px; border-radius: var(--radius); max-width: 400px; width: 90%; text-align: center; box-shadow: var(--shadow); animation: fadeIn 0.3s; }
    .modal-content h2 { margin-bottom: 15px; color: var(--primary); }
    .modal-content p { margin-bottom: 20px; color: var(--muted); }
    .modal-content button { padding: 12px 28px; border-radius: var(--radius); border: none; background: #555; color: #fff; font-weight: 600; cursor: pointer; transition: background 0.3s; }
    .modal-content button:hover { background: #333; }

    @keyframes fadeIn { from { opacity: 0; transform: translateY(-10px); } to { opacity: 1; transform: translateY(0); } }
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
        <p>Яндекс.Браузер, Яндекс.Диск и Яндекс.Браузер с VPN. Более стильный и безопасный софт для всех устройств.</p>
        <a id="openModalHero" data-link="https://browser.yandex.ru/">Скачать</a>
      </div>
    </section>

    <main id="apps" class="grid">
      <div class="card">
        <h3>Яндекс.Браузер</h3>
        <p>Быстрый браузер с защитой от фишинга и встроенными сервисами. Поддержка расширений.</p>
        <div class="actions">
          <a class="primary" data-link="https://browser.yandex.ru/">Скачать</a>
          <a href="#">Инструкция</a>
        </div>
      </div>
      <div class="card">
        <h3>Яндекс.Диск</h3>
        <p>Облачное хранилище для файлов. Синхронизация между устройствами и резервные копии.</p>
        <div class="actions">
          <a class="primary" data-link="https://disk.yandex.ru/">Скачать</a>
          <a href="#">Поддержка</a>
        </div>
      </div>
      <div class="card">
        <h3>Яндекс.Браузер с VPN</h3>
        <p>Версия браузера с включенным VPN для приватного просмотра и обхода геоблокировок.</p>
        <div class="actions">
          <a class="primary" data-link="https://browser.yandex.ru/features/vpn/">Скачать</a>
          <a href="#">Как включить VPN</a>
        </div>
      </div>
    </main>

    <h2 class="section-title">Популярные функции и расширения</h2>
    <div class="grid">
      <div class="card">
        <h3>Расширения и VPN</h3>
        <p>AdBlock, Юбуст, VPN и другие расширения для защиты и удобства работы в браузере.</p>
        <div class="actions">
          <a class="primary" data-link="https://browser.yandex.ru/features/extensions/">Подробнее</a>
        </div>
      </div>
      <div class="card">
        <h3>Очистка кэша и куки</h3>
        <p>Инструменты для удаления кэша, истории и сохраненных данных для ускорения работы.</p>
        <div class="actions">
          <a class="primary" href="#">Инструкция</a>
        </div>
      </div>
      <div class="card">
        <h3>Настройки и вкладки</h3>
        <p>Управление закладками, паролями, вкладками, режим инкогнито и другими параметрами.</p>
        <div class="actions">
          <a class="primary" href="#">Настройка</a>
        </div>
      </div>
      <div class="card">
        <h3>Видео и пересказ</h3>
        <p>Пересказ видео, встроенные функции для просмотра и управления медиа в браузере.</p>
        <div class="actions">
          <a class="primary" href="#">Подробнее</a>
        </div>
      </div>
    </div>

    <h2 class="section-title">FAQ и помощь</h2>
    <div class="grid">
      <div class="card">
        <h3>Восстановление вкладок</h3>
        <p>Как вернуть закрытые вкладки и историю браузера.</p>
        <div class="actions">
          <a class="primary" href="#">Инструкция</a>
        </div>
      </div>
      <div class="card">
        <h3>Сделать браузер основным</h3>
        <p>Инструкция по установке Яндекс.Браузера по умолчанию на устройстве.</p>
        <div class="actions">
          <a class="primary" href="#">Подробнее</a>
        </div>
      </div>
      <div class="card">
        <h3>Обновление браузера</h3>
        <p>Как обновить Яндекс.Браузер до последней версии бесплатно.</p>
        <div class="actions">
          <a class="primary" href="#">Инструкция</a>
        </div>
      </div>
    </div>

    <footer>
      © 2025 Яндекс Софт. GitHub Pages.
    </footer>
  </div>

  <div id="modal" class="modal">
    <div class="modal-content">
      <h2>Скачать приложение</h2>
      <p>Нажмите кнопку ниже, чтобы перейти к загрузке выбранного приложения.</p>
      <button id="modalDownload">Скачать</button>
    </div>
  </div>

  <script>
    const modal = document.getElementById('modal');
    const modalDownload = document.getElementById('modalDownload');
    let downloadLink = '';

    document.querySelectorAll('[data-link]').forEach(btn => {
      btn.addEventListener('click', () => {
        downloadLink = btn.getAttribute('data-link');
        modal.classList.add('active');
      });
    });

    modalDownload.addEventListener('click', () => {
      if(downloadLink) window.open(downloadLink, '_blank');
      modal.classList.remove('active');
    });

    window.addEventListener('click', (e) => {
      if(e.target === modal){
        modal.classList.remove('active');
      }
    });
  </script>
</body>
</html>
