<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LoadBrowser - Загрузчик для браузерных игр</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #2e7d32;
            --primary-dark: #1b5e20;
            --secondary-color: #0288d1;
            --accent-color: #ff9800;
            --light-color: #f5f5f5;
            --dark-color: #212121;
            --gray-color: #757575;
            --light-gray: #e0e0e0;
            --success-color: #4caf50;
            --warning-color: #ff9800;
            --border-radius: 10px;
            --box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--dark-color);
            background-color: #f9f9f9;
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.08);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary-color);
            text-decoration: none;
        }

        .logo i {
            color: var(--secondary-color);
        }

        .logo-text {
            display: flex;
            flex-direction: column;
            line-height: 1.2;
        }

        .logo-subtitle {
            font-size: 0.8rem;
            color: var(--gray-color);
            font-weight: 400;
        }

        .nav-links {
            display: flex;
            gap: 25px;
        }

        .nav-links a {
            color: var(--dark-color);
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
            position: relative;
        }

        .nav-links a:hover {
            color: var(--primary-color);
        }

        .nav-links a.active {
            color: var(--primary-color);
        }

        .nav-links a.active::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 100%;
            height: 2px;
            background-color: var(--primary-color);
        }

        .header-actions {
            display: flex;
            gap: 15px;
            align-items: center;
        }

        .download-btn {
            padding: 10px 24px;
            border-radius: var(--border-radius);
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            border: none;
            font-size: 1rem;
            background-color: var(--primary-color);
            color: white;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .download-btn:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--dark-color);
            cursor: pointer;
        }

        /* Hero Section */
        .hero {
            padding: 80px 0;
            background: linear-gradient(135deg, #e8f5e9 0%, #f1f8e9 100%);
            position: relative;
            overflow: hidden;
        }

        .hero-content {
            display: flex;
            align-items: center;
            gap: 60px;
        }

        .hero-text {
            flex: 1;
        }

        .hero-text h1 {
            font-size: 2.8rem;
            line-height: 1.1;
            margin-bottom: 20px;
            color: var(--dark-color);
        }

        .hero-text h1 span {
            color: var(--primary-color);
        }

        .hero-text p {
            font-size: 1.1rem;
            color: var(--gray-color);
            margin-bottom: 30px;
            max-width: 600px;
        }

        .hero-image {
            flex: 1;
            display: flex;
            justify-content: center;
        }

        .hero-image img {
            max-width: 100%;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
        }

        .features {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 40px;
        }

        .feature {
            display: flex;
            align-items: center;
            gap: 12px;
            background-color: white;
            padding: 15px 20px;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            width: calc(50% - 10px);
        }

        .feature i {
            color: var(--primary-color);
            font-size: 1.5rem;
        }

        /* Main Content */
        .main-content {
            padding: 80px 0;
        }

        .section-title {
            margin-bottom: 40px;
        }

        .section-title h2 {
            font-size: 2.2rem;
            color: var(--dark-color);
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .section-title h2 i {
            color: var(--primary-color);
        }

        .section-title p {
            color: var(--gray-color);
            max-width: 700px;
        }

        /* Apps Grid */
        .apps-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }

        .app-card {
            background-color: white;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
            border: 1px solid var(--light-gray);
        }

        .app-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }

        .app-header {
            padding: 20px;
            background-color: #f5f5f5;
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .app-icon {
            width: 60px;
            height: 60px;
            border-radius: 12px;
            background-color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .app-icon i {
            font-size: 2rem;
            color: var(--primary-color);
        }

        .app-info h3 {
            font-size: 1.3rem;
            margin-bottom: 5px;
        }

        .app-info .app-version {
            color: var(--gray-color);
            font-size: 0.9rem;
        }

        .app-body {
            padding: 20px;
        }

        .app-description {
            color: var(--gray-color);
            margin-bottom: 20px;
            font-size: 0.95rem;
        }

        .app-features {
            list-style: none;
            margin-bottom: 25px;
        }

        .app-features li {
            margin-bottom: 8px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .app-features li i {
            color: var(--success-color);
            font-size: 0.9rem;
        }

        .app-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
            background-color: #f9f9f9;
            border-top: 1px solid var(--light-gray);
        }

        .app-actions {
            display: flex;
            gap: 10px;
        }

        .btn {
            padding: 8px 16px;
            border-radius: 6px;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            border: none;
            font-size: 0.9rem;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        .btn-primary {
            background-color: var(--primary-color);
            color: white;
        }

        .btn-primary:hover {
            background-color: var(--primary-dark);
        }

        .btn-secondary {
            background-color: var(--secondary-color);
            color: white;
        }

        .btn-secondary:hover {
            background-color: #0277bd;
        }

        .app-size {
            color: var(--gray-color);
            font-size: 0.9rem;
        }

        /* How to Use */
        .how-to-use {
            padding: 60px 0;
            background-color: #f5f5f5;
        }

        .steps {
            display: flex;
            justify-content: space-between;
            gap: 30px;
            margin-top: 40px;
        }

        .step {
            flex: 1;
            background-color: white;
            border-radius: var(--border-radius);
            padding: 30px;
            text-align: center;
            box-shadow: var(--box-shadow);
            position: relative;
        }

        .step-number {
            width: 50px;
            height: 50px;
            background-color: var(--primary-color);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            font-weight: 700;
            margin: 0 auto 20px;
        }

        .step h3 {
            font-size: 1.3rem;
            margin-bottom: 15px;
        }

        .step p {
            color: var(--gray-color);
        }

        /* FAQ Section */
        .faq {
            padding: 80px 0;
        }

        .faq-item {
            margin-bottom: 15px;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
        }

        .faq-question {
            background-color: white;
            padding: 20px;
            font-weight: 600;
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: var(--transition);
        }

        .faq-question:hover {
            background-color: #f9f9f9;
        }

        .faq-question i {
            transition: var(--transition);
        }

        .faq-answer {
            background-color: white;
            padding: 0 20px;
            max-height: 0;
            overflow: hidden;
            transition: var(--transition);
            border-top: 1px solid #f0f0f0;
        }

        .faq-item.active .faq-answer {
            padding: 20px;
            max-height: 500px;
        }

        .faq-item.active .faq-question i {
            transform: rotate(180deg);
        }

        /* Footer */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 60px 0 30px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 50px;
        }

        .footer-column h3 {
            font-size: 1.3rem;
            margin-bottom: 25px;
            position: relative;
            padding-bottom: 10px;
        }

        .footer-column h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 3px;
            background-color: var(--primary-color);
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 12px;
        }

        .footer-links a {
            color: #b0b7c3;
            text-decoration: none;
            transition: var(--transition);
        }

        .footer-links a:hover {
            color: white;
            padding-left: 5px;
        }

        .footer-bottom {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid #2d3748;
            color: #b0b7c3;
            font-size: 0.9rem;
        }

        /* Responsive Design */
        @media (max-width: 992px) {
            .hero-content {
                flex-direction: column;
                text-align: center;
            }
            
            .hero-text h1 {
                font-size: 2.5rem;
            }
            
            .features {
                justify-content: center;
            }
            
            .feature {
                width: 100%;
            }
            
            .steps {
                flex-direction: column;
            }
        }

        @media (max-width: 768px) {
            .nav-links, .header-actions {
                display: none;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .hero-text h1 {
                font-size: 2.2rem;
            }
            
            .section-title h2 {
                font-size: 1.8rem;
            }
        }

        @media (max-width: 576px) {
            .hero-text h1 {
                font-size: 1.8rem;
            }
            
            .apps-grid {
                grid-template-columns: 1fr;
            }
            
            .app-footer {
                flex-direction: column;
                gap: 15px;
                align-items: flex-start;
            }
            
            .app-actions {
                width: 100%;
                justify-content: space-between;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">
                <i class="fas fa-rocket"></i>
                <div class="logo-text">
                    LoadBrowser
                    <span class="logo-subtitle">Browser Games Loader</span>
                </div>
            </a>
            
            <nav class="nav-links">
                <a href="#" class="active">Главная</a>
                <a href="#apps">Приложения</a>
                <a href="#how-to-use">Как использовать</a>
                <a href="#faq">FAQ</a>
                <a href="#download">Скачать</a>
            </nav>
            
            <div class="header-actions">
                <button class="download-btn">
                    <i class="fas fa-download"></i>
                    Скачать Loader
                </button>
            </div>
            
            <button class="mobile-menu-btn">
                <i class="fas fa-bars"></i>
            </button>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container hero-content">
            <div class="hero-text">
                <h1>LoadBrowser - <span>загрузчик для браузерных игр</span></h1>
                <p>Уникальный инструмент для загрузки и запуска браузерных игр напрямую на вашем компьютере без необходимости использования браузера.</p>
                
                <div class="hero-buttons">
                    <button class="download-btn" style="font-size: 1.1rem; padding: 12px 30px;">
                        <i class="fas fa-download"></i>
                        Скачать LoadBrowser
                    </button>
                </div>
                
                <div class="features">
                    <div class="feature">
                        <i class="fas fa-bolt"></i>
                        <span>Быстрый запуск игр</span>
                    </div>
                    <div class="feature">
                        <i class="fas fa-shield-alt"></i>
                        <span>Безопасность и защита</span>
                    </div>
                    <div class="feature">
                        <i class="fas fa-gamepad"></i>
                        <span>Поддержка множества игр</span>
                    </div>
                    <div class="feature">
                        <i class="fas fa-sync-alt"></i>
                        <span>Автообновления</span>
                    </div>
                </div>
            </div>
            
            <div class="hero-image">
                <img src="https://images.unsplash.com/photo-1511512578047-dfb367046420?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="LoadBrowser интерфейс">
            </div>
        </div>
    </section>

    <!-- Main Content -->
    <section class="main-content" id="apps">
        <div class="container">
            <div class="section-title">
                <h2><i class="fas fa-gamepad"></i> Доступные игры и приложения</h2>
                <p>Список игр и приложений, которые можно загрузить и запустить через LoadBrowser</p>
            </div>
            
            <div class="apps-grid">
                <!-- Steam App -->
                <div class="app-card">
                    <div class="app-header">
                        <div class="app-icon">
                            <i class="fab fa-steam"></i>
                        </div>
                        <div class="app-info">
                            <h3>Steam Browser</h3>
                            <div class="app-version">Версия 2.0</div>
                        </div>
                    </div>
                    <div class="app-body">
                        <p class="app-description">Доступ к магазину Steam и библиотеке игр через оптимизированный браузер.</p>
                        <ul class="app-features">
                            <li><i class="fas fa-check"></i> Доступ к магазину Steam</li>
                            <li><i class="fas fa-check"></i> Управление библиотекой игр</li>
                            <li><i class="fas fa-check"></i> Чат с друзьями</li>
                            <li><i class="fas fa-check"></i> Уведомления о скидках</li>
                        </ul>
                    </div>
                    <div class="app-footer">
                        <div class="app-actions">
                            <button class="btn btn-primary">
                                <i class="fas fa-download"></i> Скачать
                            </button>
                            <button class="btn btn-secondary">
                                <i class="fas fa-info-circle"></i> Подробнее
                            </button>
                        </div>
                        <div class="app-size">~150 MB</div>
                    </div>
                </div>
                
                <!-- Brawl Stars App -->
                <div class="app-card">
                    <div class="app-header">
                        <div class="app-icon">
                            <i class="fas fa-fist-raised"></i>
                        </div>
                        <div class="app-info">
                            <h3>Brawl Stars Browser</h3>
                            <div class="app-version">Версия 1.5</div>
                        </div>
                    </div>
                    <div class="app-body">
                        <p class="app-description">Запускайте Brawl Stars напрямую на компьютере без эмуляторов.</p>
                        <ul class="app-features">
                            <li><i class="fas fa-check"></i> Прямой запуск игры</li>
                            <li><i class="fas fa-check"></i> Поддержка управления с клавиатуры</li>
                            <li><i class="fas fa-check"></i> Стабильное соединение</li>
                            <li><i class="fas fa-check"></i> Автообновления</li>
                        </ul>
                    </div>
                    <div class="app-footer">
                        <div class="app-actions">
                            <button class="btn btn-primary">
                                <i class="fas fa-download"></i> Скачать
                            </button>
                            <button class="btn btn-secondary">
                                <i class="fas fa-info-circle"></i> Подробнее
                            </button>
                        </div>
                        <div class="app-size">~220 MB</div>
                    </div>
                </div>
                
                <!-- Minecraft App -->
                <div class="app-card">
                    <div class="app-header">
                        <div class="app-icon">
                            <i class="fas fa-cube"></i>
                        </div>
                        <div class="app-info">
                            <h3>Minecraft Browser</h3>
                            <div class="app-version">Версия 3.1</div>
                        </div>
                    </div>
                    <div class="app-body">
                        <p class="app-description">Запускайте браузерную версию Minecraft с улучшенной производительностью.</p>
                        <ul class="app-features">
                            <li><i class="fas fa-check"></i> Улучшенная графика</li>
                            <li><i class="fas fa-check"></i> Поддержка модов</li>
                            <li><i class="fas fa-check"></i> Стабильная работа</li>
                            <li><i class="fas fa-check"></i> Быстрая загрузка миров</li>
                        </ul>
                    </div>
                    <div class="app-footer">
                        <div class="app-actions">
                            <button class="btn btn-primary">
                                <i class="fas fa-download"></i> Скачать
                            </button>
                            <button class="btn btn-secondary">
                                <i class="fas fa-info-circle"></i> Подробнее
                            </button>
                        </div>
                        <div class="app-size">~180 MB</div>
                    </div>
                </div>
                
                <!-- WhatsApp App -->
                <div class="app-card">
                    <div class="app-header">
                        <div class="app-icon">
                            <i class="fab fa-whatsapp"></i>
                        </div>
                        <div class="app-info">
                            <h3>WhatsApp Browser</h3>
                            <div class="app-version">Версия 2.2</div>
                        </div>
                    </div>
                    <div class="app-body">
                        <p class="app-description">Используйте WhatsApp на компьютере с расширенными функциями.</p>
                        <ul class="app-features">
                            <li><i class="fas fa-check"></i> Полная функциональность</li>
                            <li><i class="fas fa-check"></i> Уведомления на рабочем столе</li>
                            <li><i class="fas fa-check"></i> Поддержка медиафайлов</li>
                            <li><i class="fas fa-check"></i> Голосовые сообщения</li>
                        </ul>
                    </div>
                    <div class="app-footer">
                        <div class="app-actions">
                            <button class="btn btn-primary">
                                <i class="fas fa-download"></i> Скачать
                            </button>
                            <button class="btn btn-secondary">
                                <i class="fas fa-info-circle"></i> Подробнее
                            </button>
                        </div>
                        <div class="app-size">~120 MB</div>
                    </div>
                </div>
                
                <!-- PUBG App -->
                <div class="app-card">
                    <div class="app-header">
                        <div class="app-icon">
                            <i class="fas fa-crosshairs"></i>
                        </div>
                        <div class="app-info">
                            <h3>PUBG Browser</h3>
                            <div class="app-version">Версия 1.8</div>
                        </div>
                    </div>
                    <div class="app-body">
                        <p class="app-description">Запускайте PUBG напрямую в браузере с оптимизацией под ПК.</p>
                        <ul class="app-features">
                            <li><i class="fas fa-check"></i> Оптимизация под ПК</li>
                            <li><i class="fas fa-check"></i> Поддержка геймпадов</li>
                            <li><i class="fas fa-check"></i> Низкая задержка</li>
                            <li><i class="fas fa-check"></i> Автонастройка графики</li>
                        </ul>
                    </div>
                    <div class="app-footer">
                        <div class="app-actions">
                            <button class="btn btn-primary">
                                <i class="fas fa-download"></i> Скачать
                            </button>
                            <button class="btn btn-secondary">
                                <i class="fas fa-info-circle"></i> Подробнее
                            </button>
                        </div>
                        <div class="app-size">~250 MB</div>
                    </div>
                </div>
                
                <!-- Standoff 2 App -->
                <div class="app-card">
                    <div class="app-header">
                        <div class="app-icon">
                            <i class="fas fa-user-secret"></i>
                        </div>
                        <div class="app-info">
                            <h3>Standoff 2 Browser</h3>
                            <div class="app-version">Версия 1.3</div>
                        </div>
                    </div>
                    <div class="app-body">
                        <p class="app-description">Запускайте Standoff 2 на компьютере с улучшенным управлением.</p>
                        <ul class="app-features">
                            <li><i class="fas fa-check"></i> Настройки управления</li>
                            <li><i class="fas fa-check"></i> Поддержка мыши и клавиатуры</li>
                            <li><i class="fas fa-check"></i> Стабильный FPS</li>
                            <li><i class="fas fa-check"></i> Быстрое подключение</li>
                        </ul>
                    </div>
                    <div class="app-footer">
                        <div class="app-actions">
                            <button class="btn btn-primary">
                                <i class="fas fa-download"></i> Скачать
                            </button>
                            <button class="btn btn-secondary">
                                <i class="fas fa-info-circle"></i> Подробнее
                            </button>
                        </div>
                        <div class="app-size">~200 MB</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- How to Use Section -->
    <section class="how-to-use" id="how-to-use">
        <div class="container">
            <div class="section-title">
                <h2><i class="fas fa-question-circle"></i> Как использовать LoadBrowser</h2>
                <p>Простая инструкция по установке и использованию загрузчика</p>
            </div>
            
            <div class="steps">
                <div class="step">
                    <div class="step-number">1</div>
                    <h3>Скачайте LoadBrowser</h3>
                    <p>Загрузите установщик LoadBrowser с нашего сайта. Файл имеет небольшой размер и устанавливается за несколько минут.</p>
                </div>
                
                <div class="step">
                    <div class="step-number">2</div>
                    <h3>Установите программу</h3>
                    <p>Запустите установщик и следуйте инструкциям на экране. Установка не требует специальных знаний.</p>
                </div>
                
                <div class="step">
                    <div class="step-number">3</div>
                    <h3>Выберите приложение</h3>
                    <p>Откройте LoadBrowser и выберите нужную игру или приложение из доступного списка.</p>
                </div>
                
                <div class="step">
                    <div class="step-number">4</div>
                    <h3>Наслаждайтесь игрой</h3>
                    <p>Загрузите и запустите выбранное приложение. Все игры оптимизированы для запуска на компьютере.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ Section -->
    <section class="faq" id="faq">
        <div class="container">
            <div class="section-title">
                <h2><i class="fas fa-comments"></i> Часто задаваемые вопросы</h2>
                <p>Ответы на самые популярные вопросы о LoadBrowser</p>
            </div>
            
            <div class="faq-list">
                <div class="faq-item">
                    <div class="faq-question">
                        <span>LoadBrowser безопасен для использования?</span>
                        <i class="fas fa-chevron-down"></i>
                    </div>
                    <div class="faq-answer">
                        <p>Да, LoadBrowser полностью безопасен. Все приложения проверяются на наличие вредоносного кода перед добавлением в каталог. Мы не собираем и не передаем личные данные пользователей.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question">
                        <span>Требуется ли для работы стабильное интернет-соединение?</span>
                        <i class="fas fa-chevron-down"></i>
                    </div>
                    <div class="faq-answer">
                        <p>Да, для загрузки приложений и игр требуется подключение к интернету. После загрузки некоторые игры могут работать в офлайн-режиме, но для многопользовательских игр необходимо стабильное соединение.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question">
                        <span>Какие системные требования у LoadBrowser?</span>
                        <i class="fas fa-chevron-down"></i>
                    </div>
                    <div class="faq-answer">
                        <p>LoadBrowser работает на Windows 7 и выше, требует не менее 2 ГБ оперативной памяти и 500 МБ свободного места на диске. Для некоторых игр могут потребоваться дополнительные ресурсы.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question">
                        <span>Можно ли предлагать свои игры для добавления в каталог?</span>
                        <i class="fas fa-chevron-down"></i>
                    </div>
                    <div class="faq-answer">
                        <p>Да, мы принимаем предложения по добавлению новых игр и приложений. Вы можете отправить запрос через форму обратной связи или связаться с нами по электронной почте.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question">
                        <span>Бесплатен ли LoadBrowser?</span>
                        <i class="fas fa-chevron-down"></i>
                    </div>
                    <div class="faq-answer">
                        <p>Да, LoadBrowser полностью бесплатен. Мы не берем плату за использование загрузчика. Некоторые игры могут иметь встроенные покупки, но сам LoadBrowser предоставляется бесплатно.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Download Section -->
    <section class="how-to-use" id="download" style="background-color: #e8f5e9;">
        <div class="container">
            <div class="section-title" style="text-align: center;">
                <h2><i class="fas fa-download"></i> Скачайте LoadBrowser сейчас</h2>
                <p>Начните использовать LoadBrowser уже сегодня. Это бесплатно и безопасно!</p>
            </div>
            
            <div style="text-align: center; margin-top: 40px;">
                <button class="download-btn" style="font-size: 1.2rem; padding: 15px 40px;">
                    <i class="fas fa-download"></i>
                    Скачать LoadBrowser v2.1
                </button>
                <p style="margin-top: 20px; color: var(--gray-color);">Размер установщика: ~45 MB</p>
                <p style="margin-top: 10px; color: var(--gray-color);">Поддерживаемые ОС: Windows 7, 8, 10, 11</p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>LoadBrowser</h3>
                    <p>Уникальный загрузчик для браузерных игр, который позволяет запускать игры напрямую на компьютере без использования браузера.</p>
                    <div style="margin-top: 20px; display: flex; gap: 15px;">
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-github"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-telegram"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-discord"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Приложения</h3>
                    <ul class="footer-links">
                        <li><a href="#">Steam Browser</a></li>
                        <li><a href="#">Brawl Stars Browser</a></li>
                        <li><a href="#">Minecraft Browser</a></li>
                        <li><a href="#">WhatsApp Browser</a></li>
                        <li><a href="#">Все приложения</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Помощь</h3>
                    <ul class="footer-links">
                        <li><a href="#">Инструкция по установке</a></li>
                        <li><a href="#">Решение проблем</a></li>
                        <li><a href="#">Системные требования</a></li>
                        <li><a href="#">Обратная связь</a></li>
                        <li><a href="#">Сообщить об ошибке</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Правовая информация</h3>
                    <ul class="footer-links">
                        <li><a href="#">Условия использования</a></li>
                        <li><a href="#">Политика конфиденциальности</a></li>
                        <li><a href="#">Отказ от ответственности</a></li>
                        <li><a href="#">Лицензионное соглашение</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2023 LoadBrowser. Все права защищены. LoadBrowser не аффилирован с компаниями, чьи игры представлены в каталоге.</p>
                <p style="margin-top: 10px;">Все игры являются собственностью их соответствующих правообладателей.</p>
            </div>
        </div>
    </footer>

    <script>
        // Мобильное меню
        const mobileMenuBtn = document.querySelector('.mobile-menu-btn');
        const navLinks = document.querySelector('.nav-links');
        const headerActions = document.querySelector('.header-actions');
        
        mobileMenuBtn.addEventListener('click', () => {
            if (navLinks.style.display === 'flex') {
                navLinks.style.display = 'none';
                headerActions.style.display = 'none';
            } else {
                navLinks.style.display = 'flex';
                headerActions.style.display = 'flex';
                navLinks.style.flexDirection = 'column';
                navLinks.style.position = 'absolute';
                navLinks.style.top = '100%';
                navLinks.style.left = '0';
                navLinks.style.right = '0';
                navLinks.style.backgroundColor = 'white';
                navLinks.style.padding = '20px';
                navLinks.style.boxShadow = '0 10px 20px rgba(0,0,0,0.1)';
                navLinks.style.gap = '15px';
                
                headerActions.style.flexDirection = 'column';
                headerActions.style.position = 'absolute';
                headerActions.style.top = 'calc(100% + 180px)';
                headerActions.style.left = '0';
                headerActions.style.right = '0';
                headerActions.style.backgroundColor = 'white';
                headerActions.style.padding = '20px';
                headerActions.style.boxShadow = '0 10px 20px rgba(0,0,0,0.1)';
            }
        });
        
        // FAQ аккордеон
        const faqItems = document.querySelectorAll('.faq-item');
        
        faqItems.forEach(item => {
            const question = item.querySelector('.faq-question');
            question.addEventListener('click', () => {
                // Закрываем все открытые элементы
                faqItems.forEach(otherItem => {
                    if (otherItem !== item && otherItem.classList.contains('active')) {
                        otherItem.classList.remove('active');
                    }
                });
                
                // Переключаем текущий элемент
                item.classList.toggle('active');
            });
        });
        
        // Плавная прокрутка
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Закрытие мобильного меню
                    if(window.innerWidth <= 768) {
                        navLinks.style.display = 'none';
                        headerActions.style.display = 'none';
                    }
                }
            });
        });
        
        // Анимация карточек при прокрутке
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if(entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);
        
        // Применяем анимацию к карточкам
        document.querySelectorAll('.app-card, .step').forEach(card => {
            card.style.opacity = '0';
            card.style.transform = 'translateY(20px)';
            card.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            observer.observe(card);
        });
        
        // Обновление года в футере
        document.querySelector('.footer-bottom p').innerHTML = `&copy; ${new Date().getFullYear()} LoadBrowser. Все права защищены. LoadBrowser не аффилирован с компаниями, чьи игры представлены в каталоге.`;
        
        // Кнопки скачивания
        document.querySelectorAll('.btn-primary').forEach(btn => {
            btn.addEventListener('click', function() {
                const appName = this.closest('.app-card').querySelector('h3').textContent;
                alert(`Начата загрузка: ${appName}\n\nЗагрузка начнется через несколько секунд. Если загрузка не началась автоматически, проверьте настройки браузера.`);
            });
        });
        
        // Кнопка скачивания главного загрузчика
        document.querySelector('.download-btn').addEventListener('click', function() {
            alert('Начата загрузка LoadBrowser v2.1\n\nРазмер файла: ~45 MB\nЗагрузка начнется через несколько секунд.');
        });
    </script>
</body>
</html>
