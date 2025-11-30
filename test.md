<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Популярный софт</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f5f7fa;
      color: #222;
    }
    header {
      background-color: #1a73e8;
      color: white;
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    header h1 {
      margin: 0;
      font-size: 28px;
    }
    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      font-weight: bold;
    }
    .hero {
      background-color: #e8f0fe;
      padding: 60px 40px;
      text-align: center;
    }
    .hero h2 {
      font-size: 36px;
      margin-bottom: 20px;
    }
    .hero p {
      font-size: 18px;
      max-width: 600px;
      margin: 0 auto;
    }
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
      gap: 20px;
      padding: 40px;
    }
    .card {
      background: white;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      overflow: hidden;
      cursor: pointer;
      transition: transform 0.2s, box-shadow 0.2s;
    }
    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
    }
    .card img {
      width: 100%;
      display: block;
    }
    .card-body {
      padding: 20px;
    }
    .card-body h3 {
      margin: 0;
      font-size: 18px;
    }
    /* Попап */
    .popup-overlay {
      position: fixed;
      top: 0;
      left: 0;
      right:0;
      bottom:0;
      background: rgba(0,0,0,0.6);
      display: none;
      justify-content: center;
      align-items: center;
      z-index: 1000;
    }
    .popup-content {
      background: white;
      padding: 30px;
      border-radius: 12px;
      max-width: 500px;
      text-align: left;
      position: relative;
    }
    .popup-content h2 {
      margin-top: 0;
      font-size: 22px;
    }
    .popup-content p {
      font-size: 16px;
      line-height: 1.5;
    }
    .popup-close {
      position: absolute;
      top: 10px;
      right: 15px;
      font-size: 24px;
      cursor: pointer;
    }
    footer {
      background: #1a73e8;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Популярный софт</h1>
    <nav>
      <a href="#">Главная</a>
      <a href="#">Скачать</a>
      <a href="#">Контакты</a>
    </nav>
  </header>

  <section class="hero">
    <h2>Лучшие программы для вашего ПК и смартфона</h2>
    <p>Скачивайте актуальные версии популярных браузеров, утилит и приложений для безопасной и комфортной работы на компьютере и мобильных устройствах.</p>
  </section>

  <section class="cards">
    <div class="card" data-popup="popup1">
      <img src="https://via.placeholder.com/400x200.png?text=Яндекс.Браузер" alt="Яндекс.Браузер">
      <div class="card-body">
        <h3>Яндекс.Браузер</h3>
      </div>
    </div>
    <div class="card" data-popup="popup2">
      <img src="https://via.placeholder.com/400x200.png?text=Opera" alt="Opera">
      <div class="card-body">
        <h3>Opera</h3>
      </div>
    </div>
    <div class="card" data-popup="popup3">
      <img src="https://via.placeholder.com/400x200.png?text=Chrome" alt="Chrome">
      <div class="card-body">
        <h3>Google Chrome</h3>
      </div>
    </div>
  </section>

  <!-- Попапы -->
  <div class="popup-overlay" id="popup1">
    <div class="popup-content">
      <span class="popup-close">&times;</span>
      <h2>Яндекс.Браузер</h2>
      <p>Яндекс.Браузер позволяет безопасно и быстро просматривать сайты, поддерживает синхронизацию закладок, паролей и расширений. Автообновление обеспечивает актуальность версий. Подходит для Windows, MacOS, Android и iOS. Встроенные инструменты для защиты от вирусов и рекламы делают работу комфортной и безопасной для всех пользователей.</p>
    </div>
  </div>

  <div class="popup-overlay" id="popup2">
    <div class="popup-content">
      <span class="popup-close">&times;</span>
      <h2>Opera</h2>
      <p>Opera — быстрый браузер с встроенным VPN и блокировкой рекламы. Поддерживает синхронизацию между устройствами, имеет экономный режим трафика и оптимизацию для игр и видео. Подходит для Windows, MacOS, Android и iOS. Простая установка, безопасная работа и возможность настроить интерфейс под себя делают его популярным выбором среди пользователей по всему миру.</p>
    </div>
  </div>

  <div class="popup-overlay" id="popup3">
    <div class="popup-content">
      <span class="popup-close">&times;</span>
      <h2>Google Chrome</h2>
      <p>Google Chrome обеспечивает высокую скорость работы и стабильность, поддерживает множество расширений и синхронизацию с Google-аккаунтом. Подходит для Windows, MacOS, Linux, Android и iOS. Встроенные функции защиты от фишинга и вредоносных сайтов делают его безопасным для работы в интернете, а простой интерфейс позволяет быстро находить нужные функции и управлять настройками браузера.</p>
    </div>
  </div>

  <footer>
    &copy; 2025 Популярный софт. Все права защищены.
  </footer>

  <script>
    // Открытие попапа
    const cards = document.querySelectorAll('.card');
    const popups = document.querySelectorAll('.popup-overlay');
    const closeButtons = document.querySelectorAll('.popup-close');

    cards.forEach(card => {
      card.addEventListener('click', () => {
        const popupId = card.getAttribute('data-popup');
        document.getElementById(popupId).style.display = 'flex';
      });
    });

    closeButtons.forEach(btn => {
      btn.addEventListener('click', () => {
        btn.closest('.popup-overlay').style.display = 'none';
      });
    });

    // Закрытие при клике вне контента
    popups.forEach(popup => {
      popup.addEventListener('click', (e) => {
        if(e.target === popup) popup.style.display = 'none';
      });
    });
  </script>
</body>
</html>
