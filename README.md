<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bagi SMM — Профессиональный таргетинг в Instagram</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #0B0F19;
      --card-bg: rgba(17, 24, 39, 0.75);
      --border: rgba(255, 255, 255, 0.08);
      --text: #F3F4F6;
      --muted: #9CA3AF;
      --primary-grad: linear-gradient(135deg, #FF2E93 0%, #FF8A00 50%, #833AB4 100%);
      --accent: #FF2E93;
      --wa: #25D366;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; font-family: 'Plus Jakarta Sans', sans-serif; -webkit-tap-highlight-color: transparent; }
    html { scroll-behavior: smooth; }
    body { background-color: var(--bg); color: var(--text); line-height: 1.6; overflow-x: hidden; }

    .container { width: 100%; max-width: 1100px; margin: 0 auto; padding: 0 20px; }

    /* HEADER */
    header {
      position: fixed; top: 0; left: 0; width: 100%; z-index: 100;
      background: rgba(11, 15, 25, 0.85);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      border-bottom: 1px solid var(--border);
    }
    .nav { display: flex; justify-content: space-between; align-items: center; height: 74px; }
    .logo { font-weight: 800; font-size: 20px; color: #fff; text-decoration: none; display: flex; align-items: center; gap: 10px; }
    .logo-dot { width: 10px; height: 10px; border-radius: 50%; background: var(--accent); box-shadow: 0 0 12px var(--accent); }
    .nav-inst {
      background: rgba(255, 255, 255, 0.06); border: 1px solid var(--border);
      color: #fff; padding: 8px 16px; border-radius: 12px; text-decoration: none;
      font-weight: 700; font-size: 14px; display: flex; align-items: center; gap: 8px;
      transition: background 0.2s;
    }
    .nav-inst:hover { background: rgba(255, 255, 255, 0.12); }

    /* HERO */
    .hero {
      padding: 140px 0 80px; text-align: center; position: relative;
      background: radial-gradient(circle at 50% 20%, rgba(131, 58, 180, 0.2) 0%, transparent 60%);
    }
    .badge {
      display: inline-flex; align-items: center; gap: 8px; padding: 6px 16px; border-radius: 99px;
      background: rgba(255, 46, 147, 0.1); border: 1px solid rgba(255, 46, 147, 0.3);
      color: #FF70B5; font-weight: 700; font-size: 13px; margin-bottom: 22px;
      text-transform: uppercase; letter-spacing: 0.05em;
    }
    h1 { font-size: clamp(34px, 5vw, 56px); font-weight: 800; line-height: 1.15; margin-bottom: 20px; letter-spacing: -0.02em; }
    .grad-text { background: var(--primary-grad); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
    .hero-sub { color: var(--muted); font-size: clamp(16px, 2vw, 19px); max-width: 600px; margin: 0 auto 36px; }

    .hero-btns { display: flex; justify-content: center; gap: 16px; flex-wrap: wrap; }
    .btn-main {
      background: var(--primary-grad); color: #fff; padding: 16px 32px; border-radius: 16px;
      font-weight: 800; font-size: 16px; text-decoration: none; box-shadow: 0 10px 30px rgba(255, 46, 147, 0.35);
      transition: transform 0.2s, box-shadow 0.2s; display: inline-flex; align-items: center; gap: 8px;
    }
    .btn-main:hover { transform: translateY(-3px); box-shadow: 0 15px 35px rgba(255, 46, 147, 0.5); }
    .btn-sec {
      background: rgba(255, 255, 255, 0.05); border: 1px solid var(--border); color: #fff;
      padding: 16px 28px; border-radius: 16px; font-weight: 700; font-size: 16px; text-decoration: none;
      transition: background 0.2s; display: inline-flex; align-items: center; gap: 8px;
    }
    .btn-sec:hover { background: rgba(255, 255, 255, 0.1); }

    /* PERKS */
    .perks { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 20px; margin: 60px 0; }
    .perk-card {
      background: var(--card-bg); border: 1px solid var(--border); border-radius: 20px; padding: 24px;
      backdrop-filter: blur(10px); transition: border-color 0.2s, transform 0.2s;
    }
    .perk-card:hover { border-color: rgba(255, 46, 147, 0.4); transform: translateY(-4px); }
    .perk-icon { font-size: 28px; margin-bottom: 14px; }
    .perk-card h3 { font-size: 17px; font-weight: 700; margin-bottom: 6px; color: #fff; }
    .perk-card p { font-size: 14px; color: var(--muted); }

    /* PRICING SECTION */
    .section-title { text-align: center; font-size: clamp(28px, 4vw, 38px); font-weight: 800; margin-bottom: 12px; }
    .section-desc { text-align: center; color: var(--muted); font-size: 16px; margin-bottom: 50px; }

    .pricing-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 24px; margin-bottom: 80px; }
    .price-card {
      background: var(--card-bg); border: 1px solid var(--border); border-radius: 24px; padding: 30px 24px;
      display: flex; flex-direction: column; position: relative; backdrop-filter: blur(10px);
      transition: transform 0.25s, border-color 0.25s;
    }
    .price-card:hover { transform: translateY(-6px); border-color: rgba(255, 138, 0, 0.5); }
    .price-card.popular { border-color: var(--accent); background: linear-gradient(180deg, rgba(255, 46, 147, 0.08) 0%, rgba(17, 24, 39, 0.8) 100%); }
    
    .popular-badge {
      position: absolute; top: -14px; right: 24px; background: var(--primary-grad);
      color: #fff; font-size: 11px; font-weight: 800; padding: 5px 14px; border-radius: 99px; text-transform: uppercase;
    }

    .budget-top { display: flex; justify-content: space-between; align-items: center; margin-bottom: 14px; }
    .budget-val { font-size: 44px; font-weight: 900; background: var(--primary-grad); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
    .budget-lbl { font-size: 13px; font-weight: 700; color: var(--muted); background: rgba(255,255,255,0.05); padding: 6px 12px; border-radius: 10px; }

    .service-incl {
      display: inline-block; font-size: 13px; font-weight: 700; color: #10B981; background: rgba(16, 185, 129, 0.1);
      border: 1px solid rgba(16, 185, 129, 0.2); padding: 6px 12px; border-radius: 10px; margin-bottom: 24px; width: fit-content;
    }

    .options-list { display: flex; flex-direction: column; gap: 10px; margin-bottom: 28px; flex-grow: 1; }
    .option-item {
      display: flex; justify-content: space-between; align-items: center; padding: 14px 16px;
      border-radius: 14px; border: 1.5px solid var(--border); background: rgba(255,255,255,0.02);
      cursor: pointer; transition: all 0.2s;
    }
    .option-item:hover { border-color: rgba(255,255,255,0.2); background: rgba(255,255,255,0.05); }
    .option-item.active { border-color: var(--accent); background: rgba(255, 46, 147, 0.08); }
    
    .opt-left { font-weight: 700; font-size: 15px; display: flex; align-items: center; gap: 10px; color: #fff; }
    .radio-circle { width: 18px; height: 18px; border-radius: 50%; border: 2px solid var(--muted); display: flex; align-items: center; justify-content: center; }
    .option-item.active .radio-circle { border-color: var(--accent); }
    .option-item.active .radio-circle::after { content: ''; width: 8px; height: 8px; border-radius: 50%; background: var(--accent); }
    .opt-price { font-weight: 800; font-size: 16px; color: #fff; }

    .btn-card-order {
      width: 100%; background: rgba(255,255,255,0.08); border: 1px solid var(--border); color: #fff;
      padding: 15px; border-radius: 14px; font-weight: 800; font-size: 15px; cursor: pointer;
      display: flex; align-items: center; justify-content: center; gap: 8px; transition: background 0.2s, transform 0.2s;
    }
    .price-card.popular .btn-card-order { background: var(--primary-grad); border: none; box-shadow: 0 8px 20px rgba(255,46,147,0.3); }
    .btn-card-order:hover { transform: translateY(-2px); opacity: 0.95; }

    /* CTA FORM */
    .cta-container {
      background: linear-gradient(135deg, rgba(255,46,147,0.12) 0%, rgba(131,58,180,0.12) 100%);
      border: 1px solid rgba(255, 46, 147, 0.3); border-radius: 32px; padding: 50px 40px;
      display: grid; grid-template-columns: 1fr 1fr; gap: 40px; align-items: center; margin-bottom: 80px;
    }
    .cta-text h2 { font-size: clamp(26px, 3.5vw, 36px); font-weight: 800; margin-bottom: 14px; }
    .cta-text p { color: var(--muted); font-size: 16px; margin-bottom: 20px; }
    .cta-quote { font-weight: 700; color: #FF70B5; font-size: 18px; }

    .form-box { background: rgba(11, 15, 25, 0.8); border: 1px solid var(--border); border-radius: 24px; padding: 30px; }
    .form-group { margin-bottom: 16px; }
    .form-group label { display: block; font-size: 13px; font-weight: 700; margin-bottom: 8px; color: var(--muted); }
    .form-input, .form-select {
      width: 100%; padding: 14px 18px; border-radius: 14px; border: 1.5px solid var(--border);
      background: rgba(255,255,255,0.03); color: #fff; font-size: 15px; outline: none; transition: border-color 0.2s;
    }
    .form-input:focus, .form-select:focus { border-color: var(--accent); }
    .form-select option { background: #111827; color: #fff; }

    .btn-submit-wa {
      width: 100%; background: var(--wa); color: #fff; border: none; padding: 16px; border-radius: 14px;
      font-weight: 800; font-size: 16px; cursor: pointer; display: flex; align-items: center; justify-content: center; gap: 10px;
      box-shadow: 0 10px 25px rgba(37, 211, 102, 0.3); transition: transform 0.2s; margin-top: 10px;
    }
    .btn-submit-wa:hover { transform: translateY(-2px); }

    /* FOOTER */
    footer { border-top: 1px solid var(--border); padding: 40px 0; text-align: center; color: var(--muted); font-size: 14px; }
    footer a { color: #fff; text-decoration: none; font-weight: 700; }

    /* RESPONSIVE */
    @media(max-width: 900px) {
      .pricing-grid { grid-template-columns: 1fr; max-width: 460px; margin: 0 auto 60px; }
      .cta-container { grid-template-columns: 1fr; padding: 30px 20px; }
    }
  </style>
</head>
<body>

  <!-- HEADER -->
  <header>
    <div class="container nav">
      <a href="#" class="logo">
        <span class="logo-dot"></span> Bagi SMM
      </a>
      <a href="https://instagram.com/bagi_8739" target="_blank" class="nav-inst">
        📸 Instagram: @bagi_8739
      </a>
    </div>
  </header>

  <!-- HERO SECTION -->
  <section class="hero">
    <div class="container">
      <div class="badge">🔥 Профессиональный таргетинг в Instagram</div>
      <h1>Привлекайте больше <span class="grad-text">клиентов и продаж</span></h1>
      <p class="hero-sub">Качественная настройка таргетированной рекламы под ключ. Точное попадание в вашу целевую аудиторию и рост вашего дохода[span_1](start_span)[span_1](end_span).</p>
      <div class="hero-btns">
        <a href="#pricing" class="btn-main">🚀 Выбрать тариф</a>
        <a href="https://wa.me/996704515121?text=Здравствуйте! Хочу заказать таргетированную рекламу." target="_blank" class="btn-sec">💬 Написать в WhatsApp</a>
      </div>

      <!-- PERKS -->
      <div class="perks">
        <div class="perk-card">
          <div class="perk-icon">🎯</div>
          <h3>Точный таргетинг</h3>
          <p>Настройка на горячую аудиторию, которая готова покупать ваш продукт[span_2](start_span)[span_2](end_span).</p>
        </div>
        <div class="perk-card">
          <div class="perk-icon">📈</div>
          <h3>Рост заявок</h3>
          <p>Постоянный поток клиентов в ваш Instagram Direct и WhatsApp[span_3](start_span)[span_3](end_span).</p>
        </div>
        <div class="perk-card">
          <div class="perk-icon">🛡️</div>
          <h3>Услуга ичинде</h3>
          <p>Полное сопровождение и профессиональная оптимизация рекламного бюджета[span_4](start_span)[span_4](end_span).</p>
        </div>
      </div>
    </div>
  </section>

  <!-- PRICING SECTION -->
  <section class="container" id="pricing" style="padding: 40px 0 80px;">
    <h2 class="section-title">Тарифы на рекламу</h2>
    <p class="section-desc">Выберите удобный дневной бюджет и срок запуска. Нажмите кнопку, чтобы заказать в WhatsApp.</p>

    <div class="pricing-grid">
      <!-- $3 -->
      <div class="price-card" data-budget="$3 в день">
        <div class="budget-top">
          <div class="budget-val">$3</div>
          <div class="budget-lbl">Бюджет / день</div>
        </div>
        <div class="service-incl">✅ Услуга ичинде</div>

        <div class="options-list">
          <div class="option-item active" onclick="selectOpt(this, '3 күнгө (1 300 сом)')">
            <div class="opt-left"><span class="radio-circle"></span> 3 күнгө</div>
            <div class="opt-price">1 300 сом</div>
          </div>
          <div class="option-item" onclick="selectOpt(this, '5 күнгө (1 800 сом)')">
            <div class="opt-left"><span class="radio-circle"></span> 5 күнгө</div>
            <div class="opt-price">1 800 сом</div>
          </div>
          <div class="option-item" onclick="selectOpt(this, '7 күнгө (2 400 сом)')">
            <div class="opt-left"><span class="radio-circle"></span> 7 күнгө</div>
            <div class="opt-price">2 400 сом</div>
          </div>
        </div>

        <button class="btn-card-order" onclick="orderCard(this)">📲 Заказать в WhatsApp</button>
      </div>

      <!-- $5 (Popular) -->
      <div class="price-card popular" data-budget="$5 в день">
        <div class="popular-badge">Хит продаж 🔥</div>
        <div class="budget-top">
          <div class="budget-val">$5</div>
          <div class="budget-lbl">Бюджет / день</div>
        </div>
        <div class="service-incl">✅ Услуга ичинде</div>

        <div class="options-list">
          <div class="option-item" onclick="selectOpt(this, '3 күнгө (1 800 сом)')">
            <div class="opt-left"><span class="radio-circle"></span> 3 күнгө</div>
            <div class="opt-price">1 800 сом</div>
          </div>
          <div class="option-item active" onclick="selectOpt(this, '5 күнгө (2 700 сом)')">
            <div class="opt-left"><span class="radio-circle"></span> 5 күнгө</div>
            <div class="opt-price">2 700 сом</div>
          </div>
          <div class="option-item" onclick="selectOpt(this, '7 күнгө (3 500 сом)')">
            <div class="opt-left"><span class="radio-circle"></span> 7 күнгө</div>
            <div class="opt-price">3 500 сом</div>
          </div>
        </div>

        <button class="btn-card-order" onclick="orderCard(this)">📲 Заказать в WhatsApp</button>
      </div>

      <!-- $10 -->
      <div class="price-card" data-budget="$10 в день">
        <div class="budget-top">
          <div class="budget-val">$10</div>
          <div class="budget-lbl">Бюджет / день</div>
        </div>
        <div class="service-incl">✅ Услуга ичинде</div>

        <div class="options-list">
          <div class="option-item active" onclick="selectOpt(this, '3 күнгө (2 650 сом)')">
            <div class="opt-left"><span class="radio-circle"></span> 3 күнгө</div>
            <div class="opt-price">2 650 сом</div>
          </div>
          <div class="option-item" onclick="selectOpt(this, '5 күнгө (4 880 сом)')">
            <div class="opt-left"><span class="radio-circle"></span> 5 күнгө</div>
            <div class="opt-price">4 880 сом</div>
          </div>
          <div class="option-item" onclick="selectOpt(this, '7 күнгө (6 650 сом)')">
            <div class="opt-left"><span class="radio-circle"></span> 7 күнгө</div>
            <div class="opt-price">6 650 сом</div>
          </div>
        </div>

        <button class="btn-card-order" onclick="orderCard(this)">📲 Заказать в WhatsApp</button>
      </div>
    </div>

    <!-- CTA FORM CONTAINER -->
    <div class="cta-container">
      <div class="cta-text">
        <h2>Инвестируйте в рекламу правильно! ❤️</h2>
        <p>Оставьте свои данные, и я подберу идеальную стратегию для продвижения вашего бизнеса в Instagram.</p>
        <div class="cta-quote">✨ Ваш успех в наших руках!</div>
      </div>
      <div class="form-box">
        <div class="form-group">
          <label>Ваше имя</label>
          <input type="text" id="clientName" class="form-input" placeholder="Например: Айгерим">
        </div>
        <div class="form-group">
          <label>Ваш Instagram или ниша</label>
          <input type="text" id="clientInst" class="form-input" placeholder="@instagram или магазин одежды">
        </div>
        <div class="form-group">
          <label>Выбрать тариф</label>
          <select id="clientTariff" class="form-select">
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
        <button class="btn-submit-wa" onclick="sendForm()">💬 Отправить заявку в WhatsApp</button>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="container">
      <p>© 2026 Bagi SMM — Таргетированная реклама в Instagram (<a href="https://instagram.com/bagi_8739" target="_blank">@bagi_8739</a>)</p>
    </div>
  </footer>

  <script>
    const PHONE = "996704515121";

    function selectOpt(element, text) {
      const card = element.closest('.price-card');
      card.querySelectorAll('.option-item').forEach(el => el.classList.remove('active'));
      element.classList.add('active');
    }

    function orderCard(btn) {
      const card = btn.closest('.price-card');
      const budget = card.dataset.budget;
      const activeOpt = card.querySelector('.option-item.active');
      const term = activeOpt.querySelector('.opt-left').innerText.trim();
      const price = activeOpt.querySelector('.opt-price').innerText.trim();

      const text = `Здравствуйте! Хочу заказать таргет у Bagi SMM:\n• Бюджет: ${budget}\n• Срок: ${term}\n• Стоимость: ${price} (Услуга ичинде)`;
      window.open(`https://wa.me/${PHONE}?text=${encodeURIComponent(text)}`, '_blank');
    }

    function sendForm() {
      const name = document.getElementById('clientName').value.trim() || 'Не указано';
      const inst = document.getElementById('clientInst').value.trim() || 'Не указано';
      const tariff = document.getElementById('clientTariff').value;

      const text = `Здравствуйте! Заявка с сайта Bagi SMM:\n• Имя: ${name}\n• Инстаграм/Ниша: ${inst}\n• Выбранный пакет: ${tariff}`;
      window.open(`https://wa.me/${PHONE}?text=${encodeURIComponent(text)}`, '_blank');
    }
  </script>
</body>
</html>
