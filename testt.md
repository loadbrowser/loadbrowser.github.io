<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Brawl Stars Browser - LoadBrowser</title>
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
            background: linear-gradient(135deg, #e8f5e9 0%, #f1f8e9 100%);
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
            background: linear-gradient(135deg, #ff9800, #ff5722);
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: var(--box-shadow);
        }

        .app-icon-large i {
            font-size: 3.5rem;
            color: white;
        }

        .app-header-info {
            flex: 1;
        }

        .app-title {
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: var(--dark-color);
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
            background-color: #e8f5e9;
            transform: translateX(5px);
        }

        .related-app-icon {
            width: 50px;
            height: 50px;
            border-radius: 10px;
            background-color: var(--primary-color);
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
            
            .app-icon-large i {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="index.html" class="logo">
                <i class="fas fa-rocket"></i>
                <div class="logo-text">
                    LoadBrowser
                    <span class="logo-subtitle">Browser Games Loader</span>
                </div>
            </a>
            
            <nav class="nav-links">
                <a href="index.html">Главная</a>
                <a href="index.html#apps">Приложения</a>
                <a href="index.html#how-to-use">Как использовать</a>
                <a href="index.html#faq">FAQ</a>
                <a href="index.html#download">Скачать</a>
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

    <!-- Breadcrumbs -->
    <section class="breadcrumbs">
        <div class="container breadcrumbs-container">
            <a href="index.html"><i class="fas fa-home"></i> Главная</a>
            <i class="fas fa-chevron-right"></i>
            <a href="index.html#apps">Приложения</a>
            <i class="fas fa-chevron-right"></i>
            <span>Brawl Stars Browser</span>
        </div>
    </section>

    <!-- App Detail Header -->
    <section class="app-detail-header">
        <div class="container">
            <div class="app-header-content">
                <div class="app-icon-large">
                    <i class="fas fa-fist-raised"></i>
                </div>
                <div class="app-header-info">
                    <h1 class="app-title">Brawl Stars Browser</h1>
                    <div class="app-meta">
                        <span class="app-version">Версия 1.5</span>
                        <div class="app-rating">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star-half-alt"></i>
                            <span>4.7</span>
                        </div>
                        <span class="app-size">Размер: ~220 MB</span>
                    </div>
                    <p>Запускайте Brawl Stars напрямую на компьютере без эмуляторов с улучшенной графикой и управлением.</p>
                    <div class="app-header-actions">
                        <button class="btn btn-primary">
                            <i class="fas fa-download"></i> Скачать сейчас
                        </button>
                        <button class="btn btn-secondary">
                            <i class="fas fa-play-circle"></i> Смотреть геймплей
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
            <h2 class="section-title">Описание приложения</h2>
            <div class="app-description">
                <p>Brawl Stars Browser - это специальная версия популярной игры Brawl Stars, оптимизированная для запуска на компьютере через LoadBrowser. Приложение позволяет играть в Brawl Stars без использования эмуляторов Android, что обеспечивает лучшую производительность и стабильность.</p>
                <p>Игра адаптирована для управления с клавиатуры и мыши, что дает преимущество в точности стрельбы и реакции. Все режимы игры доступны, включая командные сражения, стычки и особые события.</p>
            </div>
            
            <div class="app-features">
                <h2 class="section-title">Основные особенности</h2>
                <ul>
                    <li><i class="fas fa-check"></i> Прямой запуск без эмуляторов</li>
                    <li><i class="fas fa-check"></i> Настраиваемое управление с клавиатуры</li>
                    <li><i class="fas fa-check"></i> Улучшенная графика и производительность</li>
                    <li><i class="fas fa-check"></i> Поддержка геймпадов Xbox и PS4</li>
                    <li><i class="fas fa-check"></i> Автообновления до последней версии</li>
                    <li><i class="fas fa-check"></i> Быстрое подключение к серверам</li>
                    <li><i class="fas fa-check"></i> Сохранение прогресса в облаке</li>
                    <li><i class="fas fa-check"></i> Поддержка внутриигровых покупок</li>
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
                            <td>Windows 7</td>
                            <td>Windows 10/11</td>
                        </tr>
                        <tr>
                            <td>Процессор</td>
                            <td>Intel Core i3 или аналог</td>
                            <td>Intel Core i5 или аналог</td>
                        </tr>
                        <tr>
                            <td>Оперативная память</td>
                            <td>4 ГБ</td>
                            <td>8 ГБ</td>
                        </tr>
                        <tr>
                            <td>Видеокарта</td>
                            <td>Intel HD Graphics 4000</td>
                            <td>NVIDIA GTX 660 / AMD Radeon HD 7850</td>
                        </tr>
                        <tr>
                            <td>Место на диске</td>
                            <td>500 МБ</td>
                            <td>1 ГБ</td>
                        </tr>
                        <tr>
                            <td>Интернет</td>
                            <td>5 Мбит/с</td>
                            <td>10 Мбит/с</td>
                        </tr>
                    </tbody>
                </table>
            </div>
            
            <div class="app-screenshots">
                <h2 class="section-title">Скриншоты</h2>
                <div class="screenshots-grid">
                    <div class="screenshot">
                        <img src="https://images.unsplash.com/photo-1511512578047-dfb367046420?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Скриншот Brawl Stars 1">
                    </div>
                    <div class="screenshot">
                        <img src="https://images.unsplash.com/photo-1534423861386-85a16f5d13fd?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w-600&q=80" alt="Скриншот Brawl Stars 2">
                    </div>
                    <div class="screenshot">
                        <img src="https://images.unsplash.com/photo-1550745165-9bc0b252726f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Скриншот Brawl Stars 3">
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Right Column: Sidebar -->
        <div class="sidebar">
            <!-- Related Apps -->
            <div class="related-apps">
                <h3 class="section-title">Похожие приложения</h3>
                <div class="related-apps-list">
                    <a href="steam-browser.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #171a21;">
                            <i class="fab fa-steam"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>Steam Browser</h4>
                            <p>Доступ к магазину Steam и библиотеке</p>
                        </div>
                    </a>
                    
                    <a href="minecraft-browser.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #6caa3f;">
                            <i class="fas fa-cube"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>Minecraft Browser</h4>
                            <p>Браузерная версия Minecraft</p>
                        </div>
                    </a>
                    
                    <a href="pubg-browser.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #f7a41d;">
                            <i class="fas fa-crosshairs"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>PUBG Browser</h4>
                            <p>Запуск PUBG на компьютере</p>
                        </div>
                    </a>
                    
                    <a href="standoff2-browser.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #6c5ce7;">
                            <i class="fas fa-user-secret"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>Standoff 2 Browser</h4>
                            <p>Шутер от первого лица</p>
                        </div>
                    </a>
                </div>
            </div>
            
            <!-- Download Info -->
            <div class="download-info">
                <h3 class="section-title">Информация для скачивания</h3>
                <div class="download-info-item">
                    <h4><i class="fas fa-download"></i> Скачиваний</h4>
                    <p>Более 150,000 загрузок</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-calendar-alt"></i> Последнее обновление</h4>
                    <p>15 ноября 2023</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-user-check"></i> Разработчик</h4>
                    <p>Supercell / LoadBrowser Team</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-language"></i> Языки</h4>
                    <p>Русский, English, Español, Français</p>
                </div>
            </div>
        </div>
    </div>

    <!-- How to Install -->
    <section class="how-to-install">
        <div class="container">
            <h2 class="section-title">Как установить Brawl Stars Browser</h2>
            <div class="install-steps">
                <div class="install-step">
                    <div class="step-number">1</div>
                    <div class="step-content">
                        <h4>Скачайте LoadBrowser</h4>
                        <p>Если у вас еще не установлен LoadBrowser, скачайте его с <a href="index.html#download">главной страницы</a>. Установите программу, следуя инструкциям.</p>
                    </div>
                </div>
                <div class="install-step">
                    <div class="step-number">2</div>
                    <div class="step-content">
                        <h4>Запустите LoadBrowser</h4>
                        <p>Откройте установленный LoadBrowser. В главном меню найдите Brawl Stars Browser в списке доступных приложений или воспользуйтесь поиском.</p>
                    </div>
                </div>
                <div class="install-step">
                    <div class="step-number">3</div>
                    <div class="step-content">
                        <h4>Установите приложение</h4>
                        <p>Нажмите кнопку "Установить" на странице Brawl Stars Browser. Дождитесь завершения загрузки и установки приложения.</p>
                    </div>
                </div>
                <div class="install-step">
                    <div class="step-number">4</div>
                    <div class="step-content">
                        <h4>Настройте управление</h4>
                        <p>После установки зайдите в настройки управления и настройте клавиши под себя. Рекомендуемые настройки уже установлены по умолчанию.</p>
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
                <textarea placeholder="Оставьте ваш отзыв о Brawl Stars Browser..."></textarea>
                <button type="submit">Отправить отзыв</button>
            </div>
            
            <div class="comment">
                <div class="comment-avatar">
                    <i class="fas fa-user"></i>
                </div>
                <div class="comment-content">
                    <h4>Алексей Петров</h4>
                    <div class="comment-date">5 ноября 2023</div>
                    <p>Отличная версия игры! Управление с клавиатуры и мыши намного удобнее, чем на телефоне. FPS стабильный, никаких лагов. Рекомендую!</p>
                </div>
            </div>
            
            <div class="comment">
                <div class="comment-avatar">
                    <i class="fas fa-user"></i>
                </div>
                <div class="comment-content">
                    <h4>Мария Смирнова</h4>
                    <div class="comment-date">28 октября 2023</div>
                    <p>Играю уже неделю через LoadBrowser. Очень удобно, что не нужно использовать эмулятор. Графика лучше, чем на телефоне. Единственное - иногда бывают проблемы с подключением к серверам.</p>
                </div>
            </div>
            
            <div class="comment">
                <div class="comment-avatar">
                    <i class="fas fa-user"></i>
                </div>
                <div class="comment-content">
                    <h4>Дмитрий Иванов</h4>
                    <div class="comment-date">15 октября 2023</div>
                    <p>Отличная работа разработчиков! Все работает стабильно, управление настраивается под себя. Хотелось бы больше настроек графики для слабых компьютеров.</p>
                </div>
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
                    <h3>Навигация</h3>
                    <ul class="footer-links">
                        <li><a href="index.html">Главная страница</a></li>
                        <li><a href="index.html#apps">Все приложения</a></li>
                        <li><a href="index.html#how-to-use">Инструкция</a></li>
                        <li><a href="index.html#faq">Частые вопросы</a></li>
                        <li><a href="index.html#download">Скачать LoadBrowser</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Популярные игры</h3>
                    <ul class="footer-links">
                        <li><a href="brawl-stars-browser.html">Brawl Stars Browser</a></li>
                        <li><a href="steam-browser.html">Steam Browser</a></li>
                        <li><a href="minecraft-browser.html">Minecraft Browser</a></li>
                        <li><a href="pubg-browser.html">PUBG Browser</a></li>
                        <li><a href="whatsapp-browser.html">WhatsApp Browser</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Помощь и поддержка</h3>
                    <ul class="footer-links">
                        <li><a href="#">Техническая поддержка</a></li>
                        <li><a href="#">Сообщить об ошибке</a></li>
                        <li><a href="#">Форум</a></li>
                        <li><a href="#">Контакты</a></li>
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
        
        // Кнопки скачивания
        document.querySelectorAll('.btn-primary').forEach(btn => {
            btn.addEventListener('click', function() {
                alert('Начата загрузка Brawl Stars Browser v1.5\n\nРазмер файла: ~220 MB\nЗагрузка начнется через несколько секунд.');
            });
        });
        
        // Обновление года в футере
        document.querySelector('.footer-bottom p').innerHTML = `&copy; ${new Date().getFullYear()} LoadBrowser. Все права защищены. LoadBrowser не аффилирован с компаниями, чьи игры представлены в каталоге.`;
        
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
            if (href === currentPage || (currentPage.includes('browser') && href.includes(currentPage.replace('-browser.html', '')))) {
                link.style.color = 'var(--primary-color)';
                link.style.fontWeight = '600';
            }
        });
    </script>
</body>
</html>
