---
layout: default
title: Яндекс.Браузер | Скачать Яндекс Браузер
description: Скачать Яндекс.Браузер бесплатно на русском языке..
---

<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Яндекс.Браузер — скачать бесплатно на Windows | Быстрый и безопасный</title>
    <meta name="description" content="Скачайте Яндекс.Браузер на Windows бесплатно. Официальный браузер от Яндекса с защитой, Турбо-режимом и интеграцией сервисов. Последняя версия 2024.">
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

        /* Hero Section */
        .hero {
            padding: 60px 0;
            background: linear-gradient(135deg, #FFF5F5 0%, #FFEBEE 100%);
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
            color: white;
        }

        .btn-primary:hover {
            background-color: var(--primary-dark);
            transform: translateY(-3px);
        }

        .btn-secondary {
            background-color: white;
            color: var(--primary-color);
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

        .browser-showcase {
            width: 100%;
            max-width: 500px;
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            overflow: hidden;
        }

        .browser-header {
            background-color: #f5f5f5;
            padding: 15px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 1px solid var(--light-gray);
        }

        .browser-controls {
            display: flex;
            gap: 8px;
        }

        .browser-control {
            width: 12px;
            height: 12px;
            border-radius: 50%;
        }

        .browser-control.red {
            background-color: #FF5F56;
        }

        .browser-control.yellow {
            background-color: #FFBD2E;
        }

        .browser-control.green {
            background-color: #27C93F;
        }

        .browser-url {
            flex: 1;
            margin: 0 15px;
            background-color: white;
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            color: var(--gray-color);
            text-align: center;
        }

        .browser-content {
            padding: 30px;
            text-align: center;
        }

        .browser-icon {
            width: 100px;
            height: 100px;
            background: linear-gradient(135deg, var(--primary-color), #FF6666);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 25px;
            position: relative;
        }

        .browser-icon::before {
            content: 'Я';
            font-size: 4rem;
            font-weight: 700;
            color: white;
            font-family: 'Arial', sans-serif;
        }

        .speed-indicator {
            background-color: #f9f9f9;
            border-radius: var(--border-radius);
            padding: 20px;
            margin-top: 25px;
        }

        .speed-bar {
            height: 10px;
            background-color: var(--light-gray);
            border-radius: 5px;
            margin: 15px 0;
            overflow: hidden;
            position: relative;
        }

        .speed-fill {
            height: 100%;
            width: 85%;
            background: linear-gradient(90deg, var(--primary-color), #FF6666);
            border-radius: 5px;
            position: relative;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { opacity: 1; }
            50% { opacity: 0.8; }
            100% { opacity: 1; }
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
            background-color: #FFF5F5;
            transform: translateY(-5px);
        }

        .feature-icon {
            width: 70px;
            height: 70px;
            background-color: rgba(255, 46, 46, 0.1);
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
            background-color: #FFF5F5;
        }

        .requirement-icon {
            width: 60px;
            height: 60px;
            background-color: rgba(255, 46, 46, 0.1);
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
            background: linear-gradient(135deg, var(--primary-color), #FF6666);
            text-align: center;
            color: white;
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

        .download-info {
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: var(--border-radius);
            padding: 25px;
            max-width: 500px;
            margin: 0 auto 40px;
            box-shadow: var(--box-shadow);
            color: #333;
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
                <i class="fas fa-globe"></i>
                <div class="logo-text">
                    Яндекс.Браузер
                    <span class="logo-subtitle">Скачать для Windows</span>
                </div>
            </a>
            
            <nav class="nav-links">
                <a href="https://loadbrowser.github.io/">Главная</a>
                <a href="https://loadbrowser.github.io/yandex-disk.html">Яндекс.Диск</a>
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
            <a href="https://loadbrowser.github.io/yandex-disk.html">Яндекс.Диск</a>
            <i class="fas fa-chevron-right"></i>
            <span>Яндекс.Браузер для Windows</span>
        </div>
    </section>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container hero-content">
            <div class="hero-text">
                <h1><span>Яндекс.Браузер</span> для Windows</h1>
                <p>Быстрый, безопасный и умный браузер от Яндекса. Скачайте последнюю версию для Windows с защитой, Турбо-режимом и интеграцией сервисов.</p>
                
                <div class="hero-badges">
                    <div class="badge">
                        <i class="fas fa-check"></i>
                        Защита Active Protect
                    </div>
                    <div class="badge">
                        <i class="fas fa-check"></i>
                        Турбо-режим
                    </div>
                    <div class="badge">
                        <i class="fas fa-check"></i>
                        Встроенный переводчик
                    </div>
                </div>
                
                <div class="hero-actions">
                    <button class="btn btn-primary" id="main-download">
                        <i class="fas fa-download"></i> Скачать Яндекс.Браузер
                    </button>
                    <button class="btn btn-secondary" id="portable-version">
                        <i class="fas fa-usb"></i> Portable версия
                    </button>
                </div>
                
                <div style="margin-top: 30px; display: flex; align-items: center; gap: 15px; flex-wrap: wrap;">
                    <div style="display: flex; align-items: center; gap: 8px;">
                        <i class="fas fa-check-circle" style="color: var(--success-color);"></i>
                        <span>Версия 23.11.1</span>
                    </div>
                    <div style="display: flex; align-items: center; gap: 8px;">
                        <i class="fas fa-hdd" style="color: var(--accent-color);"></i>
                        <span>Размер: 87.5 MB</span>
                    </div>
                    <div style="display: flex; align-items: center; gap: 8px;">
                        <i class="fas fa-star" style="color: var(--warning-color);"></i>
                        <span>4.7 ★ (15,239 оценок)</span>
                    </div>
                </div>
            </div>
            
            <div class="hero-image">
                <div class="browser-showcase">
                    <div class="browser-header">
                        <div class="browser-controls">
                            <div class="browser-control red"></div>
                            <div class="browser-control yellow"></div>
                            <div class="browser-control green"></div>
                        </div>
                        <div class="browser-url">yandex.ru • Защищено</div>
                        <div style="width: 40px;"></div>
                    </div>
                    <div class="browser-content">
                        <div class="browser-icon"></div>
                        <h3 style="margin-bottom: 10px;">Яндекс.Браузер</h3>
                        <p style="color: var(--gray-color); margin-bottom: 20px;">Быстрый и безопасный</p>
                        
                        <div class="speed-indicator">
                            <div style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                                <span>Скорость загрузки</span>
                                <span>85%</span>
                            </div>
                            <div class="speed-bar">
                                <div class="speed-fill"></div>
                            </div>
                            <div style="color: var(--gray-color); font-size: 0.9rem;">
                                Быстрее чем Chrome
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
                <h2>Возможности Яндекс.Браузера для Windows</h2>
                <p>Почему миллионы пользователей выбирают Яндекс.Браузер</p>
            </div>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-bolt"></i>
                    </div>
                    <h3>Турбо-режим</h3>
                    <p>Ускорение загрузки страниц при медленном интернете. Сжатие данных до 50% для экономии трафика.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>Защита Active Protect</h3>
                    <p>Блокировка опасных сайтов, проверка файлов на вирусы и защита от фишинговых атак.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-language"></i>
                    </div>
                    <h3>Встроенный переводчик</h3>
                    <p>Мгновенный перевод страниц на русский язык. Поддержка 90+ языков прямо в браузере.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-search"></i>
                    </div>
                    <h3>Умная строка</h3>
                    <p>Поиск, адреса сайтов и команды в одной строке. Умные подсказки и быстрый доступ.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-sync-alt"></i>
                    </div>
                    <h3>Синхронизация</h3>
                    <p>Закладки, история, пароли и настройки на всех ваших устройствах. Работает с Windows, macOS, iOS, Android.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-ad"></i>
                    </div>
                    <h3>Блокировка рекламы</h3>
                    <p>Встроенный блокировщик рекламы для чистого интернета без навязчивых объявлений.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Installation Guide -->
    <section class="installation">
        <div class="container">
            <div class="section-title">
                <h2>Как установить Яндекс.Браузер на Windows</h2>
                <p>Простая пошаговая инструкция по установке и настройке</p>
            </div>
            
            <div class="guide-steps">
                <!-- Step 1 -->
                <div class="guide-step">
                    <div class="step-number">1</div>
                    <div class="step-content">
                        <h3>Скачайте установщик</h3>
                        <p>Нажмите кнопку "Скачать Яндекс.Браузер" выше. Установочный файл будет загружен на ваш компьютер (размер около 88 МБ).</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1593640408182-31c70c8268f5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Скачивание Яндекс.Браузера">
                        </div>
                    </div>
                </div>
                
                <!-- Step 2 -->
                <div class="guide-step">
                    <div class="step-number">2</div>
                    <div class="step-content">
                        <h3>Запустите установщик</h3>
                        <p>Найдите скачанный файл <strong>YandexBrowserSetup.exe</strong> в папке "Загрузки" и запустите его двойным кликом.</p>
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
                        <p>После установки войдите в свой аккаунт Яндекс для синхронизации закладок, истории и паролей. Если аккаунта нет — создайте бесплатно.</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Вход в аккаунт">
                        </div>
                    </div>
                </div>
                
                <!-- Step 5 -->
                <div class="guide-step">
                    <div class="step-number">5</div>
                    <div class="step-content">
                        <h3>Настройте браузер под себя</h3>
                        <p>Выберите тему оформления, установите нужные расширения, настройте поисковую систему и параметры защиты.</p>
                        <div class="step-image">
                            <img src="https://images.unsplash.com/photo-1517077304055-6e89abbf09b0?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Настройка браузера">
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
                <p>Проверьте, подходит ли ваш компьютер для Яндекс.Браузера</p>
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
                    <p>Intel Pentium 4 или выше с поддержкой SSE2</p>
                </div>
                
                <div class="requirement-card">
                    <div class="requirement-icon">
                        <i class="fas fa-memory"></i>
                    </div>
                    <h3>Оперативная память</h3>
                    <p>512 МБ ОЗУ (рекомендуется 1 ГБ или больше)</p>
                </div>
                
                <div class="requirement-card">
                    <div class="requirement-icon">
                        <i class="fas fa-hdd"></i>
                    </div>
                    <h3>Свободное место</h3>
                    <p>400 МБ на жестком диске для установки</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Comparison Section -->
    <section class="comparison">
        <div class="container">
            <div class="section-title">
                <h2>Сравнение с другими браузерами для Windows</h2>
                <p>Почему Яндекс.Браузер — лучший выбор</p>
            </div>
            
            <table class="comparison-table">
                <thead>
                    <tr>
                        <th>Функция</th>
                        <th>Яндекс.Браузер</th>
                        <th>Google Chrome</th>
                        <th>Microsoft Edge</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td class="feature-name">Встроенный переводчик</td>
                        <td class="check">Да</td>
                        <td class="check">Требует расширение</td>
                        <td class="check">Да</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Турбо-режим</td>
                        <td class="check">Да</td>
                        <td class="partial">Нет</td>
                        <td class="partial">Есть экономия трафика</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Защита Active Protect</td>
                        <td class="check">Да</td>
                        <td class="check">Safe Browsing</td>
                        <td class="check">Microsoft Defender</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Встроенный блокировщик рекламы</td>
                        <td class="check">Да</td>
                        <td class="partial">Требует расширение</td>
                        <td class="partial">Базовый</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Интеграция с Яндекс.Диском</td>
                        <td class="check">Полная</td>
                        <td class="partial">Через расширение</td>
                        <td class="partial">Через расширение</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Потребление памяти</td>
                        <td class="check">Оптимизировано</td>
                        <td class="partial">Высокое</td>
                        <td class="check">Оптимизировано</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Русская техподдержка</td>
                        <td class="check">Круглосуточно</td>
                        <td class="partial">Ограниченная</td>
                        <td class="partial">Ограниченная</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <!-- FAQ Section -->
    <section class="faq">
        <div class="container">
            <div class="section-title">
                <h2>Частые вопросы о Яндекс.Браузере</h2>
                <p>Ответы на самые популярные вопросы пользователей</p>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Чем Яндекс.Браузер лучше Chrome для Windows?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Яндекс.Браузер предлагает несколько преимуществ перед Chrome: встроенный переводчик, Турбо-режим для медленного интернета, лучшая интеграция с российскими сервисами, оптимизированное потребление памяти и круглосуточная русскоязычная поддержка.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Можно ли установить расширения Chrome в Яндекс.Браузер?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, Яндекс.Браузер основан на Chromium и полностью совместим с расширениями из Chrome Web Store. Вы можете устанавливать любые расширения, которые работают в Chrome.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Работает ли Яндекс.Браузер с Яндекс.Диском?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, Яндекс.Браузер имеет глубокую интеграцию с <a href="https://loadbrowser.github.io/yandex-disk.html" style="color: var(--primary-color); font-weight: 600;">Яндекс.Диском</a>. Вы можете сохранять файлы прямо в облако, открывать документы онлайн и делиться ссылками через контекстное меню браузера.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Нужен ли AdGuard с Яндекс.Браузером?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Яндекс.Браузер имеет встроенный блокировщик рекламы, но <a href="https://loadbrowser.github.io/adguard.html" style="color: var(--primary-color); font-weight: 600;">AdGuard</a> предлагает более продвинутые функции: защиту от трекеров, фишинга и улучшенную блокировку. Вы можете использовать оба для максимальной защиты.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Можно ли синхронизировать Яндекс.Браузер с телефоном?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, при входе в аккаунт Яндекс ваши закладки, история, пароли и настройки синхронизируются между всеми устройствами: Windows, macOS, iOS и Android. Это работает автоматически и бесплатно.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Download Section -->
    <section class="download-section" id="download">
        <div class="container">
            <h2>Скачайте Яндекс.Браузер для Windows</h2>
            <p>Установите официальный браузер от Яндекса и получите все преимущества быстрого и безопасного интернета</p>
            
            <div class="download-info">
                <div class="download-info-item">
                    <span>Версия:</span>
                    <span>23.11.1</span>
                </div>
                <div class="download-info-item">
                    <span>Размер файла:</span>
                    <span>87.5 МБ</span>
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
            
            <button class="btn btn-primary" id="final-download" style="background-color: white; color: var(--primary-color); font-size: 1.2rem; padding: 16px 40px;">
                <i class="fas fa-download"></i> Скачать Яндекс.Браузер для Windows
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
                <h2>Совместимые программы для Windows</h2>
                <p>Расширьте возможности вашего компьютера</p>
            </div>
            
            <div class="apps-grid">
                <a href="https://loadbrowser.github.io/yandex-disk.html" class="app-card">
                    <div class="app-icon" style="background-color: #FFCC00;">
                        <i class="fas fa-cloud"></i>
                    </div>
                    <h3>Яндекс.Диск</h3>
                    <p>Облачное хранилище для синхронизации файлов с Яндекс.Браузером</p>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard.html" class="app-card">
                    <div class="app-icon" style="background-color: #4CAF50;">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>AdGuard</h3>
                    <p>Продвинутый блокировщик рекламы для полной защиты в интернете</p>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard-vpn.html" class="app-card">
                    <div class="app-icon" style="background-color: #2196F3;">
                        <i class="fas fa-lock"></i>
                    </div>
                    <h3>AdGuard VPN</h3>
                    <p>Защитите свою приватность в Яндекс.Браузере и обходите блокировки</p>
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
                    <h3>Яндекс.Браузер для Windows</h3>
                    <p>Официальный браузер от Яндекса. Скачайте бесплатно и получите быстрый, безопасный и умный браузер для Windows.</p>
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
                        <li><a href="https://loadbrowser.github.io/yandex-disk.html">Яндекс.Диск</a></li>
                        <li><a href="https://loadbrowser.github.io/adguard.html">AdGuard</a></li>
                        <li><a href="https://loadbrowser.github.io/adguard-vpn.html">AdGuard VPN</a></li>
                        <li><a href="#download">Скачать Яндекс.Браузер</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Полезные ссылки</h3>
                    <ul class="footer-links">
                        <li><a href="#">Инструкция по установке</a></li>
                        <li><a href="#">Настройки браузера</a></li>
                        <li><a href="#">Расширения для Яндекс.Браузера</a></li>
                        <li><a href="#">Включить Турбо-режим</a></li>
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
                <p>&copy; 2023 Яндекс.Браузер для Windows. Все права защищены.</p>
                <p style="margin-top: 10px;">Яндекс.Браузер является продуктом компании Яндекс. Это демонстрационная страница для загрузки программы.</p>
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
        
        document.getElementById('portable-version').addEventListener('click', function() {
            alert('Portable версия Яндекс.Браузера\n\nЭта версия не требует установки и может работать с USB-флешки.\nРазмер: 92 МБ');
        });
        
        function startDownload() {
            alert('Начинается загрузка Яндекс.Браузера для Windows\n\nФайл: YandexBrowserSetup.exe\nРазмер: 87.5 МБ\n\nФайл будет сохранен в папке "Загрузки".');
        }
        
        // Обновление года в футере
        document.querySelector('.footer-bottom p').innerHTML = `&copy; ${new Date().getFullYear()} Яндекс.Браузер для Windows. Все права защищены.`;
        
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
        
        // Анимация скорости загрузки
        const speedFill = document.querySelector('.speed-fill');
        let speedWidth = 85;
        let speedDirection = 1;
        
        setInterval(() => {
            if (speedWidth >= 90) speedDirection = -1;
            if (speedWidth <= 80) speedDirection = 1;
            
            speedWidth += 0.05 * speedDirection;
            speedFill.style.width = speedWidth + '%';
            
            // Обновляем текст
            document.querySelector('.speed-indicator span:last-child').textContent = Math.round(speedWidth) + '%';
        }, 100);
    </script>
</body>
</html>
