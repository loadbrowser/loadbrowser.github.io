---
layout: default
title: HideMyName VPN для Яндекс Браузера | Скрыть IP и безопасный серфинг
description: Узнайте, как установить HideMyName VPN в Яндекс Браузере для защиты данных, обхода блокировок и приватного просмотра сайтов.
---

<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HideMyName VPN - Скачать бесплатный VPN для Windows, Android, iOS</title>
    <meta name="description" content="Скачайте HideMyName VPN бесплатно - мощный VPN сервис для анонимного серфинга, обхода блокировок и защиты данных. Совместим с Яндекс.Браузером, AdGuard и другими программами.">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #4A00E0;
            --primary-dark: #3A00B0;
            --secondary-color: #8E2DE2;
            --accent-color: #00C9FF;
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
            background: linear-gradient(135deg, #F3F0FF 0%, #EDE7FF 100%);
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
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: var(--box-shadow);
            position: relative;
            overflow: hidden;
        }

        .app-icon-large i {
            font-size: 4rem;
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
            background-color: #00B8E6;
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
            background-color: #F3F0FF;
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
            background-color: #F3F0FF;
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

        .comparison-table .vpn-check {
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

        /* VPN Advantages */
        .vpn-advantages {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 30px;
            margin-top: 40px;
            box-shadow: var(--box-shadow);
        }

        .advantages-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }

        .advantage-card {
            background-color: #f9f9f9;
            border-radius: var(--border-radius);
            padding: 25px;
            text-align: center;
            transition: var(--transition);
        }

        .advantage-card:hover {
            background-color: #F3F0FF;
            transform: translateY(-5px);
        }

        .advantage-icon {
            width: 70px;
            height: 70px;
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
        }

        .advantage-icon i {
            font-size: 2rem;
            color: white;
        }

        /* Compatibility Section */
        .compatibility-section {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 30px;
            margin-top: 40px;
            box-shadow: var(--box-shadow);
        }

        .compatibility-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 25px;
        }

        .compatibility-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
            background-color: #f9f9f9;
            border-radius: var(--border-radius);
            transition: var(--transition);
        }

        .compatibility-item:hover {
            background-color: #F3F0FF;
            transform: translateY(-3px);
        }

        .compatibility-icon {
            width: 60px;
            height: 60px;
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 15px;
        }

        .compatibility-icon i {
            font-size: 1.8rem;
            color: white;
        }

        /* FAQ Section */
        .faq-section {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 30px;
            margin-top: 40px;
            box-shadow: var(--box-shadow);
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

        /* Navigation Cards */
        .navigation-cards {
            margin-top: 40px;
        }

        .nav-cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .nav-card {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            border-radius: var(--border-radius);
            padding: 30px;
            color: white;
            text-decoration: none;
            transition: var(--transition);
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }

        .nav-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(74, 0, 224, 0.2);
        }

        .nav-card i {
            font-size: 2.5rem;
            margin-bottom: 15px;
        }

        .nav-card h3 {
            font-size: 1.4rem;
            margin-bottom: 10px;
        }

        .nav-card p {
            opacity: 0.9;
            font-size: 0.95rem;
        }

        .nav-card.secondary {
            background: linear-gradient(135deg, #FF2E2E, #FF6666);
        }

        .nav-card.success {
            background: linear-gradient(135deg, #4CAF50, #66BB6A);
        }

        .nav-card.info {
            background: linear-gradient(135deg, #2196F3, #42A5F5);
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
            
            .advantages-grid, .compatibility-grid, .nav-cards-grid {
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
            
            .advantages-grid, .compatibility-grid, .nav-cards-grid {
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
                font-size: 3rem;
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
                    HideMyName VPN
                    <span class="logo-subtitle">Анонимность и безопасность</span>
                </div>
            </a>
            
            <nav class="nav-links">
                <a href="https://loadbrowser.github.io/">Главная</a>
                <a href="https://loadbrowser.github.io/yandex-browser.html" class="active">Яндекс.Браузер</a>
                <a href="https://loadbrowser.github.io/yandex-disk.html">Яндекс.Диск</a>
                <a href="https://loadbrowser.github.io/adguard.html">AdGuard</a>
                <a href="#download">Скачать VPN</a>
            </nav>
            
            <div class="header-actions">
                <button class="download-btn" id="main-download">
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
            <a href="https://loadbrowser.github.io/adguard.html">AdGuard</a>
            <i class="fas fa-chevron-right"></i>
            <span>HideMyName VPN</span>
        </div>
    </section>

    <!-- App Detail Header -->
    <section class="app-detail-header">
        <div class="container">
            <div class="app-header-content">
                <div class="app-icon-large">
                    <i class="fas fa-user-secret"></i>
                </div>
                <div class="app-header-info">
                    <h1 class="app-title"><span>HideMyName VPN</span> — анонимность в один клик</h1>
                    <div class="app-meta">
                        <span class="app-version">Версия 3.2.1</span>
                        <div class="app-rating">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star-half-alt"></i>
                            <span>4.7 (8,452 оценок)</span>
                        </div>
                        <span class="app-size">Размер: 52.8 MB</span>
                    </div>
                    <p>Мощный VPN-сервис для защиты вашей приватности, обхода блокировок и безопасного серфинга в интернете. Совместим с Яндекс.Браузером, AdGuard и другими программами.</p>
                    <div class="app-header-actions">
                        <button class="btn btn-primary" id="download-windows">
                            <i class="fas fa-download"></i> Скачать для Windows
                        </button>
                        <button class="btn btn-accent" id="download-android">
                            <i class="fab fa-android"></i> Версия для Android
                        </button>
                        <button class="btn btn-secondary" id="download-ios">
                            <i class="fab fa-apple"></i> Версия для iOS
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
            <h2 class="section-title">О HideMyName VPN</h2>
            <div class="app-description">
                <p><strong>HideMyName VPN</strong> — это современный VPN-сервис, который обеспечивает полную анонимность и безопасность в интернете. С помощью нашего сервиса вы сможете скрыть свой реальный IP-адрес, обойти географические ограничения и защитить свои данные от хакеров и слежки.</p>
                
                <div class="highlight">
                    <p><strong>Совместимость с другими программами:</strong> HideMyName VPN отлично работает вместе с <a href="https://loadbrowser.github.io/yandex-browser.html" style="color: var(--primary-color); font-weight: 600;">Яндекс.Браузером</a>, <a href="https://loadbrowser.github.io/adguard.html" style="color: var(--primary-color); font-weight: 600;">AdGuard</a> и другими популярными приложениями. Вы можете использовать VPN совместно с блокировщиком рекламы для максимальной защиты.</p>
                </div>
                
                <p>Сервис использует современные протоколы шифрования (OpenVPN, IKEv2, WireGuard) и не ведет логов вашей активности. Приложение имеет простой и интуитивно понятный интерфейс — подключение к VPN происходит в один клик.</p>
            </div>
            
            <div class="app-features">
                <h2 class="section-title">Ключевые возможности</h2>
                <ul>
                    <li><i class="fas fa-check"></i> <strong>Бесплатный тариф</strong> — 10 Мбит/с, 20+ серверов</li>
                    <li><i class="fas fa-check"></i> <strong>Безлимитный трафик</strong> — даже на бесплатном тарифе</li>
                    <li><i class="fas fa-check"></i> <strong>Без логов</strong> — мы не храним вашу активность</li>
                    <li><i class="fas fa-check"></i> <strong>Высокая скорость</strong> — до 1 Гбит/с на премиум-тарифе</li>
                    <li><i class="fas fa-check"></i> <strong>Обход блокировок</strong> — доступ к любым сайтам</li>
                    <li><i class="fas fa-check"></i> <strong>Защита Wi-Fi</strong> — безопасное использование публичных сетей</li>
                    <li><i class="fas fa-check"></i> <strong>Кill Switch</strong> — защита при потере VPN-соединения</li>
                    <li><i class="fas fa-check"></i> <strong>Совместимость</strong> — работает с Яндекс.Браузером и AdGuard</li>
                </ul>
            </div>
            
            <div class="system-requirements">
                <h2 class="section-title">Системные требования</h2>
                <table class="requirements-table">
                    <thead>
                        <tr>
                            <th>Платформа</th>
                            <th>Минимальные</th>
                            <th>Рекомендуемые</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>Windows</td>
                            <td>Windows 7, 1 ГБ ОЗУ</td>
                            <td>Windows 10/11, 2 ГБ ОЗУ</td>
                        </tr>
                        <tr>
                            <td>Android</td>
                            <td>Android 5.0, 1 ГБ ОЗУ</td>
                            <td>Android 8.0+, 2 ГБ ОЗУ</td>
                        </tr>
                        <tr>
                            <td>iOS</td>
                            <td>iOS 11.0</td>
                            <td>iOS 14.0+</td>
                        </tr>
                        <tr>
                            <td>macOS</td>
                            <td>macOS 10.12</td>
                            <td>macOS 11.0+</td>
                        </tr>
                        <tr>
                            <td>Linux</td>
                            <td>Ubuntu 16.04</td>
                            <td>Ubuntu 20.04+</td>
                        </tr>
                    </tbody>
                </table>
            </div>
            
            <div class="app-screenshots">
                <h2 class="section-title">Скриншоты приложения</h2>
                <div class="screenshots-grid">
                    <div class="screenshot">
                        <img src="https://images.unsplash.com/photo-1550751827-4bd374c3f58b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Интерфейс HideMyName VPN">
                    </div>
                    <div class="screenshot">
                        <img src="https://images.unsplash.com/photo-1531299204818-ea1d6b2b30a8?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Выбор сервера">
                    </div>
                    <div class="screenshot">
                        <img src="https://images.unsplash.com/photo-1558494949-ef010cbdcc31?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Настройки VPN">
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Right Column: Sidebar -->
        <div class="sidebar">
            <!-- Related Apps -->
            <div class="related-apps">
                <h3 class="section-title">Популярные программы</h3>
                <div class="related-apps-list">
                    <a href="https://loadbrowser.github.io/yandex-browser.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #FF2E2E;">
                            <i class="fas fa-globe"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>Яндекс.Браузер</h4>
                            <p>Быстрый и безопасный браузер</p>
                        </div>
                    </a>
                    
                    <a href="https://loadbrowser.github.io/yandex-disk.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #FFCC00;">
                            <i class="fas fa-cloud"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>Яндекс.Диск</h4>
                            <p>Облачное хранилище файлов</p>
                        </div>
                    </a>
                    
                    <a href="https://loadbrowser.github.io/adguard.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #4CAF50;">
                            <i class="fas fa-shield-alt"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>AdGuard</h4>
                            <p>Блокировщик рекламы</p>
                        </div>
                    </a>
                    
                    <a href="https://loadbrowser.github.io/adguard-vpn.html" class="related-app">
                        <div class="related-app-icon" style="background-color: #2196F3;">
                            <i class="fas fa-lock"></i>
                        </div>
                        <div class="related-app-info">
                            <h4>AdGuard VPN</h4>
                            <p>VPN сервис от AdGuard</p>
                        </div>
                    </a>
                </div>
            </div>
            
            <!-- Download Info -->
            <div class="download-info">
                <h3 class="section-title">Информация о загрузке</h3>
                <div class="download-info-item">
                    <h4><i class="fas fa-download"></i> Скачиваний</h4>
                    <p>Более 1,200,000 загрузок</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-calendar-alt"></i> Последнее обновление</h4>
                    <p>25 ноября 2023</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-user-check"></i> Разработчик</h4>
                    <p>HideMyName Technologies</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-language"></i> Языки интерфейса</h4>
                    <p>Русский, English, 中文, Español</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-shield-alt"></i> Безопасность</h4>
                    <p>Проверено на вирусы</p>
                </div>
            </div>
            
            <!-- Quick Stats -->
            <div class="download-info">
                <h3 class="section-title">Статистика серверов</h3>
                <div class="download-info-item">
                    <h4><i class="fas fa-server"></i> Серверы</h4>
                    <p>750+ в 65 странах</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-users"></i> Пользователи</h4>
                    <p>Более 5 миллионов</p>
                </div>
                <div class="download-info-item">
                    <h4><i class="fas fa-bolt"></i> Скорость</h4>
                    <p>До 1 Гбит/с</p>
                </div>
            </div>
        </div>
    </div>

    <!-- VPN Advantages -->
    <section class="vpn-advantages" id="features">
        <div class="container">
            <h2 class="section-title">Преимущества HideMyName VPN</h2>
            <div class="advantages-grid">
                <div class="advantage-card">
                    <div class="advantage-icon">
                        <i class="fas fa-user-shield"></i>
                    </div>
                    <h3>100% анонимность</h3>
                    <p>Скрывайте ваш реальный IP-адрес и местоположение. Ваши данные остаются конфиденциальными.</p>
                </div>
                <div class="advantage-card">
                    <div class="advantage-icon">
                        <i class="fas fa-lock"></i>
                    </div>
                    <h3>Безопасное соединение</h3>
                    <p>Военное шифрование данных защищает вашу информацию при использовании публичных Wi-Fi сетей.</p>
                </div>
                <div class="advantage-card">
                    <div class="advantage-icon">
                        <i class="fas fa-globe"></i>
                    </div>
                    <h3>Доступ к контенту</h3>
                    <p>Обходите географические ограничения и получайте доступ к любым сайтам и сервисам.</p>
                </div>
                <div class="advantage-card">
                    <div class="advantage-icon">
                        <i class="fas fa-tachometer-alt"></i>
                    </div>
                    <h3>Высокая скорость</h3>
                    <p>Оптимизированные серверы обеспечивают максимальную скорость соединения без тормозов.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Compatibility Section -->
    <section class="compatibility-section">
        <div class="container">
            <h2 class="section-title">Совместимость с популярными программами</h2>
            <p class="app-description" style="margin-bottom: 25px;">HideMyName VPN отлично работает вместе с другими популярными приложениями для максимальной производительности и защиты.</p>
            
            <div class="compatibility-grid">
                <a href="https://loadbrowser.github.io/yandex-browser.html" class="compatibility-item">
                    <div class="compatibility-icon" style="background-color: #FF2E2E;">
                        <i class="fas fa-globe"></i>
                    </div>
                    <h4>Яндекс.Браузер</h4>
                    <p style="text-align: center; font-size: 0.9rem; color: var(--gray-color); margin-top: 5px;">Полная совместимость</p>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard.html" class="compatibility-item">
                    <div class="compatibility-icon" style="background-color: #4CAF50;">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h4>AdGuard</h4>
                    <p style="text-align: center; font-size: 0.9rem; color: var(--gray-color); margin-top: 5px;">Совместная работа</p>
                </a>
                
                <a href="https://loadbrowser.github.io/yandex-disk.html" class="compatibility-item">
                    <div class="compatibility-icon" style="background-color: #FFCC00;">
                        <i class="fas fa-cloud"></i>
                    </div>
                    <h4>Яндекс.Диск</h4>
                    <p style="text-align: center; font-size: 0.9rem; color: var(--gray-color); margin-top: 5px;">Защита облака</p>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard-vpn.html" class="compatibility-item">
                    <div class="compatibility-icon" style="background-color: #2196F3;">
                        <i class="fas fa-lock"></i>
                    </div>
                    <h4>AdGuard VPN</h4>
                    <p style="text-align: center; font-size: 0.9rem; color: var(--gray-color); margin-top: 5px;">Альтернатива</p>
                </a>
            </div>
        </div>
    </section>

    <!-- Comparison Section -->
    <section class="comparison-section" id="faq">
        <div class="container">
            <h2 class="section-title">Сравнение с другими VPN сервисами</h2>
            <table class="comparison-table">
                <thead>
                    <tr>
                        <th>Функция</th>
                        <th>HideMyName VPN</th>
                        <th><a href="https://loadbrowser.github.io/adguard-vpn.html" style="color: var(--dark-color); text-decoration: none;">AdGuard VPN</a></th>
                        <th>NordVPN</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td class="feature-name">Бесплатный тариф</td>
                        <td class="vpn-check">✓ Есть (10 Мбит/с)</td>
                        <td class="other-check">Ограниченный трафик</td>
                        <td class="other-check">Нет</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Безлимитный трафик</td>
                        <td class="vpn-check">✓ Да</td>
                        <td class="other-check">На платных тарифах</td>
                        <td class="vpn-check">✓ Да</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Без логов</td>
                        <td class="vpn-check">✓ Гарантируется</td>
                        <td class="vpn-check">✓ Гарантируется</td>
                        <td class="vpn-check">✓ Гарантируется</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Количество серверов</td>
                        <td class="vpn-check">750+</td>
                        <td class="other-check">300+</td>
                        <td class="vpn-check">5500+</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Совместимость с AdGuard</td>
                        <td class="vpn-check">✓ Полная</td>
                        <td class="vpn-check">✓ Полная</td>
                        <td class="other-check">Частичная</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Поддержка P2P</td>
                        <td class="other-check">Нет (бесплатный)</td>
                        <td class="other-check">Нет</td>
                        <td class="vpn-check">✓ Да</td>
                    </tr>
                    <tr>
                        <td class="feature-name">Стоимость (месяц)</td>
                        <td class="vpn-check">Бесплатно / $4.99</td>
                        <td class="other-check">$2.99 / $11.99</td>
                        <td class="other-check">$11.95</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <!-- FAQ Section -->
    <section class="faq-section">
        <div class="container">
            <h2 class="section-title">Часто задаваемые вопросы</h2>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Можно ли использовать HideMyName VPN вместе с Яндекс.Браузером?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, HideMyName VPN полностью совместим с <a href="https://loadbrowser.github.io/yandex-browser.html" style="color: var(--primary-color);">Яндекс.Браузером</a>. После установки VPN просто запустите браузер - все соединения будут автоматически защищены. Вы также можете настроить исключения для определенных сайтов.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Работает ли HideMyName VPN с AdGuard?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, HideMyName VPN отлично работает вместе с <a href="https://loadbrowser.github.io/adguard.html" style="color: var(--primary-color);">AdGuard</a>. Рекомендуется сначала запустить VPN, а затем AdGuard. Это обеспечит двойную защиту: анонимность через VPN и блокировку рекламы через AdGuard.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Чем отличается HideMyName VPN от AdGuard VPN?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p><a href="https://loadbrowser.github.io/adguard-vpn.html" style="color: var(--primary-color);">AdGuard VPN</a> больше фокусируется на интеграции с блокировщиком рекламы, в то время как HideMyName VPN предлагает более широкий выбор серверов и бесплатный тариф с безлимитным трафиком. Оба сервиса качественные, выбор зависит от ваших потребностей.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">
                    <span>Можно ли использовать VPN для Яндекс.Диска?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Да, HideMyName VPN защищает все интернет-соединения, включая <a href="https://loadbrowser.github.io/yandex-disk.html" style="color: var(--primary-color);">Яндекс.Диск</a>. Это особенно полезно при использовании публичных Wi-Fi сетей для загрузки или скачивания файлов из облачного хранилища.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Navigation Cards -->
    <section class="navigation-cards">
        <div class="container">
            <h2 class="section-title">Другие полезные программы</h2>
            <div class="nav-cards-grid">
                <a href="https://loadbrowser.github.io/yandex-browser.html" class="nav-card secondary">
                    <i class="fas fa-globe"></i>
                    <h3>Яндекс.Браузер</h3>
                    <p>Быстрый и безопасный браузер с интеграцией сервисов Яндекса</p>
                </a>
                
                <a href="https://loadbrowser.github.io/yandex-disk.html" class="nav-card">
                    <i class="fas fa-cloud"></i>
                    <h3>Яндекс.Диск</h3>
                    <p>Облачное хранилище для ваших файлов с защитой через VPN</p>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard.html" class="nav-card success">
                    <i class="fas fa-shield-alt"></i>
                    <h3>AdGuard</h3>
                    <p>Лучший блокировщик рекламы для безопасного серфинга</p>
                </a>
                
                <a href="https://loadbrowser.github.io/adguard-vpn.html" class="nav-card info">
                    <i class="fas fa-lock"></i>
                    <h3>AdGuard VPN</h3>
                    <p>Альтернативный VPN сервис от создателей AdGuard</p>
                </a>
            </div>
        </div>
    </section>

    <!-- How to Install -->
    <section class="how-to-install" id="download">
        <div class="container">
            <h2 class="section-title">Как установить HideMyName VPN</h2>
            <div class="install-steps">
                <div class="install-step">
                    <div class="step-number">1</div>
                    <div class="step-content">
                        <h4>Скачайте установщик</h4>
                        <p>Нажмите кнопку "Скачать для Windows" выше. Установщик HideMyName VPN будет загружен на ваш компьютер (файл размером ~53 MB).</p>
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
                        <h4>Запустите и подключитесь</h4>
                        <p>После установки запустите HideMyName VPN, выберите сервер и нажмите кнопку "Подключиться". Ваше соединение теперь защищено!</p>
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
                <textarea placeholder="Оставьте ваш отзыв о HideMyName VPN..."></textarea>
                <button type="submit">Отправить отзыв</button>
            </div>
            
            <div class="comment">
                <div class="comment-avatar">
                    <i class="fas fa-user"></i>
                </div>
                <div class="comment-content">
                    <h4>Иван Сергеев</h4>
                    <div class="comment-date">7 ноября 2023</div>
                    <p>Пользуюсь бесплатной версией уже 3 месяца вместе с <a href="https://loadbrowser.github.io/yandex-browser.html" style="color: var(--primary-color);">Яндекс.Браузером</a>. Отлично работает для обычного серфинга. Скорость достаточная для YouTube в HD. Рекомендую!</p>
                </div>
            </div>
            
            <div class="comment">
                <div class="comment-avatar">
                    <i class="fas fa-user"></i>
                </div>
                <div class="comment-content">
                    <h4>Екатерина Морозова</h4>
                    <div class="comment-date">1 ноября 2023</div>
                    <p>Использую HideMyName VPN вместе с <a href="https://loadbrowser.github.io/adguard.html" style="color: var(--primary-color);">AdGuard</a>. Идеальная комбинация - никакой рекламы и полная анонимность. Бесплатный тариф работает отлично!</p>
                </div>
            </div>
            
            <div class="comment">
                <div class="comment-avatar">
                    <i class="fas fa-user"></i>
                </div>
                <div class="comment-content">
                    <h4>Александр Козлов</h4>
                    <div class="comment-date">28 октября 2023</div>
                    <p>Хороший VPN, особенно для работы с <a href="https://loadbrowser.github.io/yandex-disk.html" style="color: var(--primary-color);">Яндекс.Диском</a> в общественных местах. Защищает мои файлы при загрузке в облако через публичный Wi-Fi.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>HideMyName VPN</h3>
                    <p>Мощный VPN-сервис для защиты вашей приватности в интернете. Бесплатные и платные тарифы с гарантией безопасности.</p>
                    <div style="margin-top: 20px; display: flex; gap: 15px;">
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-telegram"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-twitter"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-github"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Навигация</h3>
                    <ul class="footer-links">
                        <li><a href="https://loadbrowser.github.io/">Главная страница</a></li>
                        <li><a href="https://loadbrowser.github.io/yandex-browser.html">Яндекс.Браузер</a></li>
                        <li><a href="https://loadbrowser.github.io/yandex-disk.html">Яндекс.Диск</a></li>
                        <li><a href="https://loadbrowser.github.io/adguard.html">AdGuard</a></li>
                        <li><a href="https://loadbrowser.github.io/adguard-vpn.html">AdGuard VPN</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Другие программы</h3>
                    <ul class="footer-links">
                        <li><a href="https://loadbrowser.github.io/yandex-browser.html">Яндекс.Браузер</a></li>
                        <li><a href="https://loadbrowser.github.io/adguard.html">AdGuard</a></li>
                        <li><a href="https://loadbrowser.github.io/yandex-disk.html">Яндекс.Диск</a></li>
                        <li><a href="https://loadbrowser.github.io/adguard-vpn.html">AdGuard VPN</a></li>
                        <li><a href="#">Google Chrome</a></li>
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
                <p>&copy; 2023 HideMyName VPN. Все права защищены. VPN должен использоваться в законных целях.</p>
                <p style="margin-top: 10px;">Это демонстрационная страница. HideMyName VPN является вымышленным продуктом.</p>
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
            alert('Загрузка HideMyName VPN для Windows начата!\n\nФайл: hidemyname_vpn_setup.exe\nРазмер: 52.8 MB\n\nФайл будет сохранен в папке "Загрузки".');
        });
        
        document.getElementById('download-android').addEventListener('click', function() {
            alert('Открывается Google Play Store для установки HideMyName VPN на Android.\n\nВы будете перенаправлены в магазин приложений.');
        });
        
        document.getElementById('download-ios').addEventListener('click', function() {
            alert('Открывается App Store для установки HideMyName VPN на iPhone/iPad.\n\nВы будете перенаправлены в магазин приложений Apple.');
        });
        
        document.getElementById('main-download').addEventListener('click', function() {
            alert('Загрузка HideMyName VPN начата!\n\nВыберите вашу операционную систему для загрузки соответствующей версии.');
        });
        
        // Обновление года в футере
        document.querySelector('.footer-bottom p').innerHTML = `&copy; ${new Date().getFullYear()} HideMyName VPN. Все права защищены. VPN должен использоваться в законных целях.`;
        
        // Отправка комментария
        const commentForm = document.querySelector('.comment-form');
        const commentTextarea = commentForm.querySelector('textarea');
        const commentButton = commentForm.querySelector('button');
        
        commentButton.addEventListener('click', function() {
            if (commentTextarea.value.trim() === '') {
                alert('Пожалуйста, введите текст отзыва');
                return;
            }
            
            alert('Спасибо за ваш отзыв о HideMyName VPN! После модерации он будет опубликован на сайте.');
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
        document.querySelectorAll('.install-step, .related-app, .comment, .advantage-card, .compatibility-item, .nav-card').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            observer.observe(el);
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
        
        // Подсветка активной ссылки в хлебных крошках
        const breadcrumbLinks = document.querySelectorAll('.breadcrumbs a');
        
        breadcrumbLinks.forEach(link => {
            const href = link.getAttribute('href');
            if (href.includes('hidemyname')) {
                link.style.color = 'var(--primary-color)';
                link.style.fontWeight = '600';
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
    </script>
</body>
</html>
