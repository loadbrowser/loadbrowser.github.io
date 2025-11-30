<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Новости Яндекс.Браузера</title>
<style>
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: #f5f7fa;
    margin: 0;
    padding: 0;
    color: #222;
  }

  h1 {
    text-align: center;
    margin-top: 40px;
    font-size: 2rem;
    color: #1a73e8;
  }

  .container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 20px;
    max-width: 1200px;
    margin: 40px auto;
    padding: 0 20px;
  }

  .news-card {
    background: #fff;
    border-radius: 12px;
    padding: 20px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.08);
    transition: transform 0.3s, box-shadow 0.3s;
    display: flex;
    flex-direction: column;
  }

  .news-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 25px rgba(0,0,0,0.15);
  }

  .news-title {
    background: linear-gradient(90deg, #1a73e8, #4285f4);
    color: #fff;
    padding: 10px 15px;
    border-radius: 8px;
    font-size: 1.2rem;
    margin-bottom: 15px;
    display: flex;
    align-items: center;
  }

  .news-title::before {
    content: "📰";
    margin-right: 10px;
    font-size: 1.2rem;
  }

  .news-card ul {
    list-style: none;
    padding-left: 0;
    margin: 0;
    flex-grow: 1;
  }

  .news-card ul li {
    margin-bottom: 10px;
    position: relative;
    padding-left: 15px;
    transition: color 0.2s;
    cursor: pointer;
  }

  .news-card ul li::before {
    content: "•";
    position: absolute;
    left: 0;
    color: #1a73e8;
    font-weight: bold;
  }

  .news-card ul li:hover {
    color: #1a73e8;
  }

  @media (max-width: 500px) {
    .news-title {
      font-size: 1rem;
    }
    .news-card {
      padding: 15px;
    }
  }
</style>
</head>
<body>

<h1>Новости Яндекс.Браузера</h1>

<div class="container">
  <div class="news-card">
    <h3 class="news-title">Скачивание и установка</h3>
    <ul>
      <li>Скачать Яндекс.Браузер</li>
      <li>Установить Яндекс.Браузер</li>
      <li>Яндекс.Браузер бесплатно</li>
      <li>Скачать на телефон</li>
      <li>Официальный Яндекс.Браузер</li>
    </ul>
  </div>

  <div class="news-card">
    <h3 class="news-title">Обновление и версии</h3>
    <ul>
      <li>Версия Яндекс.Браузера</li>
      <li>Последняя версия 2025</li>
      <li>Обновить Яндекс.Браузер</li>
      <li>32/64 бит</li>
      <li>Новинки и функции</li>
    </ul>
  </div>

  <div class="news-card">
    <h3 class="news-title">Расширения и VPN</h3>
    <ul>
      <li>Расширения и плагины</li>
      <li>Adblock для Яндекс.Браузера</li>
      <li>Ublock Origin</li>
      <li>VPN для безопасного серфинга</li>
      <li>Browsec, Planet VPN, AdGuard VPN, VPNly</li>
    </ul>
  </div>

  <div class="news-card">
    <h3 class="news-title">Советы и инструкции</h3>
    <ul>
      <li>Как ускорить браузер</li>
      <li>Настройки безопасности</li>
      <li>Секреты Яндекс.Браузера</li>
      <li>Трюки для удобного использования</li>
      <li>FAQ и поддержка</li>
    </ul>
  </div>
</div>

</body>
</html>
