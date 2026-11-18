<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>BAGI SMM — Таргетированная реклама в Instagram и Meta</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #FFFFFF;
      --surface: #F7F7F5;
      --surface-alt: #EFECE6;
      --text: #141414;
      --text-secondary: #5C5C5C;
      --border: #E5E4E0;
      --accent: #141414;
      --accent-warm: #C85A32;
      --wa: #1F8B4C;
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
      font-family: 'Manrope', -apple-system, BlinkMacSystemFont, sans-serif;
      background-color: var(--bg);
      color: var(--text);
      line-height: 1.55;
      -webkit-font-smoothing: antialiased;
    }

    .container {
      width: 100%;
      max-width: 1120px;
      margin: 0 auto;
      padding: 0 20px;
    }

    /* HEADER */
    header {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(255, 255, 255, 0.94);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--border);
    }

    .nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      height: 72px;
      gap: 12px;
    }

    .brand {
      display: flex;
      flex-direction: column;
      text-decoration: none;
      color: var(--text);
    }

    .brand-name {
      font-size: 18px;
      font-weight: 800;
      letter-spacing: -0.03em;
      line-height: 1.1;
    }

    .brand-sub {
      font-size: 11px;
      font-weight: 600;
      color: var(--text-secondary);
      letter-spacing: 0.04em;
      text-transform: uppercase;
    }

    .nav-menu {
      display: flex;
      gap: 28px;
    }

    .nav-menu a {
      text-decoration: none;
      color: var(--text-secondary);
      font-size: 14px;
      font-weight: 600;
      transition: color 0.2s;
    }

    .nav-menu a:hover {
      color: var(--text);
    }

    .header-contacts {
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .pill-link {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      padding: 9px 14px;
      border-radius: 99px;
      font-size: 13px;
      font-weight: 700;
      text-decoration: none;
      transition: all 0.2s;
    }

    .pill-ig {
      background: var(--surface);
      color: var(--text);
      border: 1px solid var(--border);
    }

    .pill-ig:hover {
      background: var(--surface-alt);
    }

    .pill-wa {
      background: var(--text);
      color: #fff;
    }

    .pill-wa:hover {
      background: var(--accent-warm);
    }

    /* HERO */
    .hero {
      padding: 64px 0 56px;
      border-bottom: 1px solid var(--border);
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.2fr 0.8fr;
      gap: 40px;
      align-items: end;
    }

    .eyebrow {
      display: inline-block;
      font-size: 12px;
      font-weight: 700;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--accent-warm);
      margin-bottom: 16px;
    }

    h1 {
      font-size: clamp(32px, 4.8vw, 54px);
      font-weight: 800;
      line-height: 1.08;
      letter-spacing: -0.03em;
      margin-bottom: 20px;
    }

    .hero-lead {
      font-size: clamp(16px, 1.8vw, 18px);
      color: var(--text-secondary);
      max-width: 540px;
      margin-bottom: 32px;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
    }

    .btn-dark {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      background: var(--text);
      color: #fff;
      padding: 15px 28px;
      border-radius: 12px;
      font-size: 15px;
      font-weight: 700;
      text-decoration: none;
      border: none;
      cursor: pointer;
      transition: background 0.2s, transform 0.15s;
    }

    .btn-dark:hover {
      background: var(--accent-warm);
      transform: translateY(-1px);
    }

    .btn-outline {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      background: transparent;
      color: var(--text);
      padding: 15px 24px;
      border-radius: 12px;
      font-size: 15px;
      font-weight: 700;
      text-decoration: none;
      border: 1px solid var(--border);
      transition: border-color 0.2s, background 0.2s;
    }

    .btn-outline:hover {
      border-color: var(--text);
      background: var(--surface);
    }

    /* SPECIALIST CARD */
    .profile-box {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 20px;
      padding: 28px;
    }

    .profile-top {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding-bottom: 18px;
      margin-bottom: 18px;
      border-bottom: 1px solid var(--border);
    }

    .profile-title {
      font-size: 13px;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      color: var(--text-secondary);
    }

    .status-dot {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      font-size: 12px;
      font-weight: 700;
      color: var(--wa);
    }

    .status-dot::before {
      content: "";
      width: 8px;
      height: 8px;
      border-radius: 50%;
      background: var(--wa);
    }

    .contact-row {
      display: flex;
      flex-direction: column;
      gap: 12px;
    }

    .contact-item {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 14px 16px;
      background: var(--bg);
      border: 1px solid var(--border);
      border-radius: 12px;
      text-decoration: none;
      color: var(--text);
      transition: border-color 0.2s;
    }

    .contact-item:hover {
      border-color: var(--text);
    }

    .contact-label {
      font-size: 12px;
      color: var(--text-secondary);
      display: block;
    }

    .contact-val {
      font-size: 15px;
      font-weight: 800;
    }

    /* APPROACH GRID */
    .section {
      padding: 72px 0;
    }

    .section-header {
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      gap: 20px;
      margin-bottom: 40px;
      flex-wrap: wrap;
    }

    .section-header h2 {
      font-size: clamp(26px, 3.6vw, 38px);
      font-weight: 800;
      letter-spacing: -0.02em;
      line-height: 1.15;
    }

    .section-header p {
      color: var(--text-secondary);
      max-width: 440px;
      font-size: 15px;
    }

    .grid-4 {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 16px;
    }

    .info-card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 24px;
    }

    .info-num {
      font-size: 12px;
      font-weight: 800;
      color: var(--accent-warm);
      margin-bottom: 14px;
      display: block;
    }

    .info-card h3 {
      font-size: 17px;
      font-weight: 800;
      margin-bottom: 8px;
    }

    .info-card p {
      font-size: 14px;
      color: var(--text-secondary);
    }

    /* TARIFF TABS SECTION */
    .tariffs-section {
      background: var(--surface);
      border-top: 1px solid var(--border);
      border-bottom: 1px solid var(--border);
    }

    .tabs-bar {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
      background: var(--bg);
      padding: 8px;
      border-radius: 16px;
      border: 1px solid var(--border);
      margin-bottom: 28px;
    }

    .tab-btn {
      padding: 16px 12px;
      border: none;
      border-radius: 11px;
      background: transparent;
      color: var(--text-secondary);
      font-family: inherit;
      cursor: pointer;
      text-align: center;
      transition: all 0.2s;
    }

    .tab-btn strong {
      display: block;
      font-size: 20px;
      font-weight: 800;
      color: var(--text);
      line-height: 1.2;
    }

    .tab-btn span {
      font-size: 12px;
      font-weight: 600;
    }

    .tab-btn.active {
      background: var(--text);
      color: #fff;
    }

    .tab-btn.active strong {
      color: #fff;
    }

    .tab-btn.active span {
      color: rgba(255, 255, 255, 0.75);
    }

    .tab-panel {
      display: none;
      background: var(--bg);
      border: 1px solid var(--border);
      border-radius: 22px;
      padding: 32px;
    }

    .tab-panel.active {
      display: block;
    }

    .panel-top {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      gap: 20px;
      padding-bottom: 24px;
      margin-bottom: 24px;
      border-bottom: 1px solid var(--border);
      flex-wrap: wrap;
    }

    .panel-title {
      font-size: 24px;
      font-weight: 800;
      margin-bottom: 4px;
    }

    .panel-desc {
      font-size: 14px;
      color: var(--text-secondary);
    }

    .badge-included {
      background: #EAF6EE;
      color: var(--wa);
      font-size: 13px;
      font-weight: 800;
      padding: 8px 14px;
      border-radius: 10px;
    }

    .duration-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 16px;
    }

    .duration-card {
      border: 1.5px solid var(--border);
      border-radius: 16px;
      padding: 24px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      transition: border-color 0.2s, transform 0.2s;
    }

    .duration-card:hover {
      border-color: var(--text);
      transform: translateY(-2px);
    }

    .duration-card.featured {
      border-color: var(--accent-warm);
      background: #FFFDFB;
    }

    .dur-tag {
      font-size: 11px;
      font-weight: 800;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      color: var(--accent-warm);
      margin-bottom: 8px;
      display: block;
    }

    .dur-days {
      font-size: 18px;
      font-weight: 800;
      margin-bottom: 6px;
    }

    .dur-price {
      font-size: 28px;
      font-weight: 800;
      letter-spacing: -0.02em;
      margin-bottom: 6px;
    }

    .dur-note {
      font-size: 13px;
      color: var(--text-secondary);
      margin-bottom: 20px;
    }

    .btn-select {
      width: 100%;
      padding: 13px;
      border-radius: 10px;
      border: 1px solid var(--text);
      background: var(--text);
      color: #fff;
      font-family: inherit;
      font-size: 14px;
      font-weight: 700;
      cursor: pointer;
      transition: background 0.2s, border-color 0.2s;
    }

    .btn-select:hover {
      background: var(--accent-warm);
      border-color: var(--accent-warm);
    }

    /* CONSULTATION FORM */
    .order-wrap {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 40px;
      align-items: center;
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 24px;
      padding: 40px;
    }

    .order-wrap h2 {
      font-size: clamp(24px, 3vw, 32px);
      font-weight: 800;
      letter-spacing: -0.02em;
      margin-bottom: 12px;
    }

    .order-wrap p {
      color: var(--text-secondary);
      font-size: 15px;
      margin-bottom: 24px;
    }

    .direct-links {
      display: flex;
      flex-direction: column;
      gap: 10px;
      font-size: 14px;
      font-weight: 700;
    }

    .direct-links a {
      color: var(--text);
      text-decoration: none;
    }

    .direct-links a:hover {
      color: var(--accent-warm);
    }

    .form-panel {
      background: var(--bg);
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 28px;
    }

    .field {
      margin-bottom: 14px;
    }

    .field label {
      display: block;
      font-size: 13px;
      font-weight: 700;
      margin-bottom: 6px;
    }

    .field input,
    .field select {
      width: 100%;
      padding: 13px 14px;
      border-radius: 10px;
      border: 1px solid var(--border);
      font-family: inherit;
      font-size: 14px;
      color: var(--text);
      background: var(--bg);
      outline: none;
    }

    .field input:focus,
    .field select:focus {
      border-color: var(--text);
    }

    /* FOOTER */
    footer {
      border-top: 1px solid var(--border);
      padding: 36px 0;
      font-size: 13px;
      color: var(--text-secondary);
    }

    .footer-inner {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 16px;
    }

    .footer-links {
      display: flex;
      gap: 20px;
    }

    .footer-links a {
      color: var(--text);
      font-weight: 700;
      text-decoration: none;
    }

    /* RESPONSIVE */
    @media (max-width: 900px) {
      .hero-grid,
      .order-wrap {
        grid-template-columns: 1fr;
      }
      .grid-4 {
        grid-template-columns: repeat(2, 1fr);
      }
      .duration-grid {
        grid-template-columns: 1fr;
      }
      .nav-menu {
        display: none;
      }
    }

    @media (max-width: 560px) {
      .hero {
        padding: 40px 0;
      }
      .grid-4 {
        grid-template-columns: 1fr;
      }
      .tab-panel {
        padding: 20px;
      }
      .order-wrap {
        padding: 24px 18px;
      }
      .pill-ig span {
        display: none;
      }
    }
  </style>
</head>
<body>

  <!-- HEADER -->
  <header>
    <div class="container nav">
      <a href="#" class="brand">
        <span class="brand-name">BAGI SMM</span>
        <span class="brand-sub">Target & Meta Ads</span>
      </a>

      <nav class="nav-menu">
        <a href="#approach">Преимущества</a>
        <a href="#tariffs">Тарифы</a>
        <a href="#consult">Консультация</a>
      </nav>

      <div class="header-contacts">
        <a href="https://instagram.com/bagi_8739" target="_blank" class="pill-link pill-ig">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2"><rect x="2" y="2" width="20" height="20" rx="5"/><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"/></svg>
          <span>@bagi_8739</span>
        </a>
        <a href="https://wa.me/996704515121" target="_blank" class="pill-link pill-wa">
          WhatsApp
        </a>
      </div>
    </div>
  </header>

  <!-- HERO -->
  <section class="hero">
    <div class="container hero-grid">
      <div>
        <span class="eyebrow">Instagram & Meta Business</span>
        <h1>Таргетированная реклама для роста ваших продаж</h1>
        <p class="hero-lead">
          Привлекайте целевых клиентов и стабильный поток заявок каждый день. Работа по настройке и ведению рекламы уже включена в стоимость каждого тарифа.
        </p>
        <div class="hero-actions">
          <a href="#tariffs" class="btn-dark">Выбрать тариф</a>
          <a href="https://wa.me/996704515121?text=Здравствуйте! Хочу обсудить запуск таргетированной рекламы." target="_blank" class="btn-outline">Написать в WhatsApp</a>
        </div>
      </div>

      <div class="profile-box">
        <div class="profile-top">
          <span class="profile-title">Контакты специалиста</span>
          <span class="status-dot">На связи</span>
        </div>
        <div class="contact-row">
          <a href="https://instagram.com/bagi_8739" target="_blank" class="contact-item">
            <div>
              <span class="contact-label">Instagram профиль</span>
              <span class="contact-val">@bagi_8739</span>
            </div>
            <span>→</span>
          </a>
          <a href="https://wa.me/996704515121" target="_blank" class="contact-item">
            <div>
              <span class="contact-label">WhatsApp для заявок</span>
              <span class="contact-val">+996 704 515 121</span>
            </div>
            <span>→</span>
          </a>
        </div>
      </div>
    </div>
  </section>

  <!-- APPROACH -->
  <section class="section" id="approach">
    <div class="container">
      <div class="section-header">
        <h2>Профессиональный подход к рекламе</h2>
        <p>Инвестируйте бюджет разумно: прозрачные условия, понятные сроки и сопровождение на каждом этапе.</p>
      </div>

      <div class="grid-4">
        <div class="info-card">
          <span class="info-num">01</span>
          <h3>Точный таргетинг</h3>
          <p>Сегментация по интересам, географии и поведению именно вашей платежеспособной аудитории.</p>
        </div>
        <div class="info-card">
          <span class="info-num">02</span>
          <h3>Больше заявок и продаж</h3>
          <p>Настройка рекламных кампаний на переписки в Instagram Direct и переходы в WhatsApp.</p>
        </div>
        <div class="info-card">
          <span class="info-num">03</span>
          <h3>Эффективный бюджет</h3>
          <p>Фиксированная стоимость пакета без скрытых доплат — работа специалиста уже включена.</p>
        </div>
        <div class="info-card">
          <span class="info-num">04</span>
          <h3>Контроль результата</h3>
          <p>Ежедневный мониторинг показателей и корректировка объявлений для лучшей окупаемости.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- TARIFFS WITH SEPARATE TABS -->
  <section class="section tariffs-section" id="tariffs">
    <div class="container">
      <div class="section-header">
        <h2>Тарифы и дневной бюджет</h2>
        <p>Переключайте вкладки бюджета ($3, $5 или $10 в день), чтобы выбрать подходящую длительность запуска.</p>
      </div>

      <!-- TABS NAVIGATION -->
      <div class="tabs-bar" role="tablist">
        <button class="tab-btn active" onclick="openTab(event, 'tab-3')">
          <strong>$3 / день</strong>
          <span>Базовый старт</span>
        </button>
        <button class="tab-btn" onclick="openTab(event, 'tab-5')">
          <strong>$5 / день</strong>
          <span>Оптимальный</span>
        </button>
        <button class="tab-btn" onclick="openTab(event, 'tab-10')">
          <strong>$10 / день</strong>
          <span>Максимальный охват</span>
        </button>
      </div>

      <!-- TAB $3 -->
      <div class="tab-panel active" id="tab-3">
        <div class="panel-top">
          <div>
            <div class="panel-title">Дневной бюджет — $3 в сутки</div>
            <div class="panel-desc">Подходит для тестирования ниши, локальных услуг и небольших магазинов.</div>
          </div>
          <div class="badge-included">Услуга ичинде (всё включено)</div>
        </div>

        <div class="duration-grid">
          <div class="duration-card">
            <div>
              <span class="dur-tag">Тестовый запуск</span>
              <div class="dur-days">3 күнгө (3 дня)</div>
              <div class="dur-price">1 300 сом</div>
              <div class="dur-note">Рекламный бюджет + работа таргетолога</div>
            </div>
            <button class="btn-select" onclick="orderTariff('$3 / день', '3 күнгө', '1 300 сом')">Заказать пакет</button>
          </div>

          <div class="duration-card featured">
            <div>
              <span class="dur-tag">Рекомендуемый срок</span>
              <div class="dur-days">5 күнгө (5 дней)</div>
              <div class="dur-price">1 800 сом</div>
              <div class="dur-note">Рекламный бюджет + работа таргетолога</div>
            </div>
            <button class="btn-select" onclick="orderTariff('$3 / день', '5 күнгө', '1 800 сом')">Заказать пакет</button>
          </div>

          <div class="duration-card">
            <div>
              <span class="dur-tag">Недельный цикл</span>
              <div class="dur-days">7 күнгө (7 дней)</div>
              <div class="dur-price">2 400 сом</div>
              <div class="dur-note">Рекламный бюджет + работа таргетолога</div>
            </div>
            <button class="btn-select" onclick="orderTariff('$3 / день', '7 күнгө', '2 400 сом')">Заказать пакет</button>
          </div>
        </div>
      </div>

      <!-- TAB $5 -->
      <div class="tab-panel" id="tab-5">
        <div class="panel-top">
          <div>
            <div class="panel-title">Дневной бюджет — $5 в сутки</div>
            <div class="panel-desc">Сбалансированный темп показов для стабильного потока заявок и продаж.</div>
          </div>
          <div class="badge-included">Услуга ичинде (всё включено)</div>
        </div>

        <div class="duration-grid">
          <div class="duration-card">
            <div>
              <span class="dur-tag">Быстрый старт</span>
              <div class="dur-days">3 күнгө (3 дня)</div>
              <div class="dur-price">1 800 сом</div>
              <div class="dur-note">Рекламный бюджет + работа таргетолога</div>
            </div>
            <button class="btn-select" onclick="orderTariff('$5 / день', '3 күнгө', '1 800 сом')">Заказать пакет</button>
          </div>

          <div class="duration-card featured">
            <div>
              <span class="dur-tag">Выбор клиентов</span>
              <div class="dur-days">5 күнгө (5 дней)</div>
              <div class="dur-price">2 700 сом</div>
              <div class="dur-note">Рекламный бюджет + работа таргетолога</div>
            </div>
            <button class="btn-select" onclick="orderTariff('$5 / день', '5 күнгө', '2 700 сом')">Заказать пакет</button>
          </div>

          <div class="duration-card">
            <div>
              <span class="dur-tag">Полная неделя</span>
              <div class="dur-days">7 күнгө (7 дней)</div>
              <div class="dur-price">3 500 сом</div>
              <div class="dur-note">Рекламный бюджет + работа таргетолога</div>
            </div>
            <button class="btn-select" onclick="orderTariff('$5 / день', '7 күнгө', '3 500 сом')">Заказать пакет</button>
          </div>
        </div>
      </div>

      <!-- TAB $10 -->
      <div class="tab-panel" id="tab-10">
        <div class="panel-top">
          <div>
            <div class="panel-title">Дневной бюджет — $10 в сутки</div>
            <div class="panel-desc">Усиленное продвижение для масштабирования продаж, акций и крупных запусков.</div>
          </div>
          <div class="badge-included">Услуга ичинде (всё включено)</div>
        </div>

        <div class="duration-grid">
          <div class="duration-card">
            <div>
              <span class="dur-tag">Интенсив</span>
              <div class="dur-days">3 күнгө (3 дня)</div>
              <div class="dur-price">2 650 сом</div>
              <div class="dur-note">Рекламный бюджет + работа таргетолога</div>
            </div>
            <button class="btn-select" onclick="orderTariff('$10 / день', '3 күнгө', '2 650 сом')">Заказать пакет</button>
          </div>

          <div class="duration-card featured">
            <div>
              <span class="dur-tag">Высокий поток</span>
              <div class="dur-days">5 күнгө (5 дней)</div>
              <div class="dur-price">4 880 сом</div>
              <div class="dur-note">Рекламный бюджет + работа таргетолога</div>
            </div>
            <button class="btn-select" onclick="orderTariff('$10 / день', '5 күнгө', '4 880 сом')">Заказать пакет</button>
          </div>

          <div class="duration-card">
            <div>
              <span class="dur-tag">Максимум</span>
              <div class="dur-days">7 күнгө (7 дней)</div>
              <div class="dur-price">6 650 сом</div>
              <div class="dur-note">Рекламный бюджет + работа таргетолога</div>
            </div>
            <button class="btn-select" onclick="orderTariff('$10 / день', '7 күнгө', '6 650 сом')">Заказать пакет</button>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- CONSULTATION FORM -->
  <section class="section" id="consult">
    <div class="container">
      <div class="order-wrap">
        <div>
          <h2>Инвестируйте разумно — развивайте свой бизнес</h2>
          <p>Не знаете, какой бюджет выбрать? Оставьте заявку, и я помогу подобрать оптимальный пакет под вашу нишу и цели.</p>
          <div class="direct-links">
            <a href="https://instagram.com/bagi_8739" target="_blank">Instagram: @bagi_8739</a>
            <a href="https://wa.me/996704515121" target="_blank">WhatsApp: +996 704 515 121</a>
          </div>
        </div>

        <div class="form-panel">
          <div class="field">
            <label>Ваше имя</label>
            <input type="text" id="fName" placeholder="Введите ваше имя">
          </div>
          <div class="field">
            <label>Ссылка на Instagram или сфера бизнеса</label>
            <input type="text" id="fInst" placeholder="@ваш_аккаунт">
          </div>
          <div class="field">
            <label>Интересующий тариф</label>
            <select id="fTariff">
              <option value="$3/день — 3 күнгө (1 300 сом)">$3/день — 3 күнгө (1 300 сом)</option>
              <option value="$3/день — 5 күнгө (1 800 сом)">$3/день — 5 күнгө (1 800 сом)</option>
              <option value="$3/день — 7 күнгө (2 400 сом)">$3/день — 7 күнгө (2 400 сом)</option>
              <option value="$5/день — 3 күнгө (1 800 сом)">$5/день — 3 күнгө (1 800 сом)</option>
              <option value="$5/день — 5 күнгө (2 700 сом)" selected>$5/день — 5 күнгө (2 700 сом)</option>
              <option value="$5/день — 7 күнгө (3 500 сом)">$5/день — 7 күнгө (3 500 сом)</option>
              <option value="$10/день — 3 күнгө (2 650 сом)">$10/день — 3 күнгө (2 650 сом)</option>
              <option value="$10/день — 5 күнгө (4 880 сом)">$10/день — 5 күнгө (4 880 сом)</option>
              <option value="$10/день — 7 күнгө (6 650 сом)">$10/день — 7 күнгө (6 650 сом)</option>
            </select>
          </div>
          <button class="btn-dark" style="width: 100%;" onclick="sendConsultation()">Отправить заявку в WhatsApp</button>
        </div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="container footer-inner">
      <div>© 2026 BAGI SMM — Таргетированная реклама</div>
      <div class="footer-links">
        <a href="https://instagram.com/bagi_8739" target="_blank">Instagram: @bagi_8739</a>
        <a href="https://wa.me/996704515121" target="_blank">+996 704 515 121</a>
      </div>
    </div>
  </footer>

  <script>
    const WA_PHONE = "996704515121";

    function openTab(evt, tabId) {
      document.querySelectorAll('.tab-panel').forEach(p => p.classList.remove('active'));
      document.querySelectorAll('.tab-btn').forEach(b => b.classList.remove('active'));
      document.getElementById(tabId).classList.add('active');
      evt.currentTarget.classList.add('active');
    }

    function orderTariff(budget, days, price) {
      const msg = `Здравствуйте! Хочу заказать таргетированную рекламу:\n• Бюджет: ${budget}\n• Срок: ${days}\n• Стоимость: ${price} (Услуга ичинде)`;
      window.open(`https://wa.me/${WA_PHONE}?text=${encodeURIComponent(msg)}`, '_blank');
    }

    function sendConsultation() {
      const name = document.getElementById('fName').value.trim() || 'Не указано';
      const inst = document.getElementById('fInst').value.trim() || 'Не указано';
      const tariff = document.getElementById('fTariff').value;
      const msg = `Здравствуйте! Заявка с сайта:\n• Имя: ${name}\n• Instagram: ${inst}\n• Тариф: ${tariff}`;
      window.open(`https://wa.me/${WA_PHONE}?text=${encodeURIComponent(msg)}`, '_blank');
    }
  </script>
</body>
</html>
