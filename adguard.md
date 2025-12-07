---
layout: default
title: AdGuard для Яндекс Браузера | Скачать
description: Скачайте AdGuard для Яндекс Браузера на Windows для блокировки рекламы и защиты от угроз.
---

<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AdGuard VPN для Яндекс.Браузера - Установка и настройка</title>
    <meta name="description" content="Установите AdGuard VPN для Яндекс.Браузера. Полная защита приватности, обход блокировок и безопасный серфинг. Скачайте расширение бесплатно.">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #4CAF50;
            --primary-dark: #388E3C;
            --secondary-color: #66BB6A;
            --accent-color: #FF9800;
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

        /* Hero Section */
        .hero {
            padding: 60px 0;
            background: linear-gradient(135deg, #E8F5E9 0%, #F1F8E9 100%);
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

        .hero-browser {
            width: 100%;
            max-width: 500px;
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            overflow: hidden;
            position: relative;
        }

        .browser-header {
            background-color: #f5f5f5;
            padding: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
            border-bottom: 1px solid var(--light-gray);
        }

        .browser-dots {
            display: flex;
            gap: 8px;
        }

        .browser-dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
        }

        .browser-dot.red {
            background-color: #FF5F56;
        }

        .browser-dot.yellow {
            background-color: #FFBD2E;
        }

        .browser-dot.green {
            background-color: #27C93F;
        }

        .browser-url {
            flex: 1;
            background-color: white;
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            color: var(--gray-color);
        }

        .browser-content {
            padding: 30px;
            text-align: center;
        }

        .browser-icon {
            width: 80px;
            height: 80px;
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
        }

        .browser-icon i {
            font-size: 2.5rem;
            color: white;
        }

        /* Benefits Section */
        .benefits {
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

        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .benefit-card {
            background-color: #f9f9f9;
            border-radius: var(--border-radius);
            padding: 30px;
            text-align: center;
            transition: var(--transition);
        }

        .benefit-card:hover {
            background-color: #E8F5E9;
            transform: translateY(-5px);
        }

        .benefit-icon {
            width: 70px;
            height: 70px;
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
        }

        .benefit-icon i {
            font-size: 2rem;
            color: white;
        }

        /* Setup Guide */
        .setup-guide {
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
            color: white;
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

        .code-block {
            background-color: #2d2d2d;
            color: #f8f8f2;
            padding: 20px;
            border-radius: var(--border-radius);
            font-family: 'Courier New', monospace;
            margin-top: 15px;
            overflow-x: auto;
        }

        /* Features */
        .features {
            padding: 80px 0;
            background-color: white;
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
            background-color: #E8F5E9;
            transform: translateY(-3px);
        }

        .feature-icon {
            width: 60px;
            height: 60px;
            background-color: rgba(76, 175, 80, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
        }

        .feature-icon i {
            font-size: 1.8rem;
            color: var(--primary-color);
        }

        .feature-card h3 {
            font-size: 1.3rem;
            margin-bottom: 15px;
            color: var(--dark-color);
        }

        /* Comparison */
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

        .comparison-table .cross {
            color: #f44336;
        }

        /* FAQ */
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
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            text-align: center;
        }

        .download-section h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }

        .download-section p {
            font-size: 1.2rem;
            margin-bottom: 40px;
            opacity: 0.9;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }

        .download-options {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .download-option {
            background-color: white;
            color: var(--primary-color);
            padding: 20px 30px;
            border-radius: var(--border-radius);
            font-weight: 600;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 10px;
            transition: var(--transition);
        }

        .download-option:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
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
            
            .download-options {
                flex-direction: column;
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
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="https://loadbrowser.github.io/" class="logo">
                <i class="fas fa-shield-alt"></i>
                <div class="logo-text">
                    AdGuard VPN
                    <span class="logo-subtitle">Для Яндекс.Браузера</span>
                </div>
            </a>
            
            <nav class="nav-links">
                <a href="https://loadbrowser.github.io/">Главная</a>
                <a href="https://loadbrowser.github.io/yandex-browser.html" class="active">Яндекс.Браузер</a>
                <a href="https://loadbrowser.github.io/adguard.html">AdGuard</a>
                <a href="https://loadbrowser.github.io/adguard-vpn.html">AdGuard VPN</a>
                <a href="#download">Скачать</a>
            </nav>
            
            <div class="header-actions">
                <button class="download-btn">
                    <i class="fas fa-download"></i>
                    Скачать VPN
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
            <a href="https://loadbrowser.github.io/adguard-vpn.html">AdGuard VPN</a>
            <i class="fas fa-chevron-right"></i>
            <span>Для Яндекс.Браузера</span>
        </div>
    </section>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container hero-content">
            <div class="hero-text">
                <h1>AdGuard VPN для <span>Яндекс.Браузера</span></h1>
                <p>Защитите свой Яндекс.Браузер с помощью AdGuard VPN. Полная анонимность, обход блокировок и безопасный серфинг в один клик.</p>
                
                <div class="app-header-actions">
                    <button class="btn btn-primary" id="download-extension">
                        <i class="fas fa-puzzle-piece"></i> Установить расширение
                    </button>
                    <button class="btn btn-secondary" id="download-desktop">
                        <i class="fas fa-desktop"></i> Полная версия
                    </button>
                </div>
                
                <div style="margin-top: 30px; display: flex; gap: 20px; flex-wrap: wrap;">
                    <div style="display: flex; align-items: center; gap: 10px;">
                        <i class="fas fa-check" style="color: var(--success-color);"></i>
                        <span>Бесплатный тариф</span>
                    </div>
                    <div style="display: flex; align-items: center; gap: 10px;">
                        <i class="fas fa-check" style="color: var(--success-color);"></i>
                        <span>Интеграция с Яндекс.Браузером</span>
                    </div>
                    <div style="display: flex; align-items: center; gap: 10px;">
                        <i class="fas fa-check" style="color: var(--success-color);"></i>
                        <span>Защита от отслеживания</span>
                    </div>
                </div>
            </div>
            
            <div class="hero-image">
                <div class="hero-browser">
                    <div class="browser-header">
                        <div class="browser-dots">
                            <div class="browser-dot red"></div>
                            <div class="browser-dot yellow"></div>
                            <div class="browser-dot green"></div>
                        </div>
                        <div class="browser-url">yandex.ru • AdGuard VPN активен</div>
                    </div>
                    <div class="browser-content">
                        <div class="browser-icon">
                            <i class="fas fa-shield-alt"></i>
                        </div>
                        <h3 style="margin-bottom: 10px;">AdGuard VPN активен</h3>
                        <p style="color: var(--gray-color); margin-bottom: 20px;">Ваше соединение защищено</p>
                        <div style="display: inline-block; background-color: var(--success-color); color: white; padding: 8px 20px; border-radius: 20px; font-weight: 600;">
                            Подключено
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Benefits Section -->
    <section class="benefits">
        <div class="container">
            <div class="section-title">
                <h2>Преимущества AdGuard VPN для Яндекс.Браузера</h2>
                <p>Почему стоит использовать AdGuard VPN именно в Яндекс.Браузере</p>
            </div>
            
            <div class="benefits-grid">
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-bolt"></i>
                    </div>
                    <h3>Высокая скорость</h3>
                    <p>Оптимизированная работа с Яндекс.Браузером без потери скорости соединения.</p>
                </div>
                
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-lock"></i>
                    </div>
                    <h3>Полная интеграция</h3>
                    <p>Глубокая интеграция с Яндекс.Браузером, включая умную строку и настройки.</p>
                </div>
                
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>Двойная защита</h3>
                    <p>Защита встроенного блокировщика Яндекс.Браузера + AdGuard VPN.</p>
                </div>
                
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-sync-alt"></i>
                    </div>
                    <h3>Автоподключение</h3>
                    <p>Автоматическое подключение к VPN при запуске Яндекс.Браузера.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Setup Guide -->
    <section class="setup-guide">
        <div class="container">
            <div class="section-title">
                <h2>Как установить AdGuard VPN в Яндекс.Браузер</h2>
                <p>Пошаговая инструкция по установке и настройке расширения</p>
            </div>
            
            <div class="guide-steps">
                <!-- Step 1 -->
                <div class="guide-step">
                    <div class="step-number">1</div>
                    <div class="step-content">
                        <h3>Откройте Яндекс.Браузер</h3>
                        <p>Запустите Яндекс.Браузер на вашем компьютере. Убедитесь, что у вас установлена последняя версия браузера.</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Яндекс.Браузер">
                        </div>
                    </div>
                </div>
                
                <!-- Step 2 -->
                <div class="guide-step">
                    <div class="step-number">2</div>
                    <div class="step-content">
                        <h3>Перейдите в магазин расширений</h3>
                        <p>В адресной строке введите <code>chrome://extensions/</code> и нажмите Enter. Или откройте меню браузера → Дополнения → Каталог расширений.</p>
                        <div class="code-block">
                            chrome://extensions/
                        </div>
                    </div>
                </div>
                
                <!-- Step 3 -->
                <div class="guide-step">
                    <div class="step-number">3</div>
                    <div class="step-content">
                        <h3>Найдите AdGuard VPN</h3>
                        <p>В поиске магазина расширений введите "AdGuard VPN" и нажмите Enter. Найдите официальное расширение от AdGuard.</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1611224923853-80b023f02d71?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Поиск расширения">
                        </div>
                    </div>
                </div>
                
                <!-- Step 4 -->
                <div class="guide-step">
                    <div class="step-number">4</div>
                    <div class="step-content">
                        <h3>Установите расширение</h3>
                        <p>Нажмите кнопку "Установить" на странице расширения AdGuard VPN. Подтвердите установку во всплывающем окне.</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1581276879432-15e50529f34b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Установка расширения">
                        </div>
                    </div>
                </div>
                
                <!-- Step 5 -->
                <div class="guide-step">
                    <div class="step-number">5</div>
                    <div class="step-content">
                        <h3>Настройте и используйте</h3>
                        <p>После установки нажмите на иконку AdGuard VPN в панели расширений, создайте аккаунт и подключитесь к VPN.</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1558494949-ef010cbdcc31?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Настройка VPN">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Features -->
    <section class="features">
        <div class="container">
            <div class="section-title">
                <h2>Особенности расширения AdGuard VPN</h2>
                <p>Все возможности VPN, оптимизированные для Яндекс.Браузера</p>
            </div>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-globe"></i>
                    </div>
                    <h3>Выбор серверов</h3>
                    <p>Доступ к серверам в 50+ странах с оптимизацией для российских пользователей.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-user-shield"></i>
                    </div>
                    <h3>Режим невидимки</h3>
                    <p>Скрытие вашего реального IP-адреса и местоположения от сайтов и трекеров.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-list"></i>
                    </div>
                    <h3>Исключения</h3>
                    <p>Настройка списка сайтов, для которых VPN не будет использоваться.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-tachometer-alt"></i>
                    </div>
                    <h3>Автовыбор сервера</h3>
                    <p>Автоматический выбор самого быстрого сервера для вашего местоположения.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-wifi"></i>
                    </div>
                    <h3>Защита Wi-Fi</h3>
                    <p>Автоматическое включение VPN при подключении к публичным сетям Wi-Fi.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-bell"></i>
                    </div>
                    <h3>Уведомления</h3>
                    <p>Оповещения о статусе VPN-соединения прямо в Яндекс.Браузере.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Comparison -->
    <section class="comparison">
        <div class="container">
            <div class="section-title">
                <h2>Сравнение с другими VPN для Яндекс.Браузера</h2>
                <p>Почему AdGuard VPN - лучший выбор для Яндекс.Браузера</p>
            </div>
            
            <table class="comparison-table">
                <thead>
                    <tr>
                        <th>Функция</th>
                        <th>AdGuard VPN</th>
                        <th>Hola VPN</th>
                        <th>Windscribe</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td class="feature-name">Бесплатный трафик</td>
                        <td class="check">3 ГБ/месяц</td>
                        <td class="check">Неограниченно</td>
                        <td class="check">10 ГБ/месяц</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Интеграция с Яндекс.Браузером</td>
                        <td class="check">Полная</td>
                        <td class="cross">Частичная</td>
                        <td class="cross">Частичная</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Совместимость с AdGuard</td>
                        <td class="check">Да</td>
                        <td class="cross">Нет</td>
                        <td class="check">Да</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Русский интерфейс</td>
                        <td class="check">Да</td>
                        <td class="check">Да</td>
                        <td class="cross">Нет</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Серверы в России</td>
                        <td class="check">Да</td>
                        <td class="check">Да</td>
                        <td class="cross">Нет</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Безлоговый режим</td>
                        <td class="check">Да</td>
                        <td class="cross">Нет</td>
                        <td class="check">Да</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Поддержка WireGuard</td>
                        <td class="check">Да</td>
                        <td class="cross">Нет</td>
                        <td class="check">Да</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <!-- FAQ -->
    <section class="faq">
        <div class="container">
            <div class="section-title">
                <h2>Частые вопросы об AdGuard VPN</h2>
                <p>Ответы на самые популярные вопросы пользователей</p>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>AdGuard VPN бесплатный для Яндекс.Браузера?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, AdGuard VPN предлагает бесплатный тариф с ограничением 3 ГБ трафика в месяц. Этого достаточно для безопасного серфинга и доступа к заблокированным сайтам. Для неограниченного трафика и доступа ко всем серверам доступен платный тариф.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Можно ли использовать AdGuard VPN вместе с AdGuard для Яндекс.Браузера?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, AdGuard VPN и <a href="https://loadbrowser.github.io/adguard.html" style="color: var(--primary-color); font-weight: 600;">AdGuard</a> отлично работают вместе в Яндекс.Браузере. AdGuard блокирует рекламу и трекеры, а AdGuard VPN обеспечивает анонимность и обход блокировок. Рекомендуется использовать оба расширения для максимальной защиты.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Замедляет ли AdGuard VPN работу Яндекс.Браузера?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>AdGuard VPN оптимизирован для работы с Яндекс.Браузером и практически не влияет на скорость загрузки страниц. На некоторых серверах может наблюдаться незначительное снижение скорости, но для большинства задач (серфинг, видео, мессенджеры) это незаметно.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Нужно ли отключать встроенную защиту Яндекс.Браузера при использовании AdGuard VPN?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Нет, AdGuard VPN работает независимо от встроенных систем защиты <a href="https://loadbrowser.github.io/yandex-browser.html" style="color: var(--primary-color); font-weight: 600;">Яндекс.Браузера</a>. Вы можете использовать их одновременно для многоуровневой защиты. Встроенный блокировщик рекламы Яндекс.Браузера и AdGuard VPN дополняют друг друга.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Как отключить AdGuard VPN для определенных сайтов?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>В настройках расширения AdGuard VPN есть раздел "Исключения". Вы можете добавить туда сайты, для которых VPN не должен использоваться. Это полезно для сайтов, которые требуют ваш реальный IP-адрес (например, онлайн-банкинг или некоторые государственные сервисы).</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Download Section -->
    <section class="download-section" id="download">
        <div class="container">
            <h2>Установите AdGuard VPN для Яндекс.Браузера</h2>
            <p>Защитите свой Яндекс.Браузер в один клик. Бесплатный тариф с 3 ГБ трафика в месяц.</p>
            
            <div class="download-options">
                <a href="#" class="download-option" id="install-chrome-store">
                    <i class="fab fa-chrome"></i>
                    <span>Установить из Chrome Web Store</span>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard-vpn.html" class="download-option" id="full-version">
                    <i class="fas fa-desktop"></i>
                    <span>Полная версия AdGuard VPN</span>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard.html" class="download-option" id="adguard-only">
                    <i class="fas fa-shield-alt"></i>
                    <span>Только AdGuard (без VPN)</span>
                </a>
            </div>
            
            <p style="margin-top: 30px; font-size: 0.9rem; opacity: 0.8;">
                Расширение совместимо с Яндекс.Браузером версии 23.0 и выше
            </p>
        </div>
    </section>

    <!-- Related Apps -->
    <section class="related-apps">
        <div class="container">
            <div class="section-title">
                <h2>Другие полезные программы</h2>
                <p>Расширьте возможности вашего Яндекс.Браузера</p>
            </div>
            
            <div class="apps-grid">
                <a href="https://loadbrowser.github.io/yandex-browser.html" class="app-card">
                    <div class="app-icon" style="background-color: #FF2E2E;">
                        <i class="fas fa-globe"></i>
                    </div>
                    <h3>Яндекс.Браузер</h3>
                    <p>Скачайте последнюю версию быстрого и безопасного браузера от Яндекса</p>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard.html" class="app-card">
                    <div class="app-icon" style="background-color: #4CAF50;">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>AdGuard</h3>
                    <p>Мощный блокировщик рекламы для чистого интернета без трекеров</p>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard-vpn.html" class="app-card">
                    <div class="app-icon" style="background-color: #2196F3;">
                        <i class="fas fa-lock"></i>
                    </div>
                    <h3>AdGuard VPN</h3>
                    <p>Полнофункциональный VPN-клиент для всех устройств и браузеров</p>
                </a>
                
                <a href="https://loadbrowser.github.io/yandex-disk.html" class="app-card">
                    <div class="app-icon" style="background-color: #FFCC00;">
                        <i class="fas fa-cloud"></i>
                    </div>
                    <h3>Яндекс.Диск</h3>
                    <p>Облачное хранилище для ваших файлов с защитой через VPN</p>
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>AdGuard VPN для Яндекс.Браузера</h3>
                    <p>Официальное расширение AdGuard VPN для Яндекс.Браузера. Защита приватности и обход блокировок в один клик.</p>
                    <div style="margin-top: 20px; display: flex; gap: 15px;">
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-telegram"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-vk"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-github"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Навигация</h3>
                    <ul class="footer-links">
                        <li><a href="https://loadbrowser.github.io/">Главная страница</a></li>
                        <li><a href="https://loadbrowser.github.io/yandex-browser.html">Яндекс.Браузер</a></li>
                        <li><a href="https://loadbrowser.github.io/adguard.html">AdGuard</a></li>
                        <li><a href="https://loadbrowser.github.io/adguard-vpn.html">AdGuard VPN</a></li>
                        <li><a href="#download">Скачать расширение</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Полезные ссылки</h3>
                    <ul class="footer-links">
                        <li><a href="#">Инструкция по установке</a></li>
                        <li><a href="#">Настройки VPN</a></li>
                        <li><a href="#">Список серверов</a></li>
                        <li><a href="#">Бесплатный тариф</a></li>
                        <li><a href="#">Поддержка</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Правовая информация</h3>
                    <ul class="footer-links">
                        <li><a href="#">Политика конфиденциальности</a></li>
                        <li><a href="#">Условия использования</a></li>
                        <li><a href="#">DMCA</a></li>
                        <li><a href="#">Контакты</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2023 AdGuard VPN для Яндекс.Браузера. Все права защищены.</p>
                <p style="margin-top: 10px;">Это демонстрационная страница. AdGuard VPN является продуктом компании AdGuard Software Ltd.</p>
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
        document.getElementById('download-extension').addEventListener('click', function() {
            alert('Открывается Chrome Web Store для установки AdGuard VPN расширения.\n\nНажмите "Установить" на странице расширения.');
        });
        
        document.getElementById('download-desktop').addEventListener('click', function() {
            alert('Открывается страница загрузки полной версии AdGuard VPN.\n\nВы будете перенаправлены на официальный сайт AdGuard.');
        });
        
        document.getElementById('install-chrome-store').addEventListener('click', function(e) {
            e.preventDefault();
            alert('Открывается Chrome Web Store для установки AdGuard VPN расширения для Яндекс.Браузера.\n\nНажмите "Установить" на странице расширения.');
        });
        
        document.querySelector('.download-btn').addEventListener('click', function() {
            alert('Скачивание AdGuard VPN для Яндекс.Браузера\n\nВыберите способ установки: расширение из Chrome Web Store или полная версия.');
        });
        
        // Обновление года в футере
        document.querySelector('.footer-bottom p').innerHTML = `&copy; ${new Date().getFullYear()} AdGuard VPN для Яндекс.Браузера. Все права защищены.`;
        
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
        document.querySelectorAll('.benefit-card, .guide-step, .feature-card, .app-card').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            observer.observe(el);
        });
        
        // Подсветка ссылок в тексте при наведении
        document.querySelectorAll('a').forEach(link => {
            if (link.href.includes('loadbrowser.github.io')) {
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
        
        // Имитация переключения состояния VPN в браузере
        const vpnStatus = document.querySelector('.browser-content div:last-child');
        let vpnConnected = true;
        
        vpnStatus.addEventListener('click', function() {
            if (vpnConnected) {
                this.textContent = 'Отключено';
                this.style.backgroundColor = '#f44336';
                this.parentElement.querySelector('h3').textContent = 'AdGuard VPN отключен';
                this.parentElement.querySelector('p').textContent = 'Ваше соединение не защищено';
            } else {
                this.textContent = 'Подключено';
                this.style.backgroundColor = '#4CAF50';
                this.parentElement.querySelector('h3').textContent = 'AdGuard VPN активен';
                this.parentElement.querySelector('p').textContent = 'Ваше соединение защищено';
            }
            vpnConnected = !vpnConnected;
        });
    </script>
</body>
</html>
