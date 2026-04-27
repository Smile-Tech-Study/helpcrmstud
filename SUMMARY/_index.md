---
title: Содержание
order: 0.3
---

[html]

<style>
@import url('https://fonts.googleapis.com/css2?family=Onest:wght@300;400;500;600&display=swap');

.sp-wrap {
  font-family: 'Onest', sans-serif;
  max-width: 860px;
  margin: 0 auto;
  padding: 0 0 48px;
  color: #1a1a2e;
}

.sp-hero {
  background: linear-gradient(135deg, #0f3460 0%, #16213e 60%, #0f3460 100%);
  border-radius: 16px;
  padding: 48px 40px;
  margin-bottom: 40px;
  position: relative;
  overflow: hidden;
}

.sp-hero::before {
  content: '';
  position: absolute;
  top: -60px; right: -60px;
  width: 240px; height: 240px;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(99,179,237,0.15) 0%, transparent 70%);
}

.sp-hero::after {
  content: '';
  position: absolute;
  bottom: -40px; left: 40px;
  width: 160px; height: 160px;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(56,130,221,0.12) 0%, transparent 70%);
}

.sp-logo {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 24px;
}

.sp-logo-dot {
  width: 32px; height: 32px;
  border-radius: 50%;
  background: linear-gradient(135deg, #378ADD, #63b3ed);
  display: flex; align-items: center; justify-content: center;
  font-size: 16px;
}

.sp-logo-text {
  font-size: 13px;
  font-weight: 500;
  color: rgba(255,255,255,0.6);
  letter-spacing: .08em;
  text-transform: uppercase;
}

.sp-hero h1 {
  font-size: 28px;
  font-weight: 600;
  color: #fff;
  margin: 0 0 12px;
  line-height: 1.3;
  position: relative;
  z-index: 1;
}

.sp-hero p {
  font-size: 15px;
  color: rgba(255,255,255,0.65);
  margin: 0 0 28px;
  line-height: 1.6;
  position: relative;
  z-index: 1;
  max-width: 520px;
}

.sp-hero-btn {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  background: #378ADD;
  color: #fff;
  text-decoration: none;
  font-size: 14px;
  font-weight: 500;
  padding: 10px 20px;
  border-radius: 8px;
  transition: background .15s;
  position: relative;
  z-index: 1;
}

.sp-hero-btn:hover { background: #2d6db5; }

.sp-section-title {
  font-size: 11px;
  font-weight: 600;
  letter-spacing: .1em;
  text-transform: uppercase;
  color: #8892a4;
  margin: 0 0 16px;
}

.sp-cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 12px;
  margin-bottom: 40px;
}

.sp-card {
  display: block;
  text-decoration: none;
  background: #fff;
  border: 1px solid #e8ecf2;
  border-radius: 12px;
  padding: 20px;
  transition: border-color .15s, box-shadow .15s, transform .15s;
}

.sp-card:hover {
  border-color: #378ADD;
  box-shadow: 0 4px 16px rgba(55,138,221,0.1);
  transform: translateY(-2px);
}

.sp-card-icon {
  font-size: 24px;
  margin-bottom: 12px;
  display: block;
}

.sp-card-title {
  font-size: 15px;
  font-weight: 600;
  color: #1a1a2e;
  margin: 0 0 6px;
  line-height: 1.3;
}

.sp-card-desc {
  font-size: 13px;
  color: #6b7280;
  margin: 0;
  line-height: 1.5;
}

.sp-card-arrow {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-top: 14px;
}

.sp-card-tag {
  font-size: 11px;
  background: #f0f6ff;
  color: #378ADD;
  padding: 3px 8px;
  border-radius: 20px;
  font-weight: 500;
}

.sp-card-arr {
  color: #c5cdd8;
  font-size: 18px;
  transition: color .15s, transform .15s;
}

.sp-card:hover .sp-card-arr {
  color: #378ADD;
  transform: translateX(3px);
}

.sp-faq-section {
  margin-bottom: 40px;
}

.sp-faq-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 8px;
}

.sp-faq-item {
  display: block;
  text-decoration: none;
  background: #f8fafd;
  border: 1px solid #e8ecf2;
  border-radius: 10px;
  padding: 14px 16px;
  font-size: 14px;
  color: #374151;
  transition: background .15s, border-color .15s;
  display: flex;
  align-items: center;
  gap: 10px;
}

.sp-faq-item:hover {
  background: #eef5fd;
  border-color: #b8d4f0;
  color: #0f3460;
}

.sp-faq-icon { font-size: 16px; flex-shrink: 0; }

.sp-contact {
  background: #f8fafd;
  border: 1px solid #e8ecf2;
  border-radius: 12px;
  padding: 24px 28px;
  display: flex;
  align-items: center;
  gap: 20px;
}

.sp-contact-icon {
  width: 48px; height: 48px;
  border-radius: 50%;
  background: linear-gradient(135deg, #378ADD22, #63b3ed22);
  border: 1px solid #b8d4f0;
  display: flex; align-items: center; justify-content: center;
  font-size: 22px;
  flex-shrink: 0;
}

.sp-contact-text h3 {
  font-size: 15px;
  font-weight: 600;
  color: #1a1a2e;
  margin: 0 0 4px;
}

.sp-contact-text p {
  font-size: 13px;
  color: #6b7280;
  margin: 0;
  line-height: 1.5;
}

@media (max-width: 560px) {
  .sp-hero { padding: 32px 24px; }
  .sp-hero h1 { font-size: 22px; }
  .sp-contact { flex-direction: column; gap: 12px; }
}
</style>

<div class="sp-wrap">

  <div class="sp-hero">
    <h1>Добро пожаловать в справочный центр</h1>
    <p>Здесь вы найдёте ответы на вопросы о работе в личном кабинете: от входа и заполнения данных до получения документа об обучении.</p>
    <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/instrukciya-po-rabote-v-lichnom-kabinete" class="sp-hero-btn">
      📋 Инструкция по работе в ЛК →
    </a>
  </div>

  <p class="sp-section-title">Основные разделы</p>
  <div class="sp-cards">

    <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/instrukciya-po-rabote-v-lichnom-kabinete" class="sp-card">
      <span class="sp-card-icon">🗺️</span>
      <div class="sp-card-title">Путь слушателя в ЛК</div>
      <p class="sp-card-desc">Интерактивная схема всех этапов — от знакомства до завершения обучения</p>
      <div class="sp-card-arrow">
        <span class="sp-card-tag">Интерактивно</span>
        <span class="sp-card-arr">→</span>
      </div>
    </a>

    <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/chasto-zadavaemye-voprosy" class="sp-card">
      <span class="sp-card-icon">💬</span>
      <div class="sp-card-title">Частые вопросы</div>
      <p class="sp-card-desc">Ответы на самые популярные вопросы: вход, документы, оплата, сроки</p>
      <div class="sp-card-arrow">
        <span class="sp-card-tag">FAQ</span>
        <span class="sp-card-arr">→</span>
      </div>
    </a>

    <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/README" class="sp-card">
      <span class="sp-card-icon">🌊</span>
      <div class="sp-card-title">Flow — что это?</div>
      <p class="sp-card-desc">Коротко о системе: зачем нужен личный кабинет и как он устроен</p>
      <div class="sp-card-arrow">
        <span class="sp-card-tag">Введение</span>
        <span class="sp-card-arr">→</span>
      </div>
    </a>

  </div>

  <p class="sp-section-title">Быстрые ответы</p>
  <div class="sp-faq-section">
    <div class="sp-faq-grid">
      <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/pochemu-ya-vkhozhu-po-ssylke-bezopasno-li-eto" class="sp-faq-item">
        <span class="sp-faq-icon">🔒</span> Почему вход по ссылке? Это безопасно?
      </a>
      <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/chasto-zadavaemye-voprosy" class="sp-faq-item">
        <span class="sp-faq-icon">⏰</span> Ссылка для входа не работает
      </a>
      <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/chasto-zadavaemye-voprosy" class="sp-faq-item">
        <span class="sp-faq-icon">📱</span> Как сканировать документы с телефона?
      </a>
      <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/chasto-zadavaemye-voprosy" class="sp-faq-item">
        <span class="sp-faq-icon">💳</span> Как оплатить обучение?
      </a>
      <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/chasto-zadavaemye-voprosy" class="sp-faq-item">
        <span class="sp-faq-icon">🧾</span> Где найти чек об оплате?
      </a>
      <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/chasto-zadavaemye-voprosy" class="sp-faq-item">
        <span class="sp-faq-icon">🏅</span> Где мой документ об окончании?
      </a>
      <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/chasto-zadavaemye-voprosy" class="sp-faq-item">
        <span class="sp-faq-icon">📭</span> Письма приходят на старую почту
      </a>
      <a target="_blank" href="https://www.flow-crm.study/helpcrmstud/chasto-zadavaemye-voprosy" class="sp-faq-item">
        <span class="sp-faq-icon">🕐</span> Как долго проверяются документы?
      </a>
    </div>
  </div>

  <div class="sp-contact">
    <div class="sp-contact-icon">🏛️</div>
    <div class="sp-contact-text">
      <h3>Не нашли ответ?</h3>
      <p>По вопросам обучения, зачисления и документов обращайтесь в вашу образовательную организацию — контакты есть в разделе <strong>«Программа»</strong> в меню личного кабинета. Техподдержка Flow занимается только техническими вопросами внутри системы.</p>
    </div>
  </div>

</div>

[/html]