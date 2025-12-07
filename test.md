<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SoftWeb - Лучшее программное обеспечение</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #4361ee;
            --primary-dark: #3a56d4;
            --secondary-color: #7209b7;
            --accent-color: #f72585;
            --light-color: #f8f9fa;
            --dark-color: #212529;
            --gray-color: #6c757d;
            --light-gray: #e9ecef;
            --border-radius: 12px;
            --box-shadow: 0 10px 20px rgba(0, 0, 0, 0.08);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', system-ui, sans-serif;
            line-height: 1.6;
            color: var(--dark-color);
            background-color: #fefefe;
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
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
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

        .nav-links {
            display: flex;
            gap: 30px;
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
        }

        .btn {
            padding: 10px 24px;
            border-radius: var(--border-radius);
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            border: none;
            font-size: 1rem;
        }

        .btn-primary {
            background-color: var(--primary-color);
            color: white;
        }

        .btn-primary:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
        }

        .btn-outline {
            background-color: transparent;
            color: var(--primary-color);
            border: 2px solid var(--primary-color);
        }

        .btn-outline:hover {
            background-color: var(--primary-color);
            color: white;
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
            padding: 100px 0;
            background: linear-gradient(135deg, #f5f7ff 0%, #f0f2ff 100%);
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 40%;
            height: 100%;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><path d="M0,0 L100,0 L100,100 Z" fill="%234361ee" opacity="0.03"/></svg>') no-repeat;
            background-size: cover;
        }

        .hero-content {
            display: flex;
            align-items: center;
            gap: 60px;
            position: relative;
            z-index: 1;
        }

        .hero-text {
            flex: 1;
        }

        .hero-text h1 {
            font-size: 3.2rem;
            line-height: 1.1;
            margin-bottom: 20px;
            color: var(--dark-color);
        }

        .hero-text h1 span {
            color: var(--primary-color);
        }

        .hero-text p {
            font-size: 1.2rem;
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
            gap: 20px;
            margin-top: 40px;
        }

        .feature {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .feature i {
            color: var(--primary-color);
            font-size: 1.5rem;
        }

        /* Software Categories */
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-title h2 {
            font-size: 2.5rem;
            color: var(--dark-color);
            margin-bottom: 15px;
        }

        .section-title p {
            color: var(--gray-color);
            max-width: 700px;
            margin: 0 auto;
        }

        .categories {
            padding: 100px 0;
        }

        .category-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
        }

        .category-card {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 35px 25px;
            text-align: center;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
        }

        .category-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }

        .category-icon {
            width: 80px;
            height: 80px;
            background-color: rgba(67, 97, 238, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 25px;
        }

        .category-icon i {
            font-size: 2.2rem;
            color: var(--primary-color);
        }

        .category-card h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
        }

        .category-card p {
            color: var(--gray-color);
            margin-bottom: 20px;
        }

        .category-link {
            color: var(--primary-color);
            text-decoration: none;
            font-weight: 600;
            display: inline-flex;
            align-items: center;
            gap: 8px;
        }

        /* Featured Software */
        .featured-software {
            padding: 100px 0;
            background-color: var(--light-gray);
        }

        .software-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
        }

        .software-card {
            background-color: white;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
        }

        .software-card:hover {
            transform: translateY(-5px);
        }

        .software-img {
            height: 180px;
            background-color: var(--light-color);
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }

        .software-img i {
            font-size: 4rem;
            color: var(--primary-color);
        }

        .software-info {
            padding: 25px;
        }

        .software-info h3 {
            font-size: 1.4rem;
            margin-bottom: 10px;
        }

        .software-info p {
            color: var(--gray-color);
            margin-bottom: 20px;
            font-size: 0.95rem;
        }

        .software-meta {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }

        .software-rating {
            color: #ffc107;
        }

        .software-price {
            font-weight: 700;
            font-size: 1.2rem;
            color: var(--primary-color);
        }

        .software-price.free {
            color: #2ecc71;
        }

        /* CTA Section */
        .cta {
            padding: 100px 0;
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
            color: white;
            text-align: center;
        }

        .cta h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }

        .cta p {
            font-size: 1.2rem;
            margin-bottom: 40px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
            opacity: 0.9;
        }

        .cta .btn {
            background-color: white;
            color: var(--primary-color);
            font-size: 1.1rem;
            padding: 15px 40px;
        }

        /* Footer */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 80px 0 30px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 50px;
            margin-bottom: 60px;
        }

        .footer-column h3 {
            font-size: 1.4rem;
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
                font-size: 2.8rem;
            }
            
            .features {
                justify-content: center;
            }
            
            .hero::before {
                width: 70%;
            }
        }

        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .header-actions {
                display: none;
            }
            
            .hero-text h1 {
                font-size: 2.3rem;
            }
            
            .section-title h2 {
                font-size: 2rem;
            }
            
            .features {
                flex-direction: column;
                align-items: center;
            }
        }

        @media (max-width: 576px) {
            .hero-text h1 {
                font-size: 2rem;
            }
            
            .btn {
                padding: 10px 20px;
            }
            
            .category-grid, .software-grid {
                grid-template-columns: 1fr;
            }
            
            .cta h2 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">
                <i class="fas fa-cube"></i>
                SoftWeb
            </a>
            
            <nav class="nav-links">
                <a href="#" class="active">Главная</a>
                <a href="#categories">Категории</a>
                <a href="#featured">Популярное</a>
                <a href="#">Блог</a>
                <a href="#">Поддержка</a>
            </nav>
            
            <div class="header-actions">
                <button class="btn btn-outline">Войти</button>
                <button class="btn btn-primary">Регистрация</button>
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
                <h1>Лучшее <span>программное обеспечение</span> для всех ваших задач</h1>
                <p>Откройте для себя тысячи приложений, утилит и инструментов для повышения производительности, творчества и развлечений. Все программы проверены на безопасность.</p>
                
                <div class="hero-buttons">
                    <button class="btn btn-primary">Начать поиск</button>
                    <button class="btn btn-outline">Как это работает</button>
                </div>
                
                <div class="features">
                    <div class="feature">
                        <i class="fas fa-shield-alt"></i>
                        <span>100% безопасно</span>
                    </div>
                    <div class="feature">
                        <i class="fas fa-download"></i>
                        <span>Быстрая загрузка</span>
                    </div>
                    <div class="feature">
                        <i class="fas fa-star"></i>
                        <span>Проверенные отзывы</span>
                    </div>
                </div>
            </div>
            
            <div class="hero-image">
                <img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Программное обеспечение">
            </div>
        </div>
    </section>

    <!-- Categories Section -->
    <section class="categories" id="categories">
        <div class="container">
            <div class="section-title">
                <h2>Популярные категории</h2>
                <p>Найдите необходимое программное обеспечение по категориям</p>
            </div>
            
            <div class="category-grid">
                <div class="category-card">
                    <div class="category-icon">
                        <i class="fas fa-desktop"></i>
                    </div>
                    <h3>Операционные системы</h3>
                    <p>Дистрибутивы Linux, системные утилиты, драйверы и обновления</p>
                    <a href="#" class="category-link">Смотреть <i class="fas fa-arrow-right"></i></a>
                </div>
                
                <div class="category-card">
                    <div class="category-icon">
                        <i class="fas fa-briefcase"></i>
                    </div>
                    <h3>Бизнес и офис</h3>
                    <p>Офисные пакеты, планировщики, CRM и бухгалтерские программы</p>
                    <a href="#" class="category-link">Смотреть <i class="fas fa-arrow-right"></i></a>
                </div>
                
                <div class="category-card">
                    <div class="category-icon">
                        <i class="fas fa-paint-brush"></i>
                    </div>
                    <h3>Графика и дизайн</h3>
                    <p>Редакторы изображений, 3D моделирование, CAD и векторная графика</p>
                    <a href="#" class="category-link">Смотреть <i class="fas fa-arrow-right"></i></a>
                </div>
                
                <div class="category-card">
                    <div class="category-icon">
                        <i class="fas fa-gamepad"></i>
                    </div>
                    <h3>Игры и развлечения</h3>
                    <p>Видеоигры, эмуляторы, медиаплееры и стриминговые приложения</p>
                    <a href="#" class="category-link">Смотреть <i class="fas fa-arrow-right"></i></a>
                </div>
                
                <div class="category-card">
                    <div class="category-icon">
                        <i class="fas fa-lock"></i>
                    </div>
                    <h3>Безопасность</h3>
                    <p>Антивирусы, файрволы, VPN и инструменты для шифрования</p>
                    <a href="#" class="category-link">Смотреть <i class="fas fa-arrow-right"></i></a>
                </div>
                
                <div class="category-card">
                    <div class="category-icon">
                        <i class="fas fa-code"></i>
                    </div>
                    <h3>Разработка</h3>
                    <p>IDE, компиляторы, системы контроля версий и отладчики</p>
                    <a href="#" class="category-link">Смотреть <i class="fas fa-arrow-right"></i></a>
                </div>
            </div>
        </div>
    </section>

    <!-- Featured Software Section -->
    <section class="featured-software" id="featured">
        <div class="container">
            <div class="section-title">
                <h2>Рекомендуемое ПО</h2>
                <p>Популярные программы, выбранные нашей командой</p>
            </div>
            
            <div class="software-grid">
                <div class="software-card">
                    <div class="software-img">
                        <i class="fab fa-figma"></i>
                    </div>
                    <div class="software-info">
                        <h3>Figma Design</h3>
                        <p>Профессиональный инструмент для проектирования интерфейсов с совместной работой в реальном времени</p>
                        
                        <div class="software-meta">
                            <div class="software-rating">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star-half-alt"></i>
                                <span>4.7</span>
                            </div>
                            <div class="software-price free">Бесплатно</div>
                        </div>
                        
                        <button class="btn btn-primary" style="width: 100%;">Скачать</button>
                    </div>
                </div>
                
                <div class="software-card">
                    <div class="software-img">
                        <i class="fas fa-video"></i>
                    </div>
                    <div class="software-info">
                        <h3>VideoStudio Pro</h3>
                        <p>Мощный видеоредактор с поддержкой 4K и обширной библиотекой эффектов</p>
                        
                        <div class="software-meta">
                            <div class="software-rating">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="far fa-star"></i>
                                <span>4.2</span>
                            </div>
                            <div class="software-price">$49.99</div>
                        </div>
                        
                        <button class="btn btn-primary" style="width: 100%;">Скачать</button>
                    </div>
                </div>
                
                <div class="software-card">
                    <div class="software-img">
                        <i class="fas fa-file-archive"></i>
                    </div>
                    <div class="software-info">
                        <h3>WinRAR Ultimate</h3>
                        <p>Архиватор файлов с поддержкой всех популярных форматов и высокой степенью сжатия</p>
                        
                        <div class="software-meta">
                            <div class="software-rating">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <span>5.0</span>
                            </div>
                            <div class="software-price">$29.99</div>
                        </div>
                        
                        <button class="btn btn-primary" style="width: 100%;">Скачать</button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="cta">
        <div class="container">
            <h2>Начните использовать лучшее ПО уже сегодня</h2>
            <p>Присоединяйтесь к миллионам пользователей, которые доверяют SoftWeb для поиска и загрузки безопасного программного обеспечения</p>
            <button class="btn">Создать аккаунт бесплатно</button>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>SoftWeb</h3>
                    <p>Крупнейшая библиотека программного обеспечения с 2010 года. Все программы проверяются на безопасность.</p>
                    <div style="margin-top: 20px; display: flex; gap: 15px;">
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-twitter"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-facebook"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-instagram"></i></a>
                        <a href="#" style="color: white; font-size: 1.2rem;"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Категории</h3>
                    <ul class="footer-links">
                        <li><a href="#">Операционные системы</a></li>
                        <li><a href="#">Бизнес и офис</a></li>
                        <li><a href="#">Графика и дизайн</a></li>
                        <li><a href="#">Игры и развлечения</a></li>
                        <li><a href="#">Безопасность</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Компания</h3>
                    <ul class="footer-links">
                        <li><a href="#">О нас</a></li>
                        <li><a href="#">Карьера</a></li>
                        <li><a href="#">Партнеры</a></li>
                        <li><a href="#">Пресса</a></li>
                        <li><a href="#">Контакты</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Правовая информация</h3>
                    <ul class="footer-links">
                        <li><a href="#">Условия использования</a></li>
                        <li><a href="#">Политика конфиденциальности</a></li>
                        <li><a href="#">Политика возврата</a></li>
                        <li><a href="#">Правила загрузки</a></li>
                        <li><a href="#">DMCA</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2023 SoftWeb. Все права защищены. Логотипы и товарные знаки являются собственностью соответствующих владельцев.</p>
            </div>
        </div>
    </footer>

    <script>
        // Мобильное меню
        const mobileMenuBtn = document.querySelector('.mobile-menu-btn');
        const navLinks = document.querySelector('.nav-links');
        
        mobileMenuBtn.addEventListener('click', () => {
            navLinks.style.display = navLinks.style.display === 'flex' ? 'none' : 'flex';
            if (navLinks.style.display === 'flex') {
                navLinks.style.flexDirection = 'column';
                navLinks.style.position = 'absolute';
                navLinks.style.top = '100%';
                navLinks.style.left = '0';
                navLinks.style.right = '0';
                navLinks.style.backgroundColor = 'white';
                navLinks.style.padding = '20px';
                navLinks.style.boxShadow = '0 10px 20px rgba(0,0,0,0.1)';
                navLinks.style.gap = '15px';
            }
        });
        
        // Обновление года в футере
        document.querySelector('.footer-bottom p').innerHTML = `&copy; ${new Date().getFullYear()} SoftWeb. Все права защищены. Логотипы и товарные знаки являются собственностью соответствующих владельцев.`;
        
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
        document.querySelectorAll('.category-card, .software-card').forEach(card => {
            card.style.opacity = '0';
            card.style.transform = 'translateY(20px)';
            card.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            observer.observe(card);
        });
    </script>
</body>
</html>
