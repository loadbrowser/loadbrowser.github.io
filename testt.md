<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Яндекс.Браузер - Загрузка и установка</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #FF2E2E;
            --primary-dark: #CC0000;
            --secondary-color: #FFCC00;
            --accent-color: #3366FF;
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

        /* Breadcrumbs */
        .breadcrumbs {
            padding: 20px 0;
            background-color: #f5f5f5;
            border-bottom: 1px solid var(--light-gray);
        }

        .breadcrumbs-container {
            display: flex;
            align-items: center;
            gap: 10px;
            flex-wrap: wrap;
        }

        .breadcrumbs a {
            color: var(--gray-color);
            text-decoration: none;
            transition: var(--transition);
        }

        .breadcrumbs a:hover {
            color: var(--primary-color);
        }

        .breadcrumbs span {
            color: var(--dark-color);
            font-weight: 500;
        }

        .breadcrumbs i {
            font-size: 0.8rem;
            color: var(--gray-color);
        }

        /* App Detail Header */
        .app-detail-header {
            padding: 40px 0;
            background: linear-gradient(135deg, #FFF5F5 0%, #FFEBEE 100%);
        }

        .app-header-content {
            display: flex;
            align-items: center;
            gap: 40px;
        }

        .app-icon-large {
            width: 120px;
            height: 120px;
            border-radius: 20px;
            background: linear-gradient(135deg, #FF2E2E, #FF6666);
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: var(--box-shadow);
            position: relative;
            overflow: hidden;
        }

        .app-icon-large::before {
            content: 'Я';
            font-size: 4rem;
            font-weight: 700;
            color: white;
            font-family: 'Arial', sans-serif;
        }

        .app-header-info {
            flex: 1;
        }

        .app-title {
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: var(--dark-color);
        }

        .app-title span {
            color: var(--primary-color);
        }

        .app-meta {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }

        .app-version {
            background-color: var(--primary-color);
            color: white;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 600;
        }

        .app-rating {
            display: flex;
            align-items: center;
            gap: 5px;
            color: var(--warning-color);
        }

        .app-size {
            color: var(--gray-color);
            font-weight: 500;
        }

        .app-header-actions {
            display: flex;
            gap: 15px;
            margin-top: 25px;
            flex-wrap: wrap;
        }

        .btn {
            padding: 12px 24px;
            border-radius: var(--border-radius);
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            border: none;
            font-size: 1rem;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .btn-primary {
            background-color: var(--primary-color);
            color: white;
        }

        .btn-primary:hover {
            background-color: var(--primary-dark);
        }

        .btn-secondary {
            background-color: white;
            color: var(--primary-color);
            border: 2px solid var(--primary-color);
        }

        .btn-secondary:hover {
            background-color: #f5f5f5;
        }

        .btn-accent {
            background-color: var(--accent-color);
            color: white;
        }

        .btn-accent:hover {
            background-color: #2952CC;
        }

        /* Main Content */
        .main-content {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 40px;
            padding: 40px 0;
        }

        /* App Details */
        .app-details {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 30px;
            box-shadow: var(--box-shadow);
        }

        .section-title {
            font-size: 1.5rem;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--light-gray);
            color: var(--dark-color);
        }

        .app-description {
            margin-bottom: 30px;
            line-height: 1.8;
            color: var(--gray-color);
        }

        .highlight {
            background-color: #FFF5F5;
            border-left: 4px solid var(--primary-color);
            padding: 20px;
            border-radius: 0 var(--border-radius) var(--border-radius) 0;
            margin: 25px 0;
        }

        .app-features {
            margin-bottom: 40px;
        }

        .app-features ul {
            list-style: none;
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
        }

        .app-features li {
            display: flex;
            align-items: center;
            gap: 10px;
            padding: 10px;
            background-color: #f9f9f9;
            border-radius: 8px;
        }

        .app-features li i {
            color: var(--success-color);
        }

        /* System Requirements */
        .system-requirements {
            margin-bottom: 40px;
        }

        .requirements-table {
            width: 100%;
            border-collapse: collapse;
        }

        .requirements-table th, .requirements-table td {
            padding: 12px 15px;
            text-align: left;
            border-bottom: 1px solid var(--light-gray);
        }

        .requirements-table th {
            background-color: #f5f5f5;
            font-weight: 600;
        }

        .requirements-table tr:last-child td {
            border-bottom: none;
        }

        /* Screenshots */
        .app-screenshots {
            margin-bottom: 40px;
        }

        .screenshots-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
        }

        .screenshot {
            border-radius: 8px;
            overflow: hidden;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
        }

        .screenshot:hover {
            transform: scale(1.03);
        }

        .screenshot img {
            width: 100%;
            height: 150px;
            object-fit: cover;
            display: block;
        }

        /* Sidebar */
        .sidebar {
            display: flex;
            flex-direction: column;
            gap: 30px;
        }

        /* Related Apps */
        .related-apps {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 25px;
            box-shadow: var(--box-shadow);
        }

        .related-apps-list {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .related-app {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 15px;
            border-radius: 8px;
            background-color: #f9f9f9;
            transition: var(--transition);
            text-decoration: none;
            color: var(--dark-color);
        }

        .related-app:hover {
            background-color: #FFF5F5;
            transform: translateX(5px);
        }

        .related-app-icon {
            width: 50px;
            height: 50px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .related-app-icon i {
            color: white;
            font-size: 1.5rem;
        }

        .related-app-info h4 {
            margin-bottom: 5px;
        }

        .related-app-info p {
            font-size: 0.9rem;
            color: var(--gray-color);
        }

        /* Download Info */
        .download-info {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 25px;
            box-shadow: var(--box-shadow);
        }

        .download-info-item {
            margin-bottom: 20px;
            padding-bottom: 20px;
            border-bottom: 1px solid var(--light-gray);
        }

        .download-info-item:last-child {
            margin-bottom: 0;
            padding-bottom: 0;
            border-bottom: none;
        }

        .download-info-item h4 {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .download-info-item h4 i {
            color: var(--primary-color);
        }

        /* Comparison Table */
        .comparison-section {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 30px;
            margin-top: 40px;
            box-shadow: var(--box-shadow);
        }

        .comparison-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }

        .comparison-table th, .comparison-table td {
            padding: 15px;
            text-align: left;
            border-bottom: 1px solid var(--light-gray);
        }

        .comparison-table th {
            background-color: #f5f5f5;
            font-weight: 600;
            width: 30%;
        }

        .comparison-table .feature-name {
            font-weight: 600;
            color: var(--dark-color);
        }

        .comparison-table .yandex-check {
            color: var(--success-color);
            font-weight: bold;
        }

        .comparison-table .other-check {
            color: var(--gray-color);
        }

        /* How to Install */
        .how-to-install {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 30px;
            margin-top: 40px;
            box-shadow: var(--box-shadow);
        }

        .install-steps {
            display: flex;
            flex-direction: column;
            gap: 30px;
        }

        .install-step {
            display: flex;
            gap: 20px;
        }

        .step-number {
            width: 40px;
            height: 40px;
            background-color: var(--primary-color);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 700;
            flex-shrink: 0;
        }

        .step-content h4 {
            margin-bottom: 10px;
        }

        .step-content p {
            color: var(--gray-color);
        }

        /* Comments Section */
        .comments-section {
            margin-top: 40px;
            background-color: white;
            border-radius: var(--border-radius);
            padding: 30px;
            box-shadow: var(--box-shadow);
        }

        .comment-form {
            margin-bottom: 40px;
        }

        .comment-form textarea {
            width: 100%;
            padding: 15px;
            border-radius: 8px;
            border: 1px solid var(--light-gray);
            resize: vertical;
            min-height: 100px;
            font-family: inherit;
            margin-bottom: 15px;
        }

        .comment-form button {
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 12px 24px;
            border-radius: 8px;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
        }

        .comment-form button:hover {
            background-color: var(--primary-dark);
        }

        .comment {
            display: flex;
            gap: 15px;
            padding: 20px 0;
            border-bottom: 1px solid var(--light-gray);
        }

        .comment:last-child {
            border-bottom: none;
        }

        .comment-avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: #e0e0e0;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
        }

        .comment-avatar i {
            font-size: 1.5rem;
            color: var(--gray-color);
        }

        .comment-content h4 {
            margin-bottom: 5px;
        }

        .comment-date {
            font-size: 0.9rem;
            color: var(--gray-color);
            margin-bottom: 10px;
        }

        /* Footer */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 60px 0 30px;
            margin-top: 60px;
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
            .main-content {
                grid-template-columns: 1fr;
            }
            
            .app-features ul {
                grid-template-columns: 1fr;
            }
            
            .screenshots-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 768px) {
            .nav-links, .header-actions {
                display: none;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .app-header-content {
                flex-direction: column;
                text-align: center;
            }
            
            .app-title {
                font-size: 2rem;
            }
            
            .app-meta {
                justify-content: center;
            }
            
            .screenshots-grid {
                grid-template-columns: 1fr;
            }
            
            .comparison-table {
                display: block;
                overflow-x: auto;
            }
        }

        @media (max-width: 576px) {
            .app-header-actions {
                flex-direction: column;
            }
            
            .btn {
                width: 100%;
                justify-content: center;
            }
            
            .app-icon-large {
                width: 100px;
                height: 100px;
            }
            
            .app-icon-large::before {
                font-size: 3rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="index.html" class="logo">
                <i class="fas fa-download"></i>
                <div class="logo-text">
                    Загрузки
                    <span class="logo-subtitle">Безопасные программы</span>
                </div>
            </a>
            
            <nav class="nav-links">
                <a href="index.html">Главная</a>
                <a href="browsers.html">Браузеры</a>
                <a href="games.html">Игры</a>
                <a href="software.html">Программы</a>
                <a href="tools.html">Утилиты</a>
            </nav>
            
            <div class="header-actions">
                <button class="download-btn">
                    <i class="fas fa-search"></i>
                    Поиск
                </button>
            </div>
            
            <button class="mobile-menu-btn">
                <i class="fas fa-bars"></i>
            </button>
        </div>
    </header>

    <!-- Breadcrumbs -->
    <section class="breadcrumbs">
        <div class="container breadcrumbs-container">
            <a href="index.html"><i class="fas fa-home"></i> Главная</a>
            <i class="fas fa-chevron-right"></i>
            <a href="browsers.html">Браузеры</a>
            <i class="fas fa-chevron-right"></i>
            <span>Яндекс.Браузер</span>
        </div>
    </section>

    <!-- App Detail Header -->
    <section class="app-detail-header">
        <div class="container">
            <div class="app-header-content">
                <div class="app-icon-large"></div>
                <div class="app-header-info">
                    <h1 class="app-title"><span>Яндекс.Браузер</span> — быстрый и умный браузер</h1>
                    <div class="app-meta">
                        <span class="app-version">Версия 23.11</span>
                        <div class="app-rating">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star-half-alt"></i>
                            <span>4.6 (12,347 оценок)</span>
                        </div>
                        <span class="app-size">Размер: 85.4 MB</span>
                    </div>
                    <p>Быстрый и безопасный браузер от Яндекса с интегрированными сервисами и уникальной технологией Турбо для ускорения загрузки страниц.</p>
                    <div class="app-header-actions">
                        <button class="btn btn-primary" id="download-windows">
                            <i class="fas fa-download"></i> Скачать для Windows
                        </button>
                        <button class="btn btn-accent" id="download-linux">
                            <i class="fab fa-linux"></i> Версия для Linux
                        </button>
                        <button class="btn btn-secondary" id="download-mac">
                            <i class="fab fa-apple"></i> Версия для Mac
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Main Content -->
    <div class="container main-content">
        <!-- Left Column: App Details -->
        <div class="app-details">
            <h2 class="section-title">О Яндекс.Браузере</h2>
            <div class="app-description">
                <p><strong>Яндекс.Браузер</strong> — это современный веб-браузер, разработанный компанией Яндекс на основе движка Chromium с интеграцией сервисов Яндекса. Браузер отличается высокой скоростью работы, встроенной защитой от вредоносных сайтов и уникальными функциями, такими как Турбо-режим, Умная строка и встроенный переводчик.</p>
                
                <div class="highlight">
                    <p><strong>Преимущества Яндекс.Браузера:</strong> Браузер автоматически синхронизирует закладки, историю и пароли между устройствами, поддерживает установку расширений из Chrome Web Store и имеет встроенный блокировщик рекламы. Оптимизирован для работы в российском интернет-пространстве.</p>
                </div>
                
                <p>Яндекс.Браузер предлагает уникальные возможности для пользователей, такие как "Табло" с персонализированными сайтами, режим "Турбо" для экономии трафика и ускорения загрузки, а также глубокую интеграцию с сервисами Яндекс: Поиск, Почта, Карты, Переводчик и другими.</p>
            </div>
            
            <div class="app-features">
                <h2 class="section-title">Ключевые возможности</h2>
                <ul>
                    <li><i class="fas fa-check"></i> <strong>Технология Турбо</strong> — ускорение загрузки страниц при медленном интернете</li>
                    <li><i class="fas fa-check"></i> <strong>Встроенный переводчик</strong> — мгновенный перевод страниц на русский язык</li>
                    <li><i class="fas fa-check"></i> <strong>Защита Active Protect</strong> — блокировка опасных сайтов и файлов</li>
                    <li><i class="fas fa-check"></i> <strong>Умная строка</strong> — поиск, адреса и команды в одной строке</li>
                    <li><i class="fas fa-check"></i> <strong>Режим "Инкогнито"</strong> — приватный просмотр без сохранения истории</li>
                    <li><i class="fas fa-check"></i> <strong>Синхронизация</strong> — закладки, пароли, история на всех устройствах</li>
                    <li><i class="fas fa-check"></i> <strong>Экономия трафика</strong> — сжатие данных до 50% в Турбо-режиме</li>
                    <li><i class="fas fa-check"></i> <strong>Поддержка расширений</strong> — установка из Chrome Web Store</li>
                </ul>
            </div>
            
            <div class="system-requirements">
                <h2 class="section-title">Системные требования</h2>
                <table class="requirements-table">
                    <thead>
                        <tr>
                            <th>Компонент</th>
                            <th>Минимальные</th>
                            <th>Рекомендуемые</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>Операционная система</td>
                            <td>Windows 7 / macOS 10.12 / Ubuntu 16.04</td>
                            <td>Windows 10/11 / macOS 11+ / Ubuntu 20.04+</td>
                        </tr>
                        <tr>
                            <td>Процессор</td>
                            <td>Intel Pentium 4 или аналог</td>
                            <td>Intel Core i3 или аналог</td>
                        </tr>
                        <tr>
                            <td>Оперативная память</td>
                            <td>1 ГБ</td>
                            <td>4 ГБ</td>
                        </tr>
                        <tr>
                            <td>Видеокарта</td>
                            <td>С поддержкой DirectX 9 (Windows)</td>
                            <td>С поддержкой DirectX 11 (Windows)</td>
                        </tr>
                        <tr>
                            <td>Место на диске</td>
                            <td>200 МБ</td>
                            <td>500 МБ</td>
                        </tr>
                        <tr>
                            <td>Интернет</td>
                            <td>Для установки и обновлений</td>
                            <td>Широкополосный доступ</td>
                        </tr>
                    </tbody>
                </table>
            </div>
            
            <div class="app-screenshots">
                <h2 class="section-title">Скриншоты интерфейса</h2>
                <div class="screenshots-grid">
                    <div class="screenshot">
                        <img src="https://images.unsplash.com/photo-1611224923853-80b023f02d71?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Интерфейс Яндекс.Браузера">
                    </div>
                    <div class="screenshot">
                        <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Панель быстрого доступа">
                    </div>
                    <div class="screenshot">
                        <img src="https://images.unsplash.com/photo-1581276879432-15e50529f34b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Настройки браузера">
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Right Column: Sidebar -->
        <div class="sidebar">
            <!-- Related Apps -->
            <div class="related-apps">
                <h3 class="section-title">Другие браузеры</h3>
                <div class="related-apps-list">
                    <a href="chrome.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #4285F4;">
                            <i class="fab fa-chrome"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>Google Chrome</h4>
                            <p>Самый популярный браузер</p>
                        </div>
                    </a>
                    
                    <a href="firefox.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #FF7139;">
                            <i class="fab fa-firefox"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>Mozilla Firefox</h4>
                            <p>Браузер с открытым исходным кодом</p>
                        </div>
                    </a>
                    
                    <a href="opera.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #FF1B2D;">
                            <i class="fab fa-opera"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>Opera Browser</h4>
                            <p>С встроенным VPN и блокировщиком рекламы</p>
                        </div>
                    </a>
                    
                    <a href="edge.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #0078D7;">
                            <i class="fab fa-edge"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>Microsoft Edge</h4>
                            <p>Браузер на основе Chromium от Microsoft</p>
                        </div>
                    </a>
                </div>
            </div>
            
            <!-- Download Info -->
            <div class="download-info">
                <h3 class="section-title">Информация о загрузке</h3>
                <div class="download-info-item">
                    <h4><i class="fas fa-download"></i> Скачиваний</h4>
                    <p>Более 500,000 загрузок</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-calendar-alt"></i> Последнее обновление</h4>
                    <p>20 ноября 2023</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-user-check"></i> Разработчик</h4>
                    <p>Яндекс</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-language"></i> Языки интерфейса</h4>
                    <p>Русский, English, Türkçe, Українська</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-shield-alt"></i> Безопасность</h4>
                    <p>Проверено на вирусы</p>
                </div>
            </div>
            
            <!-- Quick Stats -->
            <div class="download-info">
                <h3 class="section-title">Быстрая статистика</h3>
                <div class="download-info-item">
                    <h4><i class="fas fa-bolt"></i> Скорость загрузки</h4>
                    <p>На 15% быстрее Chrome</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-memory"></i> Потребление памяти</h4>
                    <p>На 20% меньше чем Chrome</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-mobile-alt"></i> Мобильная версия</h4>
                    <p>Доступна для iOS и Android</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Comparison Section -->
    <section class="comparison-section">
        <div class="container">
            <h2 class="section-title">Сравнение с другими браузерами</h2>
            <table class="comparison-table">
                <thead>
                    <tr>
                        <th>Функция</th>
                        <th>Яндекс.Браузер</th>
                        <th>Google Chrome</th>
                        <th>Mozilla Firefox</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td class="feature-name">Встроенный переводчик</td>
                        <td class="yandex-check">✓ Встроен</td>
                        <td class="other-check">Требует расширение</td>
                        <td class="other-check">Требует расширение</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Режим Турбо</td>
                        <td class="yandex-check">✓ Есть</td>
                        <td class="other-check">Нет</td>
                        <td class="other-check">Нет</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Защита от вредоносных сайтов</td>
                        <td class="yandex-check">✓ Active Protect</td>
                        <td class="other-check">✓ Safe Browsing</td>
                        <td class="other-check">✓ Защита</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Встроенный блокировщик рекламы</td>
                        <td class="yandex-check">✓ Есть</td>
                        <td class="other-check">Требует расширение</td>
                        <td class="other-check">Требует расширение</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Экономия трафика</td>
                        <td class="yandex-check">✓ До 50%</td>
                        <td class="other-check">Ограниченная</td>
                        <td class="other-check">Ограниченная</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Синхронизация с мобильными устройствами</td>
                        <td class="yandex-check">✓ Полная</td>
                        <td class="other-check">✓ Полная</td>
                        <td class="other-check">✓ Полная</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Поддержка расширений Chrome</td>
                        <td class="yandex-check">✓ Полная</td>
                        <td class="other-check">✓ Полная</td>
                        <td class="other-check">Частичная</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <!-- How to Install -->
    <section class="how-to-install">
        <div class="container">
            <h2 class="section-title">Как установить Яндекс.Браузер</h2>
            <div class="install-steps">
                <div class="install-step">
                    <div class="step-number">1</div>
                    <div class="step-content">
                        <h4>Скачайте установщик</h4>
                        <p>Нажмите кнопку "Скачать для Windows" выше. Установщик Яндекс.Браузера будет загружен на ваш компьютер (файл размером ~85 MB).</p>
                    </div>
                </div>
                <div class="install-step">
                    <div class="step-number">2</div>
                    <div class="step-content">
                        <h4>Запустите установщик</h4>
                        <p>Найдите загруженный файл (обычно в папке "Загрузки") и запустите его двойным кликом. Разрешите программе вносить изменения на вашем устройстве.</p>
                    </div>
                </div>
                <div class="install-step">
                    <div class="step-number">3</div>
                    <div class="step-content">
                        <h4>Следуйте инструкциям установки</h4>
                        <p>Мастер установки предложит вам выбрать язык, принять лицензионное соглашение и указать папку для установки. Рекомендуем оставить параметры по умолчанию.</p>
                    </div>
                </div>
                <div class="install-step">
                    <div class="step-number">4</div>
                    <div class="step-content">
                        <h4>Завершите установку и запустите браузер</h4>
                        <p>После завершения установки Яндекс.Браузер автоматически запустится. Вы можете войти в аккаунт Яндекс для синхронизации данных или начать использование без входа.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Comments Section -->
    <section class="comments-section">
        <div class="container">
            <h2 class="section-title">Отзывы пользователей</h2>
            
            <div class="comment-form">
                <textarea placeholder="Оставьте ваш отзыв о Яндекс.Браузере..."></textarea>
                <button type="submit">Отправить отзыв</button>
            </div>
            
            <div class="comment">
                <div class="comment-avatar">
                    <i class="fas fa-user"></i>
                </div>
                <div class="comment-content">
                    <h4>Анна Семенова</h4>
                    <div class="comment-date">5 ноября 2023</div>
                    <p>Пользуюсь Яндекс.Браузером уже больше года. Очень нравится встроенный переводчик - не нужно устанавливать дополнительные расширения. Турбо-режим реально помогает при медленном интернете.</p>
                </div>
            </div>
            
            <div class="comment">
                <div class="comment-avatar">
                    <i class="fas fa-user"></i>
                </div>
                <div class="comment-content">
                    <h4>Дмитрий Волков</h4>
                    <div class="comment-date">28 октября 2023</div>
                    <p>Перешел с Chrome на Яндекс.Браузер полгода назад. Заметил, что работает быстрее, особенно на старом компьютере. Встроенный блокировщик рекламы тоже радует - страницы загружаются чище.</p>
                </div>
            </div>
            
            <div class="comment">
                <div class="comment-avatar">
                    <i class="fas fa-user"></i>
                </div>
                <div class="comment-content">
                    <h4>Ольга Петрова</h4>
                    <div class="comment-date">15 октября 2023</div>
                    <p>Хороший браузер, но есть небольшой недостаток - иногда подвисает при открытии множества вкладок. В целом довольна, особенно интеграцией с сервисами Яндекса.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Загрузки</h3>
                    <p>Каталог проверенных программ для Windows, Linux и macOS. Все файлы проверены на вирусы и безопасность.</p>
                    <div style="margin-top: 20px; display: flex; gap: 15px;">
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-vk"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-telegram"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-github"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Навигация</h3>
                    <ul class="footer-links">
                        <li><a href="index.html">Главная страница</a></li>
                        <li><a href="browsers.html">Браузеры</a></li>
                        <li><a href="games.html">Игры</a></li>
                        <li><a href="software.html">Программы</a></li>
                        <li><a href="tools.html">Утилиты</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Популярные программы</h3>
                    <ul class="footer-links">
                        <li><a href="yandex-browser.html">Яндекс.Браузер</a></li>
                        <li><a href="chrome.html">Google Chrome</a></li>
                        <li><a href="firefox.html">Mozilla Firefox</a></li>
                        <li><a href="vivaldi.html">Vivaldi Browser</a></li>
                        <li><a href="opera.html">Opera Browser</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Помощь и поддержка</h3>
                    <ul class="footer-links">
                        <li><a href="faq.html">Частые вопросы</a></li>
                        <li><a href="contact.html">Контакты</a></li>
                        <li><a href="policy.html">Политика безопасности</a></li>
                        <li><a href="dmca.html">DMCA</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2023 Загрузки. Все права защищены. Все программы являются собственностью их разработчиков.</p>
                <p style="margin-top: 10px;">Сайт предоставляет ссылки для загрузки официальных версий программ.</p>
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
        
        // Кнопки скачивания
        document.getElementById('download-windows').addEventListener('click', function() {
            alert('Загрузка Яндекс.Браузера для Windows начата!\n\nФайл: yandex_browser_setup.exe\nРазмер: 85.4 MB\n\nФайл будет сохранен в папке "Загрузки".');
        });
        
        document.getElementById('download-linux').addEventListener('click', function() {
            alert('Загрузка Яндекс.Браузера для Linux начата!\n\nФайл: yandex-browser_current_amd64.deb\nРазмер: 87.2 MB\n\nВыберите версию для вашего дистрибутива Linux.');
        });
        
        document.getElementById('download-mac').addEventListener('click', function() {
            alert('Загрузка Яндекс.Браузера для macOS начата!\n\nФайл: Yandex.dmg\nРазмер: 89.1 MB\n\nПоддерживаются macOS 10.12 и выше.');
        });
        
        // Обновление года в футере
        document.querySelector('.footer-bottom p').innerHTML = `&copy; ${new Date().getFullYear()} Загрузки. Все права защищены. Все программы являются собственностью их разработчиков.`;
        
        // Отправка комментария
        const commentForm = document.querySelector('.comment-form');
        const commentTextarea = commentForm.querySelector('textarea');
        const commentButton = commentForm.querySelector('button');
        
        commentButton.addEventListener('click', function() {
            if (commentTextarea.value.trim() === '') {
                alert('Пожалуйста, введите текст отзыва');
                return;
            }
            
            alert('Спасибо за ваш отзыв! После модерации он будет опубликован на сайте.');
            commentTextarea.value = '';
        });
        
        // Анимация элементов при прокрутке
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
        
        // Применяем анимацию к элементам
        document.querySelectorAll('.install-step, .related-app, .comment').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            observer.observe(el);
        });
        
        // Подсветка активной ссылки в хлебных крошках
        const currentPage = window.location.pathname.split('/').pop() || 'index.html';
        const breadcrumbLinks = document.querySelectorAll('.breadcrumbs a');
        
        breadcrumbLinks.forEach(link => {
            const href = link.getAttribute('href');
            if (href === currentPage || (currentPage.includes('yandex') && href.includes('browsers'))) {
                link.style.color = 'var(--primary-color)';
                link.style.fontWeight = '600';
            }
        });
    </script>
</body>
</html>
