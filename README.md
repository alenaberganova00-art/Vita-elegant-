<meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vita Elegant Catering - Фуршетний кейтеринг у Лондоні</title>
    <style>
        :root {
            --brown-dark: #8B4513;
            --brown-light: #D2691E;
            --gold: #FFD700;
            --cream: #FFF8DC;
            --whatsapp: #25D366;
            --telegram: #0088cc;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
        }

        body {
            background: linear-gradient(135deg, #fff8f0 0%, #ffe8d6 100%);
            color: #333;
            line-height: 1.6;
            min-height: 100vh;
            padding: 10px;
        }

        .container {
            max-width: 1000px;
            margin: 0 auto;
        }

        header {
            background: linear-gradient(135deg, var(--brown-dark), var(--brown-light));
            color: white;
            text-align: center;
            padding: 40px 20px;
            border-radius: 20px;
            margin-bottom: 25px;
            box-shadow: 0 10px 30px rgba(139, 69, 19, 0.4);
            position: relative;
            overflow: hidden;
        }

        header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 100%;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" opacity="0.1"><path fill="white" d="M50 0L100 50L50 100L0 50Z"/></svg>');
        }

        .logo {
            font-size: 3rem;
            font-weight: bold;
            margin-bottom: 15px;
            color: var(--gold);
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            position: relative;
        }

        .tagline {
            font-size: 1.3rem;
            opacity: 0.95;
            position: relative;
        }

        .menu-category {
            background: white;
            border-radius: 20px;
            padding: 25px;
            margin-bottom: 25px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.08);
            border-left: 6px solid var(--brown-light);
            transition: transform 0.3s ease;
        }

        .menu-category:hover {
            transform: translateY(-3px);
        }

        .category-title {
            color: var(--brown-dark);
            font-size: 1.6rem;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 12px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--cream);
        }

        .menu-items {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .menu-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px;
            background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
            border-radius: 12px;
            border-left: 4px solid var(--gold);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .menu-item:hover {
            transform: translateX(8px);
            box-shadow: 0 5px 15px rgba(139, 69, 19, 0.2);
        }

        .item-name {
            font-weight: 600;
            flex: 1;
            font-size: 1.1rem;
        }

        .item-price {
            color: var(--brown-dark);
            font-weight: bold;
            font-size: 1.3rem;
            white-space: nowrap;
            margin-left: 15px;
            background: var(--gold);
            padding: 5px 12px;
            border-radius: 20px;
            min-width: 80px;
            text-align: center;
        }

        .contact-section {
            background: white;
            border-radius: 20px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 5px 20px rgba(0,0,0,0.08);
            margin-top: 30px;
            background: linear-gradient(135deg, white 0%, var(--cream) 100%);
        }

        .contact-title {
            color: var(--brown-dark);
            font-size: 1.8rem;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }

        .contact-info {
            font-size: 1.3rem;
            margin: 18px 0;
            color: #5D4037;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }

        .btn-container {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 25px;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            color: white;
            padding: 16px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 1.1rem;
            min-width: 200px;
            justify-content: center;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.3);
        }

        .whatsapp-btn { 
            background: var(--whatsapp);
        }

        .telegram-btn { 
            background: var(--telegram);
        }

        .phone-btn { 
            background: linear-gradient(135deg, var(--brown-dark), var(--brown-light));
        }

        .footer {
            text-align: center;
            margin-top: 40px;
            padding: 25px;
            color: #666;
            font-size: 1rem;
            border-top: 2px solid var(--cream);
        }

        .emoji { 
            font-size: 1.4em; 
        }

        /* Анімації */
        @keyframes fadeInUp {
            from { 
                opacity: 0; 
                transform: translateY(30px); 
            }
            to { 
                opacity: 1; 
                transform: translateY(0); 
            }
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        .animate-item {
            animation: fadeInUp 0.8s ease forwards;
            animation-play-state: paused;
        }

        .pulse {
            animation: pulse 2s infinite;
        }

        /* Адаптивність */
        @media (max-width: 768px) {
            .container { 
                padding: 5px; 
            }
            
            header { 
                padding: 30px 15px; 
                border-radius: 15px;
            }
            
            .logo { 
                font-size: 2.2rem; 
            }
            
            .tagline {
                font-size: 1.1rem;
            }
            
            .menu-category { 
                padding: 20px;
                border-radius: 15px;
            }
            
            .category-title {
                font-size: 1.4rem;
            }
            
            .btn-container {
                flex-direction: column;
                align-items: center;
            }
            
            .btn {
                min-width: 250px;
                padding: 14px 25px;
                font-size: 1rem;
            }
            
            .menu-item {
                flex-direction: column;
                align-items: flex-start;
                text-align: left;
                gap: 8px;
            }
            
            .item-price { 
                align-self: stretch; 
                text-align: center;
                margin-left: 0;
                margin-top: 5px;
            }
        }

        @media (max-width: 480px) {
            .logo { font-size: 1.8rem; }
            .category-title { font-size: 1.2rem; }
            .contact-title { font-size: 1.4rem; }
            .contact-info { font-size: 1.1rem; }
            .btn { min-width: 100%; }
        }
    </style>


    <div class="container">
        <header>
            <div class="logo">VITA ELEGANT</div>
            <div class="tagline">🍽️ Фуршетний кейтеринг у Лондоні</div>
        </header>

        <!-- Сирники, Налисники, Деруни -->
        <section class="menu-category">
            <h2 class="category-title">🥞 Сирники, Налисники, Деруни</h2>
            <div class="menu-items">
                <div class="menu-item animate-item" style="animation-delay: 0.1s">
                    Сирники класичні з родзинками
                    17£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.2s">
                    Сирники з маком
                    17£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.3s">
                    Налисники з сиром/родзинками
                    16£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.4s">
                    Налисники з маком/вишнею/сиром
                    19£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.5s">
                    Налисники з яблуками і корицею
                    15£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.6s">
                    Деруни класичні (1 кг)
                    13£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.7s">
                    Деруни з грибами
                    14£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.8s">
                    Деруни з м'ясом
                    15£
                </div>
            </div>
        </section>

        <!-- Голубці -->
        <section class="menu-category">
            <h2 class="category-title">🥬 Голубці</h2>
            <div class="menu-items">
                <div class="menu-item animate-item" style="animation-delay: 0.1s">
                    Голубці з курятини
                    16£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.2s">
                    Голубці з грибами
                    15£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.3s">
                    Голубці зі свинини
                    17£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.4s">
                    Голубці з яловичиною
                    18£
                </div>
            </div>
        </section>

        <!-- Вареники -->
        <section class="menu-category">
            <h2 class="category-title">🥟 Вареники</h2>
            <div class="menu-items">
                <div class="menu-item animate-item" style="animation-delay: 0.1s">
                    Вареники з картоплею
                    13£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.2s">
                    Вареники з капустою
                    14£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.3s">
                    Вареники з сиром
                    15£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.4s">
                    Вареники з вишнею/полуницею
                    17£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.5s">
                    Вареники з курячим м'ясом
                    17£
                </div>
            </div>
        </section>

        <!-- Пельмені -->
        <section class="menu-category">
            <h2 class="category-title">🍴 Пельмені (1 кг)</h2>
            <div class="menu-items">
                <div class="menu-item animate-item" style="animation-delay: 0.1s">
                    Пельмені з куркою
                    16£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.2s">
                    Пельмені з свининою
                    17£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.3s">
                    Пельмені з яловичиною
                    18£
                </div>
            </div>
        </section>

        <!-- Котлети та Відбивні -->
        <section class="menu-category">
            <h2 class="category-title">🍖 Котлети та Відбивні</h2>
            <div class="menu-items">
                <div class="menu-item animate-item" style="animation-delay: 0.1s">
                    Курячі відбивні (10 шт)
                    17£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.2s">
                    Курячі котлети з сиром
                    17£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.3s">
                    Свинячі відбивні (10 шт)
                    18£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.4s">
                    Котлети з яловичини
                    19£
                </div>
                <div class="menu-item animate-item" style="animation-delay: 0.5s">
                    Котлети Київські
                    22£
                </div>
            </div>
        </section>

        <!-- Контакти -->
        <section class="contact-section">
            <h2 class="contact-title">📞 Зв'язатися з нами</h2>
            
            <div class="contact-info">
                📱 Телефон: <strong>+447366499132</strong>
            </div>
            <div class="contact-info">
                📍 Лондон, Великобританія
            </div>
            <div class="contact-info">
                🚚 Доставка по Лондону
            </div>
            <div class="contact-info">
                ⏰ Працюємо 7 днів на тиждень
            </div>

            <div class="btn-container">
                <a href="https://wa.me/447366499132" class="btn whatsapp-btn">
                    💬 WhatsApp
                </a>
                <a href="https://t.me/Vita_Elegant_Bot" class="btn telegram-btn">
                    ✨ Telegram
                </a>
                <a href="tel:+447366499132" class="btn phone-btn">
                    📞 Зателефонувати
                </a>
            </div>
        </section>

        <footer class="footer">
            <p>© 2024 Vita Elegant Catering. Усі права захищені.</p>
            <p style="margin-top: 10px; font-size: 0.9em; opacity: 0.7;">Фуршетний кейтеринг у Лондоні</p>
        </footer>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Анімація при прокрутці
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.animationPlayState = 'running';
                    }
                });
            }, { 
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            });

            document.querySelectorAll('.animate-item').forEach(item => {
                observer.observe(item);
            });

            // Додаємо ефект пульсації для кнопок
            const buttons = document.querySelectorAll('.btn');
            buttons.forEach(btn => {
                btn.addEventListener('mouseenter', function() {
                    this.classList.add('pulse');
                });
                
                btn.addEventListener('mouseleave', function() {
                    this.classList.remove('pulse');
                });
            });

            // Плавна прокрутка для всіх посилань
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    const target = document.querySelector(this.getAttribute('href'));
                    if (target) {
                        target.scrollIntoView({
                            behavior: 'smooth',
                            block: 'start'
                        });
                    }
                });
            });
        });
    </script>
