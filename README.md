<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Таргетированная реклама Instagram & Meta — Привлекайте больше клиентов</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-main: #FFFFFF;
      --bg-soft: #F8F9FC;
      --text-dark: #111827;
      --text-muted: #4B5563;
      --border-light: #E5E7EB;
      --ig-gradient: linear-gradient(135deg, #833AB4 0%, #FD1D1D 50%, #F56040 100%);
      --meta-blue: #0668E1;
      --gold-accent: #F59E0B;
      --wa-green: #25D366;
      --wa-dark: #1EBE5D;
      --shadow-card: 0 12px 32px rgba(17, 24, 39, 0.06);
      --shadow-hover: 0 20px 40px rgba(131, 58, 180, 0.14);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      -webkit-tap-highlight-color: transparent;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
      background-color: var(--bg-main);
      color: var(--text-dark);
      line-height: 1.5;
      overflow-x: hidden;
    }

    .container {
      width: 100%;
      max-width: 1140px;
      margin: 0 auto;
      padding: 0 20px;
    }

    /* HEADER */
    header {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(255, 255, 255, 0.92);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--border-light);
    }

    .nav-wrap {
      display: flex;
      align-items: center;
      justify-content: space-between;
      height: 68px;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 10px;
      font-weight: 800;
      font-size: 19px;
      color: var(--text-dark);
      text-decoration: none;
    }

    .logo-badge {
      width: 36px;
      height: 36px;
      border-radius: 10px;
      background: var(--ig-gradient);
      display: flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      font-weight: 900;
      font-size: 18px;
      box-shadow: 0 6px 14px rgba(253, 29, 29, 0.25);
    }

    .nav-links {
      display: flex;
      gap: 28px;
    }

    .nav-links a {
      text-decoration: none;
      color: var(--text-muted);
      font-weight: 600;
      font-size: 15px;
      transition: color 0.2s;
    }

    .nav-links a:hover {
      color: #833AB4;
    }

    .header-btn {
      background: var(--text-dark);
      color: #fff;
      border: none;
      padding: 10px 18px;
      border-radius: 12px;
      font-weight: 700;
      font-size: 14px;
      cursor: pointer;
      text-decoration: none;
      transition: transform 0.2s, background 0.2s;
    }

    .header-btn:hover {
      background: #833AB4;
      transform: translateY(-1px);
    }

    /* HERO SECTION */
    .hero {
      padding: 56px 0 64px;
      background:
        radial-gradient(circle at 85% 15%, rgba(253, 29, 29, 0.08) 0%, transparent 45%),
        radial-gradient(circle at 15% 80%, rgba(6, 104, 225, 0.08) 0%, transparent 45%),
        #FFFFFF;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.15fr 0.85fr;
      gap: 40px;
      align-items: center;
    }

    .pill-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-bottom: 20px;
    }

    .pill {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      padding: 6px 14px;
      border-radius: 999px;
      font-size: 13px;
      font-weight: 700;
      background: #F3E8FF;
      color: #7E22CE;
    }

    .pill.meta {
      background: #EFF6FF;
      color: var(--meta-blue);
    }

    .hero h1 {
      font-size: clamp(32px, 4.5vw, 52px);
      font-weight: 900;
      line-height: 1.12;
      letter-spacing: -0.02em;
      margin-bottom: 18px;
    }

    .gradient-text {
      background: var(--ig-gradient);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .hero-subtitle {
      font-size: clamp(16px, 2vw, 19px);
      color: var(--text-muted);
      margin-bottom: 28px;
      max-width: 560px;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 14px;
      margin-bottom: 32px;
    }

    .btn-primary {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      background: var(--ig-gradient);
      color: #fff;
      font-weight: 800;
      font-size: 16px;
      padding: 16px 28px;
      border-radius: 16px;
      border: none;
      cursor: pointer;
      text-decoration: none;
      box-shadow: 0 12px 26px rgba(253, 29, 29, 0.28);
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .btn-primary:hover {
      transform: translateY(-2px);
      box-shadow: 0 16px 32px rgba(131, 58, 180, 0.35);
    }

    .btn-secondary {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      background: #fff;
      color: var(--text-dark);
      font-weight: 700;
      font-size: 16px;
      padding: 16px 24px;
      border-radius: 16px;
      border: 2px solid var(--border-light);
      cursor: pointer;
      text-decoration: none;
      transition: border-color 0.2s, background 0.2s;
    }

    .btn-secondary:hover {
      border-color: #833AB4;
      background: #FAF5FF;
    }

    .hero-card {
      background: #FFFFFF;
      border: 1px solid var(--border-light);
      border-radius: 26px;
      padding: 28px;
      box-shadow: var(--shadow-card);
      position: relative;
    }

    .hero-card-badge {
      display: inline-block;
      background: #FEF3C7;
      color: #B45309;
      font-weight: 800;
      font-size: 13px;
      padding: 6px 12px;
      border-radius: 10px;
      margin-bottom: 16px;
    }

    .feature-list {
      display: flex;
      flex-direction: column;
      gap: 14px;
    }

    .feature-item {
      display: flex;
      align-items: center;
      gap: 14px;
      padding: 14px;
      border-radius: 16px;
      background: var(--bg-soft);
      border: 1px solid #F1F5F9;
    }

    .feature-icon {
      width: 44px;
      height: 44px;
      border-radius: 12px;
      background: #fff;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 22px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.05);
      flex-shrink: 0;
    }

    .feature-item strong {
      display: block;
      font-size: 15px;
      font-weight: 800;
      color: var(--text-dark);
    }

    .feature-item span {
      font-size: 13px;
      color: var(--text-muted);
    }

    /* PRICING SECTION */
    .section {
      padding: 72px 0;
    }

    .section.soft {
      background: var(--bg-soft);
      border-top: 1px solid var(--border-light);
      border-bottom: 1px solid var(--border-light);
    }

    .section-head {
      text-align: center;
      max-width: 680px;
      margin: 0 auto 44px;
    }

    .section-head h2 {
      font-size: clamp(26px, 3.8vw, 38px);
      font-weight: 900;
      margin-bottom: 12px;
      letter-spacing: -0.02em;
    }

    .section-head p {
      color: var(--text-muted);
      font-size: 16px;
    }

    .pricing-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 24px;
    }

    .price-card {
      background: #FFFFFF;
      border: 2px solid var(--border-light);
      border-radius: 26px;
      padding: 28px 24px;
      box-shadow: var(--shadow-card);
      display: flex;
      flex-direction: column;
      transition: transform 0.25s, border-color 0.25s, box-shadow 0.25s;
      position: relative;
    }

    .price-card:hover {
      transform: translateY(-6px);
      border-color: #833AB4;
      box-shadow: var(--shadow-hover);
    }

    .price-card.popular {
      border-color: #FD1D1D;
      box-shadow: 0 18px 40px rgba(253, 29, 29, 0.12);
    }

    .popular-tag {
      position: absolute;
      top: -14px;
      right: 22px;
      background: var(--ig-gradient);
      color: #fff;
      font-size: 12px;
      font-weight: 800;
      padding: 5px 14px;
      border-radius: 999px;
      letter-spacing: 0.03em;
      text-transform: uppercase;
    }

    .budget-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 8px;
    }

    .budget-amount {
      font-size: 42px;
      font-weight: 900;
      background: var(--ig-gradient);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      line-height: 1;
    }

    .budget-per {
      font-size: 13px;
      font-weight: 700;
      color: var(--text-muted);
      background: var(--bg-soft);
      padding: 6px 12px;
      border-radius: 10px;
    }

    .included-note {
      display: inline-block;
      font-size: 13px;
      font-weight: 700;
      color: #059669;
      background: #ECFDF5;
      padding: 4px 10px;
      border-radius: 8px;
      margin-bottom: 20px;
      width: fit-content;
    }

    .tariff-options {
      display: flex;
      flex-direction: column;
      gap: 10px;
      margin-bottom: 24px;
      flex-grow: 1;
    }

    .option-row {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 14px 16px;
      border-radius: 14px;
      border: 1.5px solid var(--border-light);
      background: #FFFFFF;
      cursor: pointer;
      transition: all 0.2s;
    }

    .option-row:hover {
      border-color: #833AB4;
      background: #FAF5FF;
    }

    .option-row.selected {
      border-color: #FD1D1D;
      background: #FFF1F2;
    }

    .option-days {
      font-weight: 700;
      font-size: 15px;
      color: var(--text-dark);
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .radio-dot {
      width: 18px;
      height: 18px;
      border-radius: 50%;
      border: 2px solid #9CA3AF;
      display: inline-flex;
      align-items: center;
      justify-content: center;
    }

    .option-row.selected .radio-dot {
      border-color: #FD1D1D;
    }

    .option-row.selected .radio-dot::after {
      content: '';
      width: 9px;
      height: 9px;
      border-radius: 50%;
      background: #FD1D1D;
    }

    .option-price {
      font-weight: 900;
      font-size: 17px;
      color: var(--text-dark);
    }

    .btn-order-card {
      width: 100%;
      padding: 15px;
      border-radius: 14px;
      border: none;
      background: var(--text-dark);
      color: #fff;
      font-weight: 800;
      font-size: 15px;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      transition: background 0.2s, transform 0.2s;
    }

    .price-card.popular .btn-order-card {
      background: var(--ig-gradient);
    }

    .btn-order-card:hover {
      background: var(--wa-green);
      transform: translateY(-2px);
    }

    /* STEPS */
    .steps-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }

    .step-box {
      background: #fff;
      border: 1px solid var(--border-light);
      border-radius: 22px;
      padding: 24px 20px;
      box-shadow: var(--shadow-card);
    }

    .step-num {
      width: 38px;
      height: 38px;
      border-radius: 12px;
      background: var(--ig-gradient);
      color: #fff;
      font-weight: 900;
      font-size: 16px;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 14px;
    }

    .step-box h3 {
      font-size: 17px;
      font-weight: 800;
      margin-bottom: 8px;
    }

    .step-box p {
      font-size: 14px;
      color: var(--text-muted);
    }

    /* ORDER FORM SECTION */
    .cta-box {
      background: linear-gradient(135deg, #FFF5F7 0%, #F5F3FF 100%);
      border: 2px solid #F3E8FF;
      border-radius: 30px;
      padding: 40px;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 36px;
      align-items: center;
    }

    .cta-box h2 {
      font-size: clamp(24px, 3.4vw, 34px);
      font-weight: 900;
      margin-bottom: 12px;
    }

    .cta-box p {
      color: var(--text-muted);
      margin-bottom: 20px;
      font-size: 16px;
    }

    .form-card {
      background: #fff;
      padding: 26px;
      border-radius: 22px;
      box-shadow: var(--shadow-card);
      border: 1px solid var(--border-light);
    }

    .form-group {
      margin-bottom: 14px;
    }

    .form-group label {
      display: block;
      font-size: 13px;
      font-weight: 700;
      margin-bottom: 6px;
      color: var(--text-dark);
    }

    .form-group input,
    .form-group select {
      width: 100%;
      padding: 13px 15px;
      border-radius: 12px;
      border: 1.5px solid var(--border-light);
      font-size: 15px;
      font-family: inherit;
      outline: none;
      transition: border-color 0.2s;
      background: #fff;
    }

    .form-group input:focus,
    .form-group select:focus {
      border-color: #833AB4;
    }

    .btn-wa-submit {
      width: 100%;
      padding: 16px;
      border-radius: 14px;
      border: none;
      background: var(--wa-green);
      color: #fff;
      font-weight: 800;
      font-size: 16px;
      cursor: pointer;
      box-shadow: 0 10px 22px rgba(37, 211, 102, 0.3);
      transition: background 0.2s, transform 0.2s;
    }

    .btn-wa-submit:hover {
      background: var(--wa-dark);
      transform: translateY(-2px);
    }

    /* FOOTER */
    footer {
      padding: 32px 0;
      text-align: center;
      color: var(--text-muted);
      font-size: 14px;
      border-top: 1px solid var(--border-light);
    }

    /* FLOATING WHATSAPP */
    .floating-wa {
      position: fixed;
      bottom: 22px;
      right: 22px;
      z-index: 99;
      background: var(--wa-green);
      color: #fff;
      padding: 14px 20px;
      border-radius: 999px;
      font-weight: 800;
      font-size: 14px;
      text-decoration: none;
      box-shadow: 0 10px 25px rgba(37, 211, 102, 0.4);
      display: flex;
      align-items: center;
      gap: 8px;
      transition: transform 0.2s;
    }

    .floating-wa:hover {
      transform: scale(1.05);
    }

    /* RESPONSIVE: TABLET & MOBILE (iPhone, Android, iPad, Laptop) */
    @media (max-width: 960px) {
      .hero-grid,
      .cta-box {
        grid-template-columns: 1fr;
      }
      .pricing-grid {
        grid-template-columns: 1fr;
        max-width: 480px;
        margin: 0 auto;
      }
      .steps-grid {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    @media (max-width: 600px) {
      .nav-links {
        display: none;
      }
      .hero {
        padding: 36px 0 48px;
      }
      .hero-actions {
        flex-direction: column;
      }
      .btn-primary,
      .btn-secondary {
        width: 100%;
      }
      .steps-grid {
        grid-template-columns: 1fr;
      }
      .cta-box {
        padding: 24px 18px;
      }
      .floating-wa span {
        display: none;
      }
      .floating-wa {
        width: 56px;
        height: 56px;
        justify-content: center;
        padding: 0;
        font-size: 24px;
      }
    }
  </style>
</head>
<body>

  <!-- HEADER -->
  <header>
    <div class="container nav-wrap">
      <a href="#" class="logo">
        <div class="logo-badge">T</div>
        <span>Target Pro</span>
      </a>
      <nav class="nav-links">
        <a href="#benefits">Преимущества</a>
        <a href="#pricing">Тарифы и цены</a>
        <a href="#steps">Как работаем</a>
      </nav>
      <a href="#pricing" class="header-btn">Выбрать тариф</a>
    </div>
  </header>

  <!-- HERO -->
  <section class="hero">
    <div class="container hero-grid">
      <div>
        <div class="pill-tags">
          <span class="pill">📸 Instagram Ads</span>
          <span class="pill meta">∞ Meta Business</span>
        </div>
        <h1>
          Таргетированная <span class="gradient-text">реклама</span> для вашего бизнеса
        </h1>
        <p class="hero-subtitle">
          Привлекайте больше целевых клиентов, заявок и продаж каждый день. Грамотная настройка рекламного бюджета под ключ — от 1300 сом.
        </p>
        <div class="hero-actions">
          <a href="#pricing" class="btn-primary">🚀 Смотреть тарифы</a>
          <a href="#order" class="btn-secondary">Получить консультацию</a>
        </div>
      </div>

      <div class="hero-card" id="benefits">
        <span class="hero-card-badge">✨ Grow Your Business</span>
        <div class="feature-list">
          <div class="feature-item">
            <div class="feature-icon">🎯</div>
            <div>
              <strong>Точный таргетинг на аудиторию</strong>
              <span>Показываем рекламу тем, кто готов купить прямо сейчас</span>
            </div>
          </div>
          <div class="feature-item">
            <div class="feature-icon">📈</div>
            <div>
              <strong>Больше заявок и продаж</strong>
              <span>Поток обращений в Direct и WhatsApp с первого дня</span>
            </div>
          </div>
          <div class="feature-item">
            <div class="feature-icon">💳</div>
            <div>
              <strong>Эффективный бюджет</strong>
              <span>Без слива денег — работа в рамках выбранного пакета</span>
            </div>
          </div>
          <div class="feature-item">
            <div class="feature-icon">🛡️</div>
            <div>
              <strong>Профессиональный подход</strong>
              <span>Работа и настройка уже включены в стоимость (Услуга ичинде)</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- PRICING -->
  <section class="section soft" id="pricing">
    <div class="container">
      <div class="section-head">
        <h2>Тарифы на запуск рекламы</h2>
        <p>Выберите дневной бюджет ($3, $5 или $10) и количество дней. Нажмите на нужный срок и оформите запуск в один клик.</p>
      </div>

      <div class="pricing-grid">
        <!-- CARD $3 -->
        <div class="price-card" data-budget="$3 в день">
          <div class="budget-header">
            <div class="budget-amount">$3</div>
            <div class="budget-per">Бюджет / день</div>
          </div>
          <div class="included-note">✅ Услуга ичинде (всё включено)</div>

          <div class="tariff-options">
            <div class="option-row selected" onclick="selectOption(this, 'Бюджет $3 — 3 күнгө (1 300 сом)')">
              <div class="option-days"><span class="radio-dot"></span> 3 күнгө</div>
              <div class="option-price">1 300 сом</div>
            </div>
            <div class="option-row" onclick="selectOption(this, 'Бюджет $3 — 5 күнгө (1 800 сом)')">
              <div class="option-days"><span class="radio-dot"></span> 5 күнгө</div>
              <div class="option-price">1 800 сом</div>
            </div>
            <div class="option-row" onclick="selectOption(this, 'Бюджет $3 — 7 күнгө (2 400 сом)')">
              <div class="option-days"><span class="radio-dot"></span> 7 күнгө</div>
              <div class="option-price">2 400 сом</div>
            </div>
          </div>

          <button class="btn-order-card" onclick="orderFromCard(this)">
            📲 Заказать в WhatsApp
          </button>
        </div>

        <!-- CARD $5 -->
        <div class="price-card popular" data-budget="$5 в день">
          <div class="popular-tag">🔥 Оптимальный выбор</div>
          <div class="budget-header">
            <div class="budget-amount">$5</div>
            <div class="budget-per">Бюджет / день</div>
          </div>
          <div class="included-note">✅ Услуга ичинде (всё включено)</div>

          <div class="tariff-options">
            <div class="option-row" onclick="selectOption(this, 'Бюджет $5 — 3 күнгө (1 800 сом)')">
              <div class="option-days"><span class="radio-dot"></span> 3 күнгө</div>
              <div class="option-price">1 800 сом</div>
            </div>
            <div class="option-row selected" onclick="selectOption(this, 'Бюджет $5 — 5 күнгө (2 700 сом)')">
              <div class="option-days"><span class="radio-dot"></span> 5 күнгө</div>
              <div class="option-price">2 700 сом</div>
            </div>
            <div class="option-row" onclick="selectOption(this, 'Бюджет $5 — 7 күнгө (3 500 сом)')">
              <div class="option-days"><span class="radio-dot"></span> 7 күнгө</div>
              <div class="option-price">3 500 сом</div>
            </div>
          </div>

          <button class="btn-order-card" onclick="orderFromCard(this)">
            📲 Заказать в WhatsApp
          </button>
        </div>

        <!-- CARD $10 -->
        <div class="price-card" data-budget="$10 в день">
          <div class="budget-header">
            <div class="budget-amount">$10</div>
            <div class="budget-per">Бюджет / день</div>
          </div>
          <div class="included-note">✅ Услуга ичинде (всё включено)</div>

          <div class="tariff-options">
            <div class="option-row selected" onclick="selectOption(this, 'Бюджет $10 — 3 күнгө (2 650 сом)')">
              <div class="option-days"><span class="radio-dot"></span> 3 күнгө</div>
              <div class="option-price">2 650 сом</div>
            </div>
            <div class="option-row" onclick="selectOption(this, 'Бюджет $10 — 5 күнгө (4 880 сом)')">
              <div class="option-days"><span class="radio-dot"></span> 5 күнгө</div>
              <div class="option-price">4 880 сом</div>
            </div>
            <div class="option-row" onclick="selectOption(this, 'Бюджет $10 — 7 күнгө (6 650 сом)')">
              <div class="option-days"><span class="radio-dot"></span> 7 күнгө</div>
              <div class="option-price">6 650 сом</div>
            </div>
          </div>

          <button class="btn-order-card" onclick="orderFromCard(this)">
            📲 Заказать в WhatsApp
          </button>
        </div>
      </div>
    </div>
  </section>

  <!-- HOW IT WORKS -->
  <section class="section" id="steps">
    <div class="container">
      <div class="section-head">
        <h2>Как запускается ваша реклама</h2>
        <p>Всего 4 простых шага до первых заявок от клиентов</p>
      </div>

      <div class="steps-grid">
        <div class="step-box">
          <div class="step-num">1</div>
          <h3>Выбор тарифа</h3>
          <p>Выбираете подходящий бюджет ($3, $5 или $10) и срок работы рекламы.</p>
        </div>
        <div class="step-box">
          <div class="step-num">2</div>
          <h3>Анализ и аудитория</h3>
          <p>Подбираем интересы, возраст и географию ваших покупателей.</p>
        </div>
        <div class="step-box">
          <div class="step-num">3</div>
          <h3>Запуск в Meta</h3>
          <p>Настраиваем рекламную кампанию в Instagram и Facebook.</p>
        </div>
        <div class="step-box">
          <div class="step-num">4</div>
          <h3>Заявки и рост</h3>
          <p>Вы принимаете обращения клиентов в Direct и WhatsApp.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- QUICK ORDER FORM -->
  <section class="section" id="order" style="padding-top: 0;">
    <div class="container">
      <div class="cta-box">
        <div>
          <h2>Инвестируйте разумно — развивайте свой бизнес! ❤️</h2>
          <p>Оставьте заявку прямо сейчас — помогу выбрать оптимальный бюджет под вашу нишу и запущу рекламу в кратчайшие сроки.</p>
          <p style="font-weight: 700; color: var(--text-dark);">✨ Ваш успех в наших руках!</p>
        </div>

        <div class="form-card">
          <div class="form-group">
            <label>Ваше имя</label>
            <input type="text" id="clientName" placeholder="Например: Айгерим" />
          </div>
          <div class="form-group">
            <label>Ваш Instagram или ниша бизнеса</label>
            <input type="text" id="clientBusiness" placeholder="@ваш_аккаунт или магазин одежды" />
          </div>
          <div class="form-group">
            <label>Интересующий тариф</label>
            <select id="clientTariff">
              <option value="Бюджет $3 — 3 күнгө (1 300 сом)">$3 — 3 күнгө (1 300 сом)</option>
              <option value="Бюджет $3 — 5 күнгө (1 800 сом)">$3 — 5 күнгө (1 800 сом)</option>
              <option value="Бюджет $3 — 7 күнгө (2 400 сом)">$3 — 7 күнгө (2 400 сом)</option>
              <option value="Бюджет $5 — 3 күнгө (1 800 сом)">$5 — 3 күнгө (1 800 сом)</option>
              <option value="Бюджет $5 — 5 күнгө (2 700 сом)" selected>$5 — 5 күнгө (2 700 сом) 🔥</option>
              <option value="Бюджет $5 — 7 күнгө (3 500 сом)">$5 — 7 күнгө (3 500 сом)</option>
              <option value="Бюджет $10 — 3 күнгө (2 650 сом)">$10 — 3 күнгө (2 650 сом)</option>
              <option value="Бюджет $10 — 5 күнгө (4 880 сом)">$10 — 5 күнгө (4 880 сом)</option>
              <option value="Бюджет $10 — 7 күнгө (6 650 сом)">$10 — 7 күнгө (6 650 сом)</option>
            </select>
          </div>
          <button class="btn-wa-submit" onclick="sendCustomOrder()">
            💬 Отправить заявку в WhatsApp
          </button>
        </div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="container">
      © 2026 Target Pro — Таргетированная реклама для вашего бизнеса. Все права защищены.
    </div>
  </footer>

  <!-- FLOATING WHATSAPP BUTTON -->
  <a href="javascript:void(0)" onclick="openWhatsApp('Здравствуйте! Хочу проконсультироваться по запуску таргетированной рекламы.')" class="floating-wa">
    💬 <span>Написать в WhatsApp</span>
  </a>

  <script>
    // ВСТАВЬ СЮДА НОМЕР WHATSAPP КЛИЕНТКИ (в формате 996XXXXXXXXX без плюса)
    const WHATSAPP_PHONE = "996506696699";

    function selectOption(element, tariffText) {
      const card = element.closest('.price-card');
      card.querySelectorAll('.option-row').forEach(row => row.classList.remove('selected'));
      element.classList.add('selected');
      card.setAttribute('data-selected-tariff', tariffText);
    }

    function orderFromCard(btn) {
      const card = btn.closest('.price-card');
      const selectedRow = card.querySelector('.option-row.selected');
      const daysText = selectedRow.querySelector('.option-days').innerText.trim();
      const priceText = selectedRow.querySelector('.option-price').innerText.trim();
      const budgetText = card.getAttribute('data-budget');

      const message = `Здравствуйте! Хочу заказать таргетированную рекламу:\n• Тариф: ${budgetText}\n• Срок: ${daysText}\n• Стоимость: ${priceText} (Услуга ичинде)`;
      openWhatsApp(message);
    }

    function sendCustomOrder() {
      const name = document.getElementById('clientName').value.trim() || 'Не указано';
      const business = document.getElementById('clientBusiness').value.trim() || 'Не указано';
      const tariff = document.getElementById('clientTariff').value;

      const message = `Здравствуйте! Заявка с сайта на таргет:\n• Имя: ${name}\n• Бизнес / Instagram: ${business}\n• Выбранный пакет: ${tariff}`;
      openWhatsApp(message);
    }

    function openWhatsApp(text) {
      const url = `https://wa.me/${WHATSAPP_PHONE}?text=${encodeURIComponent(text)}`;
      window.open(url, '_blank');
    }
  </script>
</body>
</html>
