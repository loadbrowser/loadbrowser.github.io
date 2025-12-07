---
layout: default
title: Яндекс.Диск| Скачать Яндекс Диск
description: Скачайте Яндекс Диск бесплатно на компьютер Windows.
---

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Яндекс.Диск — скачать бесплатно на Windows | Облачное хранилище</title>
    <meta name="description" content="Скачайте Яндекс.Диск на Windows бесплатно. Официальное облачное хранилище от Яндекса. 10 ГБ свободного места, синхронизация файлов, защита данных.">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #FFCC00;
            --primary-dark: #E6B800;
            --secondary-color: #FF2E2E;
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
            color: #333;
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

        /* Hero Section */
        .hero {
            padding: 60px 0;
            background: linear-gradient(135deg, #FFF9E6 0%, #FFF3CC 100%);
        }

        .hero-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }

        .hero-text {
            flex: 1;
        }

        .hero-text h1 {
            font-size: 2.8rem;
            margin-bottom: 20px;
            color: var(--dark-color);
        }

        .hero-text h1 span {
            color: var(--secondary-color);
        }

        .hero-text p {
            font-size: 1.1rem;
            color: var(--gray-color);
            margin-bottom: 30px;
            max-width: 600px;
        }

        .hero-badges {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
            margin-bottom: 30px;
        }

        .badge {
            background-color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-weight: 600;
            font-size: 0.9rem;
            box-shadow: var(--box-shadow);
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .badge i {
            color: var(--success-color);
        }

        .hero-actions {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            padding: 14px 28px;
            border-radius: var(--border-radius);
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            border: none;
            font-size: 1.1rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .btn-primary {
            background-color: var(--primary-color);
            color: #333;
        }

        .btn-primary:hover {
            background-color: var(--primary-dark);
            transform: translateY(-3px);
        }

        .btn-secondary {
            background-color: white;
            color: #333;
            border: 2px solid var(--primary-color);
        }

        .btn-secondary:hover {
            background-color: #f5f5f5;
        }

        .hero-image {
            flex: 1;
            display: flex;
            justify-content: center;
        }

        .app-showcase {
            width: 100%;
            max-width: 500px;
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            overflow: hidden;
        }

        .app-header {
            background-color: #f5f5f5;
            padding: 15px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 1px solid var(--light-gray);
        }

        .app-title {
            display: flex;
            align-items: center;
            gap: 10px;
            font-weight: 600;
        }

        .app-title i {
            color: var(--primary-color);
        }

        .app-content {
            padding: 30px;
            text-align: center;
        }

        .cloud-icon {
            width: 100px;
            height: 100px;
            background: linear-gradient(135deg, var(--primary-color), #FFDD44);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 25px;
            position: relative;
        }

        .cloud-icon i {
            font-size: 3.5rem;
            color: white;
        }

        .storage-info {
            background-color: #f9f9f9;
            border-radius: var(--border-radius);
            padding: 20px;
            margin-top: 25px;
        }

        .storage-bar {
            height: 10px;
            background-color: var(--light-gray);
            border-radius: 5px;
            margin: 15px 0;
            overflow: hidden;
        }

        .storage-fill {
            height: 100%;
            width: 35%;
            background: linear-gradient(90deg, var(--primary-color), #FFDD44);
            border-radius: 5px;
        }

        /* Features Section */
        .features {
            padding: 80px 0;
            background-color: white;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            font-size: 2.2rem;
            color: var(--dark-color);
            margin-bottom: 15px;
        }

        .section-title p {
            color: var(--gray-color);
            max-width: 700px;
            margin: 0 auto;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .feature-card {
            background-color: #f9f9f9;
            border-radius: var(--border-radius);
            padding: 30px;
            transition: var(--transition);
        }

        .feature-card:hover {
            background-color: #FFF9E6;
            transform: translateY(-5px);
        }

        .feature-icon {
            width: 70px;
            height: 70px;
            background-color: rgba(255, 204, 0, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
        }

        .feature-icon i {
            font-size: 2rem;
            color: var(--primary-color);
        }

        .feature-card h3 {
            font-size: 1.4rem;
            margin-bottom: 15px;
            color: var(--dark-color);
        }

        /* Installation Guide */
        .installation {
            padding: 80px 0;
            background-color: #f5f5f5;
        }

        .guide-steps {
            display: flex;
            flex-direction: column;
            gap: 40px;
            max-width: 800px;
            margin: 0 auto;
        }

        .guide-step {
            display: flex;
            gap: 25px;
            align-items: flex-start;
        }

        .step-number {
            width: 50px;
            height: 50px;
            background-color: var(--primary-color);
            color: #333;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 700;
            font-size: 1.3rem;
            flex-shrink: 0;
        }

        .step-content {
            flex: 1;
        }

        .step-content h3 {
            font-size: 1.4rem;
            margin-bottom: 10px;
            color: var(--dark-color);
        }

        .step-content p {
            color: var(--gray-color);
            margin-bottom: 15px;
        }

        .step-image {
            margin-top: 20px;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--box-shadow);
        }

        .step-image img {
            width: 100%;
            height: auto;
            display: block;
        }

        /* System Requirements */
        .requirements {
            padding: 80px 0;
            background-color: white;
        }

        .requirements-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .requirement-card {
            background-color: #f9f9f9;
            border-radius: var(--border-radius);
            padding: 30px;
            text-align: center;
            transition: var(--transition);
        }

        .requirement-card:hover {
            background-color: #FFF9E6;
        }

        .requirement-icon {
            width: 60px;
            height: 60px;
            background-color: rgba(255, 204, 0, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
        }

        .requirement-icon i {
            font-size: 1.8rem;
            color: var(--primary-color);
        }

        /* Comparison Section */
        .comparison {
            padding: 80px 0;
            background-color: #f5f5f5;
        }

        .comparison-table {
            width: 100%;
            border-collapse: collapse;
            background-color: white;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--box-shadow);
        }

        .comparison-table th, .comparison-table td {
            padding: 20px;
            text-align: left;
            border-bottom: 1px solid var(--light-gray);
        }

        .comparison-table th {
            background-color: #f9f9f9;
            font-weight: 600;
            color: var(--dark-color);
        }

        .comparison-table .feature-name {
            font-weight: 600;
            color: var(--dark-color);
        }

        .comparison-table .check {
            color: var(--success-color);
            font-weight: bold;
        }

        .comparison-table .partial {
            color: var(--warning-color);
        }

        /* FAQ Section */
        .faq {
            padding: 80px 0;
            background-color: white;
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

        /* Download Section */
        .download-section {
            padding: 80px 0;
            background: linear-gradient(135deg, var(--primary-color), #FFDD44);
            text-align: center;
        }

        .download-section h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: #333;
        }

        .download-section p {
            font-size: 1.2rem;
            margin-bottom: 40px;
            color: #333;
            opacity: 0.9;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }

        .download-info {
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: var(--border-radius);
            padding: 25px;
            max-width: 500px;
            margin: 0 auto 40px;
            box-shadow: var(--box-shadow);
        }

        .download-info-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 15px;
            padding-bottom: 15px;
            border-bottom: 1px solid var(--light-gray);
        }

        .download-info-item:last-child {
            margin-bottom: 0;
            padding-bottom: 0;
            border-bottom: none;
        }

        /* Related Apps */
        .related-apps {
            padding: 80px 0;
            background-color: #f5f5f5;
        }

        .apps-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }

        .app-card {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 30px;
            text-align: center;
            text-decoration: none;
            color: var(--dark-color);
            transition: var(--transition);
            box-shadow: var(--box-shadow);
        }

        .app-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }

        .app-icon {
            width: 70px;
            height: 70px;
            border-radius: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
        }

        .app-icon i {
            font-size: 2rem;
            color: white;
        }

        .app-card h3 {
            margin-bottom: 10px;
        }

        .app-card p {
            color: var(--gray-color);
            font-size: 0.95rem;
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

        /* Responsive */
        @media (max-width: 992px) {
            .hero-content {
                flex-direction: column;
                text-align: center;
            }
            
            .hero-text h1 {
                font-size: 2.3rem;
            }
            
            .guide-step {
                flex-direction: column;
            }
            
            .step-number {
                align-self: center;
            }
        }

        @media (max-width: 768px) {
            .nav-links, .header-actions {
                display: none;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .section-title h2 {
                font-size: 1.8rem;
            }
            
            .hero-actions {
                flex-direction: column;
            }
            
            .btn {
                width: 100%;
                justify-content: center;
            }
            
            .comparison-table {
                display: block;
                overflow-x: auto;
            }
        }

        @media (max-width: 576px) {
            .hero-text h1 {
                font-size: 2rem;
            }
            
            .download-section h2 {
                font-size: 2rem;
            }
            
            .apps-grid {
                grid-template-columns: 1fr;
            }
            
            .features-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="https://loadbrowser.github.io/" class="logo">
                <i class="fas fa-cloud"></i>
                <div class="logo-text">
                    Яндекс.Диск
                    <span class="logo-subtitle">Облачное хранилище</span>
                </div>
            </a>
            
            <nav class="nav-links">
                <a href="https://loadbrowser.github.io/">Главная</a>
                <a href="https://loadbrowser.github.io/yandex-browser.html">Яндекс.Браузер</a>
                <a href="https://loadbrowser.github.io/adguard.html">AdGuard</a>
                <a href="https://loadbrowser.github.io/adguard-vpn.html">AdGuard VPN</a>
                <a href="#download" class="active">Скачать</a>
            </nav>
            
            <div class="header-actions">
                <button class="download-btn" id="header-download">
                    <i class="fas fa-download"></i>
                    Скачать для Windows
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
            <a href="https://loadbrowser.github.io/"><i class="fas fa-home"></i> Главная</a>
            <i class="fas fa-chevron-right"></i>
            <a href="https://loadbrowser.github.io/yandex-browser.html">Яндекс.Браузер</a>
            <i class="fas fa-chevron-right"></i>
            <span>Яндекс.Диск для Windows</span>
        </div>
    </section>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container hero-content">
            <div class="hero-text">
                <h1><span>Яндекс.Диск</span> для Windows</h1>
                <p>Бесплатное облачное хранилище от Яндекса. Синхронизируйте файлы между устройствами, делитесь ими с друзьями и коллегами, работайте с документами онлайн.</p>
                
                <div class="hero-badges">
                    <div class="badge">
                        <i class="fas fa-check"></i>
                        10 ГБ бесплатно
                    </div>
                    <div class="badge">
                        <i class="fas fa-check"></i>
                        Автосинхронизация
                    </div>
                    <div class="badge">
                        <i class="fas fa-check"></i>
                        Русский интерфейс
                    </div>
                </div>
                
                <div class="hero-actions">
                    <button class="btn btn-primary" id="main-download">
                        <i class="fas fa-download"></i> Скачать Яндекс.Диск
                    </button>
                    <button class="btn btn-secondary" id="web-version">
                        <i class="fas fa-globe"></i> Веб-версия
                    </button>
                </div>
                
                <div style="margin-top: 30px; display: flex; align-items: center; gap: 15px; flex-wrap: wrap;">
                    <div style="display: flex; align-items: center; gap: 8px;">
                        <i class="fas fa-check-circle" style="color: var(--success-color);"></i>
                        <span>Версия 3.2.18</span>
                    </div>
                    <div style="display: flex; align-items: center; gap: 8px;">
                        <i class="fas fa-hdd" style="color: var(--accent-color);"></i>
                        <span>Размер: 95.3 MB</span>
                    </div>
                    <div style="display: flex; align-items: center; gap: 8px;">
                        <i class="fas fa-star" style="color: var(--warning-color);"></i>
                        <span>4.7 ★ (12,847 оценок)</span>
                    </div>
                </div>
            </div>
            
            <div class="hero-image">
                <div class="app-showcase">
                    <div class="app-header">
                        <div class="app-title">
                            <i class="fas fa-cloud"></i>
                            Яндекс.Диск
                        </div>
                        <div style="font-size: 0.9rem; color: var(--gray-color);">
                            Синхронизировано
                        </div>
                    </div>
                    <div class="app-content">
                        <div class="cloud-icon">
                            <i class="fas fa-cloud"></i>
                        </div>
                        <h3 style="margin-bottom: 10px;">Облачное хранилище</h3>
                        <p style="color: var(--gray-color); margin-bottom: 20px;">Ваши файлы всегда под рукой</p>
                        
                        <div class="storage-info">
                            <div style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                                <span>Использовано: 3.5 ГБ</span>
                                <span>10 ГБ</span>
                            </div>
                            <div class="storage-bar">
                                <div class="storage-fill"></div>
                            </div>
                            <div style="color: var(--gray-color); font-size: 0.9rem;">
                                Свободно: 6.5 ГБ
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features">
        <div class="container">
            <div class="section-title">
                <h2>Возможности Яндекс.Диска для Windows</h2>
                <p>Все, что нужно для удобной работы с файлами в облаке</p>
            </div>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-sync-alt"></i>
                    </div>
                    <h3>Автосинхронизация</h3>
                    <p>Файлы автоматически синхронизируются между вашим компьютером и облаком. Изменения сохраняются в реальном времени.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-share-alt"></i>
                    </div>
                    <h3>Общий доступ</h3>
                    <p>Делитесь файлами и папками с друзьями и коллегами. Настройте права доступа: только просмотр или полный доступ.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-history"></i>
                    </div>
                    <h3>История версий</h3>
                    <p>Храните историю изменений файлов за 30 дней. Восстановите предыдущую версию, если что-то пошло не так.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-mobile-alt"></i>
                    </div>
                    <h3>Доступ с любых устройств</h3>
                    <p>Работайте с файлами на компьютере, ноутбуке, смартфоне или планшете. Приложения для Windows, macOS, iOS и Android.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-lock"></i>
                    </div>
                    <h3>Защита данных</h3>
                    <p>Все файлы шифруются при передаче и хранятся в защищенных дата-центрах. Доступ только по вашему паролю.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-search"></i>
                    </div>
                    <h3>Быстрый поиск</h3>
                    <p>Находите файлы по названию, содержимому или дате изменения. Яндекс.Диск умеет распознавать текст на фотографиях.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Installation Guide -->
    <section class="installation">
        <div class="container">
            <div class="section-title">
                <h2>Как установить Яндекс.Диск на Windows</h2>
                <p>Простая пошаговая инструкция по установке и настройке</p>
            </div>
            
            <div class="guide-steps">
                <!-- Step 1 -->
                <div class="guide-step">
                    <div class="step-number">1</div>
                    <div class="step-content">
                        <h3>Скачайте установщик</h3>
                        <p>Нажмите кнопку "Скачать Яндекс.Диск" выше. Установочный файл будет загружен на ваш компьютер (размер около 95 МБ).</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1593640408182-31c70c8268f5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Скачивание Яндекс.Диска">
                        </div>
                    </div>
                </div>
                
                <!-- Step 2 -->
                <div class="guide-step">
                    <div class="step-number">2</div>
                    <div class="step-content">
                        <h3>Запустите установщик</h3>
                        <p>Найдите скачанный файл <strong>YandexDiskSetup.exe</strong> в папке "Загрузки" и запустите его двойным кликом.</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1542831371-29b0f74f9713?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Запуск установщика">
                        </div>
                    </div>
                </div>
                
                <!-- Step 3 -->
                <div class="guide-step">
                    <div class="step-number">3</div>
                    <div class="step-content">
                        <h3>Следуйте инструкциям мастера</h3>
                        <p>В окне установки выберите язык, прочитайте лицензионное соглашение и нажмите "Установить". Процесс займет 1-2 минуты.</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1518709268805-4e9042af2176?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Мастер установки">
                        </div>
                    </div>
                </div>
                
                <!-- Step 4 -->
                <div class="guide-step">
                    <div class="step-number">4</div>
                    <div class="step-content">
                        <h3>Войдите в аккаунт Яндекс</h3>
                        <p>После установки войдите в свой аккаунт Яндекс. Если у вас его нет — создайте бесплатный аккаунт за 2 минуты.</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Вход в аккаунт">
                        </div>
                    </div>
                </div>
                
                <!-- Step 5 -->
                <div class="guide-step">
                    <div class="step-number">5</div>
                    <div class="step-content">
                        <h3>Настройте синхронизацию</h3>
                        <p>Выберите папки для синхронизации или оставьте настройки по умолчанию. Яндекс.Диск появится в проводнике Windows.</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1517077304055-6e89abbf09b0?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Настройка синхронизации">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- System Requirements -->
    <section class="requirements">
        <div class="container">
            <div class="section-title">
                <h2>Системные требования</h2>
                <p>Проверьте, подходит ли ваш компьютер для Яндекс.Диска</p>
            </div>
            
            <div class="requirements-grid">
                <div class="requirement-card">
                    <div class="requirement-icon">
                        <i class="fab fa-windows"></i>
                    </div>
                    <h3>Операционная система</h3>
                    <p>Windows 7, 8, 8.1, 10, 11 (32-бит или 64-бит)</p>
                </div>
                
                <div class="requirement-card">
                    <div class="requirement-icon">
                        <i class="fas fa-microchip"></i>
                    </div>
                    <h3>Процессор</h3>
                    <p>1 ГГц или выше (рекомендуется Intel Core i3 или аналогичный)</p>
                </div>
                
                <div class="requirement-card">
                    <div class="requirement-icon">
                        <i class="fas fa-memory"></i>
                    </div>
                    <h3>Оперативная память</h3>
                    <p>1 ГБ ОЗУ (рекомендуется 2 ГБ или больше)</p>
                </div>
                
                <div class="requirement-card">
                    <div class="requirement-icon">
                        <i class="fas fa-hdd"></i>
                    </div>
                    <h3>Свободное место</h3>
                    <p>200 МБ для установки + место для ваших файлов в облаке</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Comparison Section -->
    <section class="comparison">
        <div class="container">
            <div class="section-title">
                <h2>Сравнение с другими облачными хранилищами</h2>
                <p>Почему Яндекс.Диск — лучший выбор для Windows</p>
            </div>
            
            <table class="comparison-table">
                <thead>
                    <tr>
                        <th>Функция</th>
                        <th>Яндекс.Диск</th>
                        <th>Google Drive</th>
                        <th>Dropbox</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td class="feature-name">Бесплатный объем</td>
                        <td class="check">10 ГБ</td>
                        <td class="check">15 ГБ</td>
                        <td class="check">2 ГБ</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Русский интерфейс</td>
                        <td class="check">Полный</td>
                        <td class="partial">Частичный</td>
                        <td class="partial">Частичный</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Интеграция с Windows</td>
                        <td class="check">Полная</td>
                        <td class="check">Полная</td>
                        <td class="check">Полная</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Совместимость с Яндекс.Браузером</td>
                        <td class="check">Идеальная</td>
                        <td class="partial">Хорошая</td>
                        <td class="check">Хорошая</td>
                    </tr>
                    <tr>
                        <td class="feature-name">История версий файлов</td>
                        <td class="check">30 дней</td>
                        <td class="check">30 дней</td>
                        <td class="check">30 дней</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Максимальный размер файла</td>
                        <td class="check">50 ГБ</td>
                        <td class="check">5 ТБ</td>
                        <td class="check">50 ГБ</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Стоимость 1 ТБ</td>
                        <td class="check">299 ₽/месяц</td>
                        <td class="check">699 ₽/месяц</td>
                        <td class="check">1 199 ₽/месяц</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <!-- FAQ Section -->
    <section class="faq">
        <div class="container">
            <div class="section-title">
                <h2>Частые вопросы о Яндекс.Диске</h2>
                <p>Ответы на самые популярные вопросы пользователей</p>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Яндекс.Диск действительно бесплатный?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, Яндекс.Диск предоставляет 10 ГБ облачного пространства совершенно бесплатно. Этого достаточно для хранения документов, фотографий и важных файлов. При необходимости вы можете расширить хранилище до 1 ТБ или 3 ТБ за дополнительную плату.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Можно ли использовать Яндекс.Диск вместе с Яндекс.Браузером?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, Яндекс.Диск идеально интегрирован с <a href="https://loadbrowser.github.io/yandex-browser.html" style="color: var(--primary-color); font-weight: 600;">Яндекс.Браузером</a>. Вы можете сохранять файлы прямо из браузера в облако, открывать документы онлайн и делиться ссылками через контекстное меню браузера.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Защищены ли мои файлы в Яндекс.Диске?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, все файлы шифруются при передаче по защищенному протоколу HTTPS и хранятся в зашифрованном виде в дата-центрах Яндекса. Доступ к вашим файлам есть только у вас и у тех, с кем вы поделились файлами. Яндекс не имеет доступа к содержимому ваших файлов.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Что произойдет, если я удалю файл на компьютере?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Если файл был синхронизирован с Яндекс.Диском, он останется в облаке и в Корзине Яндекс.Диска (хранится 30 дней). Вы можете восстановить его в течение этого времени. Если вы удалите файл и из Корзины, он будет окончательно удален.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Можно ли работать с Яндекс.Диском без установки программы?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, у Яндекс.Диска есть полнофункциональная веб-версия, доступная через браузер. Вы можете загружать, скачивать, сортировать и делиться файлами прямо на сайте <a href="https://disk.yandex.ru" style="color: var(--primary-color); font-weight: 600;">disk.yandex.ru</a>. Однако для автоматической синхронизации файлов между компьютером и облаком рекомендуется установить приложение.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Download Section -->
    <section class="download-section" id="download">
        <div class="container">
            <h2>Скачайте Яндекс.Диск для Windows</h2>
            <p>Установите официальное приложение Яндекс.Диска и получите 10 ГБ облачного хранилища бесплатно</p>
            
            <div class="download-info">
                <div class="download-info-item">
                    <span>Версия:</span>
                    <span>3.2.18</span>
                </div>
                <div class="download-info-item">
                    <span>Размер файла:</span>
                    <span>95.3 МБ</span>
                </div>
                <div class="download-info-item">
                    <span>Система:</span>
                    <span>Windows 7/8/10/11</span>
                </div>
                <div class="download-info-item">
                    <span>Язык:</span>
                    <span>Русский</span>
                </div>
                <div class="download-info-item">
                    <span>Лицензия:</span>
                    <span>Бесплатно</span>
                </div>
            </div>
            
            <button class="btn btn-primary" id="final-download" style="background-color: white; color: #333; font-size: 1.2rem; padding: 16px 40px;">
                <i class="fas fa-download"></i> Скачать Яндекс.Диск для Windows
            </button>
            
            <p style="margin-top: 30px; font-size: 0.9rem; opacity: 0.8;">
                Установщик включает все необходимые компоненты. Работает на 32-битных и 64-битных системах Windows.
            </p>
        </div>
    </section>

    <!-- Related Apps -->
    <section class="related-apps">
        <div class="container">
            <div class="section-title">
                <h2>Другие программы от Яндекса</h2>
                <p>Расширьте возможности вашего компьютера</p>
            </div>
            
            <div class="apps-grid">
                <a href="https://loadbrowser.github.io/yandex-browser.html" class="app-card">
                    <div class="app-icon" style="background-color: #FF2E2E;">
                        <i class="fas fa-globe"></i>
                    </div>
                    <h3>Яндекс.Браузер</h3>
                    <p>Быстрый и безопасный браузер с интеграцией сервисов Яндекса</p>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard.html" class="app-card">
                    <div class="app-icon" style="background-color: #4CAF50;">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>AdGuard</h3>
                    <p>Лучший блокировщик рекламы для чистого интернета без трекеров</p>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard-vpn.html" class="app-card">
                    <div class="app-icon" style="background-color: #2196F3;">
                        <i class="fas fa-lock"></i>
                    </div>
                    <h3>AdGuard VPN</h3>
                    <p>Защитите свою приватность и обходите блокировки сайтов</p>
                </a>
                
                <a href="https://loadbrowser.github.io/" class="app-card">
                    <div class="app-icon" style="background-color: #9C27B0;">
                        <i class="fas fa-download"></i>
                    </div>
                    <h3>Все программы</h3>
                    <p>Перейти на главную страницу для загрузки других приложений</p>
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Яндекс.Диск для Windows</h3>
                    <p>Официальное облачное хранилище от Яндекса. Скачайте бесплатно и получите 10 ГБ для ваших файлов.</p>
                    <div style="margin-top: 20px; display: flex; gap: 15px;">
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-vk"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-telegram"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Навигация</h3>
                    <ul class="footer-links">
                        <li><a href="https://loadbrowser.github.io/">Главная страница</a></li>
                        <li><a href="https://loadbrowser.github.io/yandex-browser.html">Яндекс.Браузер</a></li>
                        <li><a href="https://loadbrowser.github.io/adguard.html">AdGuard</a></li>
                        <li><a href="https://loadbrowser.github.io/adguard-vpn.html">AdGuard VPN</a></li>
                        <li><a href="#download">Скачать Яндекс.Диск</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Полезные ссылки</h3>
                    <ul class="footer-links">
                        <li><a href="#">Инструкция по установке</a></li>
                        <li><a href="#">Настройки синхронизации</a></li>
                        <li><a href="#">Тарифы и цены</a></li>
                        <li><a href="#">Веб-версия Яндекс.Диска</a></li>
                        <li><a href="#">Поддержка</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Правовая информация</h3>
                    <ul class="footer-links">
                        <li><a href="#">Политика конфиденциальности</a></li>
                        <li><a href="#">Условия использования</a></li>
                        <li><a href="#">Лицензионное соглашение</a></li>
                        <li><a href="#">Контакты</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2023 Яндекс.Диск для Windows. Все права защищены.</p>
                <p style="margin-top: 10px;">Яндекс.Диск является продуктом компании Яндекс. Это демонстрационная страница для загрузки программы.</p>
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
        
        // Кнопки загрузки
        document.getElementById('main-download').addEventListener('click', function() {
            startDownload();
        });
        
        document.getElementById('header-download').addEventListener('click', function() {
            startDownload();
        });
        
        document.getElementById('final-download').addEventListener('click', function() {
            startDownload();
        });
        
        document.getElementById('web-version').addEventListener('click', function() {
            alert('Открывается веб-версия Яндекс.Диска.\n\nВы будете перенаправлены на сайт disk.yandex.ru');
        });
        
        function startDownload() {
            alert('Начинается загрузка Яндекс.Диска для Windows\n\nФайл: YandexDiskSetup.exe\nРазмер: 95.3 МБ\n\nФайл будет сохранен в папке "Загрузки".');
        }
        
        // Обновление года в футере
        document.querySelector('.footer-bottom p').innerHTML = `&copy; ${new Date().getFullYear()} Яндекс.Диск для Windows. Все права защищены.`;
        
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
        document.querySelectorAll('.feature-card, .guide-step, .requirement-card, .app-card').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            observer.observe(el);
        });
        
        // Подсветка ссылок в тексте при наведении
        document.querySelectorAll('a').forEach(link => {
            if (link.href.includes('loadbrowser.github.io') || link.href.includes('disk.yandex')) {
                link.addEventListener('mouseenter', function() {
                    this.style.textDecoration = 'underline';
                });
                link.addEventListener('mouseleave', function() {
                    this.style.textDecoration = 'none';
                });
            }
        });
        
        // Плавная прокрутка к якорям
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
        
        // Анимация прогресс-бара хранилища
        const storageFill = document.querySelector('.storage-fill');
        let width = 35;
        let direction = 1;
        
        setInterval(() => {
            if (width >= 40) direction = -1;
            if (width <= 30) direction = 1;
            
            width += 0.1 * direction;
            storageFill.style.width = width + '%';
            
            // Обновляем текст
            const usedGB = (width / 100 * 10).toFixed(1);
            const freeGB = (10 - usedGB).toFixed(1);
            
            document.querySelector('.storage-info span:first-child').textContent = `Использовано: ${usedGB} ГБ`;
            document.querySelector('.storage-info span:last-child').textContent = '10 ГБ';
            document.querySelector('.storage-info div:last-child').textContent = `Свободно: ${freeGB} ГБ`;
        }, 100);
    </script>
</body>
</html>
