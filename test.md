<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Яндекс.Браузер — Новости и Скачивание</title>
<style>
  body {
    margin: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: #f5f7fa;
    color: #222;
  }

  /* Хедер */
  header {
    background: #1a73e8;
    color: #fff;
    padding: 15px 20px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    position: sticky;
    top: 0;
    z-index: 1000;
  }

  header .logo {
    font-size: 1.5rem;
    font-weight: bold;
  }

  header nav a {
    color: #fff;
    text-decoration: none;
    margin-left: 20px;
    font-weight: 500;
    transition: color 0.3s;
  }

  header nav a:hover {
    color: #ffd700;
  }

  /* Hero блок */
  .hero {
    background: linear-gradient(90deg, #4285f4, #1a73e8);
    color: #fff;
    padding: 100px 20px 60px;
    text-align: center;
  }

  .hero h1 {
    font-size: 3rem;
    margin: 0 0 20px;
  }

  .hero p {
    font-size: 1.2rem;
    max-width: 700px;
    margin: 0 auto 30px;
  }

  .hero a {
    background: #ffd700;
    color: #222;
    padding: 12px 25px;
    text-decoration: none;
    border-radius: 8px;
    font-weight: bold;
    transition: background 0.3s;
  }

  .hero a:hover {
    background: #ffc107;
  }

  /* Контентные блоки */
  .container {
    max-width: 1200px;
    margin: 40px auto;
    padding: 0 20px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 20px;
  }

  .card {
    background: #fff;
    border-radius: 12px;
    padding: 20px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.08);
    transition: transform 0.3s, box-shadow 0.3s;
    cursor: pointer;
  }

  .card:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 25px rgba(0,0,0,0.15);
  }

  .card h3 {
    margin-top: 0;
    font-size: 1.3rem;
    color: #1a73e8;
    margin-bottom: 15px;
  }

  .card ul {
    list-style: none;
    padding-left: 0;
  }

  .card ul li {
    margin-bottom: 10px;
    position: relative;
    padding-left: 15px;
    transition: color 0.2s;
  }

  .card ul li::before {
    content: "•";
    position: absolute;
    left: 0;
    color: #1a73e8;
    font-weight: bold;
  }

  .card ul li:hover {
    color: #1a73e8;
  }

  /* Попап */
  .popup-overlay {
    position: fixed;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background: rgba(0,0,0,0.6);
    display: none;
    justify-content: center;
    align-items: center;
    z-index: 2000;
  }

  .popup-content {
    background: #fff;
    padding: 30px;
    border-radius: 12px;
    max-width: 500px;
    width: 90%;
    position: relative;
    text-align: left;
  }

  .popup-content h2 {
    margin-top: 0;
    color: #1a73e8;
  }

  .popup-close {
    position: absolute;
    top: 10px;
    right: 15px;
    font-size: 1.5rem;
    cursor: pointer;
    color: #888;
  }

  .popup-close:hover {
    color: #1a73e8;
  }

  /* Футер */
  footer {
    background: #1a73e8;
    color: #fff;
    padding: 40px 20px;
    text-align: center;
  }

  footer a {
    color: #ffd700;
    text-decoration: none;
    margin: 0 10px;
  }

  footer a:hover {
    text-decoration: underline;
  }

  @media (max-width: 500px) {
    .hero h1 {
      font-size: 2rem;
    }

    .hero p {
      font-size: 1rem;
    }
  }
</style>
</head>
<body>

<header>
  <div class="logo">Яндекс.Браузер</div>
  <nav>
    <a href="#download">Скачать</a>
    <a href="#news">Новости</a>
    <a href="#extensions">Расширения</a>
    <a href="#support">Поддержка</a>
  </nav>
</header>

<section class="hero">
  <h1>Яндекс.Браузер — Быстрый, безопасный, удобный</h1>
  <p>Скачайте последнюю версию Яндекс.Браузера для ПК и мобильных устройств. Наслаждайтесь безопасным веб-серфингом с расширениями и встроенным VPN.</p>
  <a href="#download">Скачать бесплатно</a>
</section>

<section class="container" id="news">
  <div class="card" data-popup="popup1">
    <h3>Скачивание и установка</h3>
    <ul>
      <li>Скачать Яндекс.Браузер</li>
      <li>Установить на ПК</li>
      <li>Версия для телефона</li>
      <li>Бесплатная установка</li>
    </ul>
  </div>

  <div class="card" data-popup="popup2">
    <h3>Обновления и версии</h3>
    <ul>
      <li>Последняя версия 2025</li>
      <li>32/64 бит</li>
      <li>Обновление через браузер</li>
      <li>Новинки и функции</li>
    </ul>
  </div>

  <div class="card" data-popup="popup3">
    <h3>Расширения и VPN</h3>
    <ul>
      <li>Adblock и блокировщики</li>
      <li>VPN для безопасности</li>
      <li>Ublock Origin, Browsec</li>
      <li>Дополнительные плагины</li>
    </ul>
  </div>

  <div class="card" data-popup="popup4">
    <h3>Советы и инструкции</h3>
    <ul>
      <li>Секреты Яндекс.Браузера</li>
      <li>Ускорение работы</li>
      <li>Настройки безопасности</li>
      <li>FAQ и поддержка</li>
    </ul>
  </div>
</section>

<!-- Попапы -->
<div class="popup-overlay" id="popup1">
  <div class="popup-content">
    <span class="popup-close">&times;</span>
    <h2>Скачивание и установка</h2>
    <p>Здесь вы можете скачать Яндекс.Браузер для ПК или мобильного устройства. Установка проста и бесплатна, подходит для Windows, MacOS, Android и iOS.</p>
  </div>
</div>

<div class="popup-overlay" id="popup2">
  <div class="popup-content">
    <span class="popup-close">&times;</span>
    <h2>Обновления и версии</h2>
    <p>Последняя версия Яндекс.Браузера включает новые функции и улучшения безопасности. Обновления доступны через браузер автоматически.</p>
  </div>
</div>

<div class="popup-overlay" id="popup3">
  <div class="popup-content">
    <span class="popup-close">&times;</span>
    <h2>Расширения и VPN</h2>
    <p>Вы можете добавить расширения для блокировки рекламы, VPN для безопасности и другие полезные плагины, чтобы улучшить работу браузера.</p>
  </div>
</div>

<div class="popup-overlay" id="popup4">
  <div class="popup-content">
    <span class="popup-close">&times;</span>
    <h2>Советы и инструкции</h2>
    <p>Изучите советы по настройке Яндекс.Браузера, ускорению работы и обеспечению безопасности, а также получите ответы на часто задаваемые вопросы.</p>
  </div>
</div>

<footer>
  <p>© 2025 Яндекс.Браузер. Все права защищены.</p>
  <p>
    <a href="#">Политика конфиденциальности</a> |
    <a href="#">Пользовательское соглашение</a> |
    <a href="#">Контакты</a>
  </p>
</footer>

<script>
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

  popups.forEach(popup => {
    popup.addEventListener('click', e => {
      if(e.target === popup) popup.style.display = 'none';
    });
  });
</script>

</body>
</html>
