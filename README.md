# homepage
moon partnersllc homepage
<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Moon Partners | Executive Personal Doctor Service</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;500;600&family=Noto+Serif+JP:wght@300;400;500;600;700&family=Cinzel:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --navy-deep: #0a1628;
    --navy: #102a43;
    --navy-light: #1a3a5c;
    --gold: #c9a961;
    --gold-light: #e6cc8a;
    --gold-dark: #9c7f3e;
    --cream: #f5f1e8;
    --cream-soft: #faf7f0;
    --ink: #1a1a1a;
    --ink-soft: #3a3a3a;
    --pearl: #ffffff;
  }

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  html {
    scroll-behavior: smooth;
  }

  body {
    font-family: 'Noto Serif JP', serif;
    color: var(--ink);
    background: var(--cream-soft);
    line-height: 1.8;
    overflow-x: hidden;
  }

  .display-font {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 300;
    letter-spacing: 0.02em;
  }

  .accent-font {
    font-family: 'Cinzel', serif;
    letter-spacing: 0.25em;
    text-transform: uppercase;
  }

  /* === HERO === */
  .hero {
    position: relative;
    min-height: 100vh;
    background:
      radial-gradient(ellipse at top right, rgba(201, 169, 97, 0.15) 0%, transparent 50%),
      radial-gradient(ellipse at bottom left, rgba(26, 58, 92, 0.4) 0%, transparent 50%),
      linear-gradient(135deg, var(--navy-deep) 0%, var(--navy) 60%, var(--navy-light) 100%);
    color: var(--cream);
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
    padding: 80px 24px;
  }

  .hero::before {
    content: '';
    position: absolute;
    inset: 0;
    background-image:
      linear-gradient(rgba(201, 169, 97, 0.04) 1px, transparent 1px),
      linear-gradient(90deg, rgba(201, 169, 97, 0.04) 1px, transparent 1px);
    background-size: 80px 80px;
    pointer-events: none;
  }

  .hero::after {
    content: '';
    position: absolute;
    inset: 0;
    background:
      radial-gradient(circle at 20% 30%, rgba(201, 169, 97, 0.08) 0%, transparent 30%),
      radial-gradient(circle at 80% 70%, rgba(201, 169, 97, 0.05) 0%, transparent 30%);
    pointer-events: none;
  }

  .moon-emblem {
    position: absolute;
    top: 50%;
    right: -200px;
    width: 600px;
    height: 600px;
    transform: translateY(-50%);
    opacity: 0.07;
    pointer-events: none;
  }

  .moon-emblem svg {
    width: 100%;
    height: 100%;
  }

  .hero-content {
    position: relative;
    max-width: 900px;
    text-align: center;
    z-index: 2;
    animation: fadeUp 1.4s cubic-bezier(0.16, 1, 0.3, 1);
  }

  @keyframes fadeUp {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  .hero-eyebrow {
    color: var(--gold);
    font-size: 0.75rem;
    margin-bottom: 32px;
    display: inline-flex;
    align-items: center;
    gap: 16px;
  }

  .hero-eyebrow::before,
  .hero-eyebrow::after {
    content: '';
    width: 40px;
    height: 1px;
    background: var(--gold);
  }

  .hero h1 {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 300;
    font-size: clamp(2.5rem, 6vw, 4.5rem);
    line-height: 1.1;
    margin-bottom: 24px;
    color: var(--cream);
  }

  .hero h1 em {
    font-style: italic;
    color: var(--gold-light);
    font-weight: 400;
  }

  .hero-jp {
    font-family: 'Noto Serif JP', serif;
    font-size: clamp(1rem, 2vw, 1.25rem);
    font-weight: 300;
    color: var(--cream);
    opacity: 0.85;
    margin-bottom: 48px;
    letter-spacing: 0.15em;
  }

  .hero-divider {
    width: 1px;
    height: 60px;
    background: linear-gradient(to bottom, transparent, var(--gold), transparent);
    margin: 0 auto 48px;
  }

  .hero-tagline {
    font-family: 'Noto Serif JP', serif;
    font-size: clamp(0.95rem, 1.5vw, 1.05rem);
    line-height: 2.2;
    color: var(--cream);
    opacity: 0.9;
    max-width: 640px;
    margin: 0 auto 56px;
    font-weight: 300;
  }

  .cta-group {
    display: flex;
    gap: 20px;
    justify-content: center;
    flex-wrap: wrap;
  }

  .btn {
    display: inline-flex;
    align-items: center;
    gap: 12px;
    padding: 18px 36px;
    font-family: 'Cinzel', serif;
    font-size: 0.75rem;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    text-decoration: none;
    transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
    cursor: pointer;
    border: none;
  }

  .btn-primary {
    background: var(--gold);
    color: var(--navy-deep);
    border: 1px solid var(--gold);
  }

  .btn-primary:hover {
    background: var(--gold-light);
    border-color: var(--gold-light);
    transform: translateY(-2px);
    box-shadow: 0 12px 30px rgba(201, 169, 97, 0.3);
  }

  .btn-outline {
    background: transparent;
    color: var(--cream);
    border: 1px solid rgba(245, 241, 232, 0.3);
  }

  .btn-outline:hover {
    border-color: var(--gold);
    color: var(--gold);
    transform: translateY(-2px);
  }

  /* === SECTION COMMON === */
  section {
    padding: 120px 24px;
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
  }

  .section-header {
    text-align: center;
    margin-bottom: 80px;
  }

  .section-eyebrow {
    color: var(--gold-dark);
    font-family: 'Cinzel', serif;
    font-size: 0.7rem;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    margin-bottom: 24px;
    display: inline-flex;
    align-items: center;
    gap: 16px;
  }

  .section-eyebrow::before,
  .section-eyebrow::after {
    content: '';
    width: 30px;
    height: 1px;
    background: var(--gold-dark);
  }

  .section-title {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 300;
    font-size: clamp(2rem, 4vw, 3rem);
    color: var(--navy-deep);
    line-height: 1.2;
    margin-bottom: 16px;
  }

  .section-title em {
    font-style: italic;
    color: var(--gold-dark);
  }

  .section-subtitle {
    font-size: 0.95rem;
    color: var(--ink-soft);
    font-weight: 300;
    letter-spacing: 0.1em;
  }

  /* === PHILOSOPHY === */
  .philosophy {
    background: var(--cream-soft);
    position: relative;
  }

  .philosophy-content {
    max-width: 760px;
    margin: 0 auto;
    text-align: center;
  }

  .philosophy-quote {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: clamp(1.5rem, 3vw, 2.2rem);
    font-weight: 300;
    line-height: 1.5;
    color: var(--navy-deep);
    margin-bottom: 48px;
    position: relative;
  }

  .philosophy-quote::before {
    content: '"';
    position: absolute;
    top: -40px;
    left: -40px;
    font-size: 8rem;
    color: var(--gold);
    opacity: 0.2;
    font-family: 'Cormorant Garamond', serif;
    line-height: 1;
  }

  .philosophy-text {
    font-size: 1rem;
    line-height: 2.2;
    color: var(--ink-soft);
    font-weight: 300;
  }

  .philosophy-text p + p {
    margin-top: 24px;
  }

  /* === SERVICES === */
  .services {
    background: var(--navy-deep);
    color: var(--cream);
    position: relative;
    overflow: hidden;
  }

  .services::before {
    content: '';
    position: absolute;
    inset: 0;
    background-image:
      linear-gradient(rgba(201, 169, 97, 0.03) 1px, transparent 1px),
      linear-gradient(90deg, rgba(201, 169, 97, 0.03) 1px, transparent 1px);
    background-size: 100px 100px;
    pointer-events: none;
  }

  .services .section-title {
    color: var(--cream);
  }

  .services .section-eyebrow {
    color: var(--gold);
  }

  .services .section-eyebrow::before,
  .services .section-eyebrow::after {
    background: var(--gold);
  }

  .services .section-subtitle {
    color: var(--cream);
    opacity: 0.7;
  }

  .services-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1px;
    background: rgba(201, 169, 97, 0.2);
    border: 1px solid rgba(201, 169, 97, 0.2);
    position: relative;
    z-index: 1;
  }

  .service-card {
    background: var(--navy-deep);
    padding: 56px 36px;
    transition: all 0.6s cubic-bezier(0.16, 1, 0.3, 1);
    position: relative;
    overflow: hidden;
  }

  .service-card::before {
    content: '';
    position: absolute;
    inset: 0;
    background: linear-gradient(135deg, rgba(201, 169, 97, 0.05) 0%, transparent 50%);
    opacity: 0;
    transition: opacity 0.6s;
  }

  .service-card:hover::before {
    opacity: 1;
  }

  .service-card:hover {
    background: var(--navy);
  }

  .service-number {
    font-family: 'Cinzel', serif;
    color: var(--gold);
    font-size: 0.7rem;
    letter-spacing: 0.3em;
    margin-bottom: 24px;
    display: block;
  }

  .service-icon {
    width: 56px;
    height: 56px;
    margin-bottom: 32px;
    color: var(--gold);
  }

  .service-icon svg {
    width: 100%;
    height: 100%;
    stroke: var(--gold);
    fill: none;
    stroke-width: 0.8;
  }

  .service-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.5rem;
    font-weight: 400;
    color: var(--cream);
    margin-bottom: 8px;
  }

  .service-jp {
    font-size: 0.85rem;
    color: var(--gold);
    margin-bottom: 24px;
    letter-spacing: 0.15em;
    font-weight: 300;
  }

  .service-description {
    font-size: 0.9rem;
    line-height: 2;
    color: var(--cream);
    opacity: 0.75;
    font-weight: 300;
  }

  .service-note {
    font-size: 0.7rem;
    color: var(--gold);
    opacity: 0.7;
    margin-top: 16px;
    letter-spacing: 0.05em;
    font-weight: 300;
    line-height: 1.6;
  }

  /* === MEMBERSHIP === */
  .membership {
    background: var(--cream-soft);
    position: relative;
  }

  .membership-card {
    max-width: 720px;
    margin: 0 auto;
    background: var(--pearl);
    padding: 80px 60px;
    border: 1px solid rgba(201, 169, 97, 0.3);
    position: relative;
    text-align: center;
  }

  .membership-card::before,
  .membership-card::after {
    content: '';
    position: absolute;
    width: 40px;
    height: 40px;
    border: 1px solid var(--gold);
  }

  .membership-card::before {
    top: 16px;
    left: 16px;
    border-right: none;
    border-bottom: none;
  }

  .membership-card::after {
    bottom: 16px;
    right: 16px;
    border-left: none;
    border-top: none;
  }

  .membership-tier {
    font-family: 'Cinzel', serif;
    font-size: 0.75rem;
    letter-spacing: 0.4em;
    color: var(--gold-dark);
    margin-bottom: 16px;
  }

  .membership-name {
    font-family: 'Cormorant Garamond', serif;
    font-size: 2.5rem;
    font-weight: 300;
    color: var(--navy-deep);
    margin-bottom: 8px;
  }

  .membership-name em {
    font-style: italic;
    color: var(--gold-dark);
  }

  .membership-jp {
    font-size: 0.9rem;
    color: var(--ink-soft);
    margin-bottom: 40px;
    letter-spacing: 0.2em;
    font-weight: 300;
  }

  .membership-divider {
    width: 60px;
    height: 1px;
    background: var(--gold);
    margin: 0 auto 40px;
  }

  .benefits-list {
    list-style: none;
    text-align: left;
    max-width: 480px;
    margin: 0 auto 48px;
  }

  .benefits-list li {
    padding: 16px 0 16px 36px;
    border-bottom: 1px solid rgba(201, 169, 97, 0.2);
    position: relative;
    font-size: 0.95rem;
    color: var(--ink-soft);
    font-weight: 300;
    line-height: 1.7;
  }

  .benefits-list li::before {
    content: '';
    position: absolute;
    left: 0;
    top: 28px;
    width: 20px;
    height: 1px;
    background: var(--gold);
  }

  .benefits-list li:last-child {
    border-bottom: none;
  }

  .benefits-list strong {
    font-weight: 500;
    color: var(--navy-deep);
  }

  .membership-note {
    font-size: 0.8rem;
    color: var(--ink-soft);
    font-style: italic;
    opacity: 0.7;
    line-height: 1.8;
  }

  /* === DOCTOR === */
  .doctor {
    background: var(--navy-deep);
    color: var(--cream);
    position: relative;
    overflow: hidden;
  }

  .doctor::before {
    content: '';
    position: absolute;
    inset: 0;
    background:
      radial-gradient(circle at 70% 30%, rgba(201, 169, 97, 0.08) 0%, transparent 40%);
    pointer-events: none;
  }

  .doctor .section-title {
    color: var(--cream);
  }

  .doctor .section-eyebrow {
    color: var(--gold);
  }

  .doctor .section-eyebrow::before,
  .doctor .section-eyebrow::after {
    background: var(--gold);
  }

  .doctor-content {
    max-width: 800px;
    margin: 0 auto;
    text-align: center;
    position: relative;
    z-index: 1;
  }

  .doctor-credentials {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 32px;
    margin: 56px 0;
    padding: 48px 0;
    border-top: 1px solid rgba(201, 169, 97, 0.2);
    border-bottom: 1px solid rgba(201, 169, 97, 0.2);
  }

  .credential {
    text-align: center;
  }

  .credential-label {
    font-family: 'Cinzel', serif;
    font-size: 0.65rem;
    letter-spacing: 0.3em;
    color: var(--gold);
    margin-bottom: 12px;
  }

  .credential-value {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.1rem;
    color: var(--cream);
    font-weight: 400;
    line-height: 1.5;
  }

  .doctor-bio {
    font-size: 0.95rem;
    line-height: 2.2;
    color: var(--cream);
    opacity: 0.85;
    font-weight: 300;
    text-align: left;
    max-width: 700px;
    margin: 0 auto;
  }

  .doctor-bio p + p {
    margin-top: 20px;
  }

  /* === CONTACT === */
  .contact {
    background: var(--cream-soft);
    text-align: center;
  }

  .contact-content {
    max-width: 640px;
    margin: 0 auto;
  }

  .contact-text {
    font-size: 1rem;
    line-height: 2.2;
    color: var(--ink-soft);
    margin-bottom: 48px;
    font-weight: 300;
  }

  .contact-info {
    background: var(--pearl);
    border: 1px solid rgba(201, 169, 97, 0.3);
    padding: 48px;
    margin-bottom: 32px;
  }

  .contact-label {
    font-family: 'Cinzel', serif;
    font-size: 0.7rem;
    letter-spacing: 0.3em;
    color: var(--gold-dark);
    margin-bottom: 16px;
  }

  .contact-value {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.4rem;
    color: var(--navy-deep);
    margin-bottom: 8px;
    font-weight: 400;
  }

  .contact-jp {
    font-size: 0.9rem;
    color: var(--ink-soft);
    line-height: 1.8;
  }

  .privacy-note {
    font-size: 0.8rem;
    color: var(--ink-soft);
    opacity: 0.7;
    font-style: italic;
    line-height: 1.8;
  }

  /* === FOOTER === */
  footer {
    background: var(--navy-deep);
    color: var(--cream);
    padding: 64px 24px 32px;
    text-align: center;
    border-top: 1px solid rgba(201, 169, 97, 0.2);
  }

  .footer-mark {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.8rem;
    font-weight: 300;
    margin-bottom: 8px;
    letter-spacing: 0.05em;
  }

  .footer-mark em {
    color: var(--gold);
    font-style: italic;
  }

  .footer-tagline {
    font-family: 'Cinzel', serif;
    font-size: 0.7rem;
    letter-spacing: 0.4em;
    color: var(--gold);
    margin-bottom: 32px;
  }

  .footer-divider {
    width: 40px;
    height: 1px;
    background: var(--gold);
    margin: 0 auto 24px;
    opacity: 0.5;
  }

  .footer-text {
    font-size: 0.75rem;
    color: var(--cream);
    opacity: 0.5;
    line-height: 1.8;
  }

  /* === RESPONSIVE === */
  @media (max-width: 768px) {
    section {
      padding: 80px 20px;
    }

    .moon-emblem {
      width: 400px;
      height: 400px;
      right: -150px;
      opacity: 0.05;
    }

    .membership-card {
      padding: 56px 32px;
    }

    .doctor-credentials {
      gap: 24px;
      padding: 32px 0;
    }

    .philosophy-quote::before {
      left: -10px;
      top: -30px;
      font-size: 5rem;
    }

    .contact-info {
      padding: 36px 24px;
    }
  }
</style>
</head>
<body>

<!-- HERO SECTION -->
<section class="hero">
  <div class="moon-emblem">
    <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <radialGradient id="moonGrad" cx="40%" cy="40%">
          <stop offset="0%" stop-color="#e6cc8a"/>
          <stop offset="100%" stop-color="#9c7f3e"/>
        </radialGradient>
      </defs>
      <circle cx="100" cy="100" r="80" fill="url(#moonGrad)"/>
      <circle cx="100" cy="100" r="80" fill="none" stroke="#c9a961" stroke-width="0.5"/>
      <circle cx="100" cy="100" r="95" fill="none" stroke="#c9a961" stroke-width="0.3"/>
    </svg>
  </div>

  <div class="hero-content">
    <div class="hero-eyebrow accent-font">Moon Partners</div>
    <h1>Your Personal <em>Doctor</em>,<br>Always at Your Side.</h1>
    <p class="hero-jp">経営者のための、もうひとりの主治医</p>

    <div class="hero-divider"></div>

    <p class="hero-tagline">
      多忙を極めるエグゼクティブのために。<br>
      24時間、いつでも、どこでも。<br>
      あなたの健康を、最も深く理解する医師が寄り添います。
    </p>

    <div class="cta-group">
      <a href="#contact" class="btn btn-primary">Inquire Privately</a>
      <a href="#services" class="btn btn-outline">View Services</a>
    </div>
  </div>
</section>

<!-- PHILOSOPHY -->
<section class="philosophy">
  <div class="container">
    <div class="section-header">
      <div class="section-eyebrow">Our Philosophy</div>
      <h2 class="section-title">健康は、最大の<em>資産</em>である</h2>
      <p class="section-subtitle">— Health is the ultimate capital —</p>
    </div>

    <div class="philosophy-content">
      <p class="philosophy-quote">
        経営判断と同じ精度で、<br>
        あなたの体と向き合う。
      </p>

      <div class="philosophy-text">
        <p>
          時間は、最も希少な資源です。会議、出張、決断の連続のなかで、自身の健康を後回しにしてはいないでしょうか。
        </p>
        <p>
          Moon Partners は、限られた会員様だけにご提供する完全紹介制のパーソナルドクターサービスです。専属医がお客様一人ひとりの健康状態を深く把握し、予防から早期発見、治療判断のセカンドオピニオンまで、生涯にわたる伴走者として機能します。
        </p>
        <p>
          病気になってから医師を探すのではなく、いつでも信頼できる医師がそばにいる安心を。それが、エグゼクティブにふさわしい医療のかたちです。
        </p>
      </div>
    </div>
  </div>
</section>

<!-- SERVICES -->
<section class="services" id="services">
  <div class="container">
    <div class="section-header">
      <div class="section-eyebrow">Concierge Services</div>
      <h2 class="section-title">Bespoke <em>Medical Care</em></h2>
      <p class="section-subtitle">— あなただけの、医療コンシェルジュ —</p>
    </div>

    <div class="services-grid">
      <div class="service-card">
        <span class="service-number">No. 01</span>
        <div class="service-icon">
          <svg viewBox="0 0 48 48"><circle cx="24" cy="24" r="20"/><path d="M24 14v10l7 4"/></svg>
        </div>
        <h3 class="service-title">24/7 Direct Access</h3>
        <p class="service-jp">24時間365日 LINE相談</p>
        <p class="service-description">
          休日も深夜も、専属医に直接ご相談いただけます。海外出張中でも、LINE一本でつながる安心。
        </p>
      </div>

      <div class="service-card">
        <span class="service-number">No. 02</span>
        <div class="service-icon">
          <svg viewBox="0 0 48 48"><path d="M24 6L8 14v10c0 10 7 16 16 18 9-2 16-8 16-18V14L24 6z"/></svg>
        </div>
        <h3 class="service-title">Second Opinion</h3>
        <p class="service-jp">セカンドオピニオン</p>
        <p class="service-description">
          重要な医療判断の場面で。ご家族の医療相談を含め、客観的な専門家の見解を提供します。
        </p>
      </div>

      <div class="service-card">
        <span class="service-number">No. 03</span>
        <div class="service-icon">
          <svg viewBox="0 0 48 48"><circle cx="24" cy="18" r="6"/><path d="M12 40c0-7 5-12 12-12s12 5 12 12"/></svg>
        </div>
        <h3 class="service-title">Family Care</h3>
        <p class="service-jp">ご家族のケア</p>
        <p class="service-description">
          会員様ご本人だけでなく、ご家族の健康相談にも対応。一族の主治医として機能します。
        </p>
      </div>

      <div class="service-card">
        <span class="service-number">No. 04</span>
        <div class="service-icon">
          <svg viewBox="0 0 48 48"><path d="M24 8v32M16 16l8-8 8 8M14 32c0 4 4 8 10 8s10-4 10-8"/></svg>
        </div>
        <h3 class="service-title">IV Therapy</h3>
        <p class="service-jp">疲労回復・美容点滴</p>
        <p class="service-description">
          重要な会議や出張前のコンディショニングに。提携クリニックを通じて、適応をご相談のうえご案内いたします。
        </p>
        <p class="service-note">※提携クリニックでの診療となります</p>
      </div>

      <div class="service-card">
        <span class="service-number">No. 05</span>
        <div class="service-icon">
          <svg viewBox="0 0 48 48"><rect x="14" y="10" width="20" height="32" rx="2"/><path d="M20 18h8M20 24h8M20 30h8"/></svg>
        </div>
        <h3 class="service-title">Online Prescription</h3>
        <p class="service-jp">オンライン処方</p>
        <p class="service-description">
          提携クリニックのオンライン診療体制を通じて、適切な処方をご案内いたします。診察の上、医師の判断にて対応いたします。
        </p>
        <p class="service-note">※提携クリニックでの診療となります</p>
      </div>

      <div class="service-card">
        <span class="service-number">No. 06</span>
        <div class="service-icon">
          <svg viewBox="0 0 48 48"><path d="M8 24h8l4-12 8 24 4-12h8"/></svg>
        </div>
        <h3 class="service-title">Health Navigation</h3>
        <p class="service-jp">健診結果のご相談・医療機関ご案内</p>
        <p class="service-description">
          人間ドックや健康診断の結果について、専属医がわかりやすく解説。必要に応じて適切な医療機関をご案内します。
        </p>
      </div>
    </div>
  </div>
</section>

<!-- MEMBERSHIP -->
<section class="membership">
  <div class="container">
    <div class="section-header">
      <div class="section-eyebrow">Membership</div>
      <h2 class="section-title">Closed <em>Membership</em></h2>
      <p class="section-subtitle">— 完全紹介制 —</p>
    </div>

    <div class="membership-card">
      <div class="membership-tier">Annual Membership</div>
      <h3 class="membership-name">Moon <em>Partners</em></h3>
      <p class="membership-jp">プレミアム会員制度</p>

      <div class="membership-divider"></div>

      <ul class="benefits-list">
        <li><strong>専属医による24時間サポート</strong>　— 主治医が直接、あなたの健康を見守ります</li>
        <li><strong>無制限のオンライン相談</strong>　— LINEを通じた医療相談はいつでも、何度でも</li>
        <li><strong>健診結果のパーソナル解説</strong>　— 人間ドック結果を専属医が詳細にレビュー</li>
        <li><strong>セカンドオピニオン</strong>　— 重要な医療判断の場面で客観的な見解を提供</li>
        <li><strong>提携クリニックとの連携</strong>　— オンライン処方・点滴療法等は提携先にてご案内</li>
        <li><strong>ご家族枠の付帯</strong>　— 配偶者・お子様も含めたファミリーケア</li>
        <li><strong>優先的な医療機関紹介</strong>　— 必要に応じ、専門医へスムーズにご案内</li>
      </ul>

      <p class="membership-note">
        ※ 当サービスは完全紹介制です。<br>
        会員数を限定しており、サービス品質の維持に努めております。<br>
        詳細につきましては、個別にご案内させていただきます。
      </p>
    </div>
  </div>
</section>

<!-- DOCTOR -->
<section class="doctor">
  <div class="container">
    <div class="section-header">
      <div class="section-eyebrow">Your Physician</div>
      <h2 class="section-title">Meet Your <em>Doctor</em></h2>
      <p class="section-subtitle">— 担当医のご紹介 —</p>
    </div>

    <div class="doctor-content">
      <div class="doctor-credentials">
        <div class="credential">
          <div class="credential-label">Speciality</div>
          <div class="credential-value">循環器内科<br>専門医</div>
        </div>
        <div class="credential">
          <div class="credential-label">Affiliation</div>
          <div class="credential-value">大学病院<br>勤務医</div>
        </div>
        <div class="credential">
          <div class="credential-label">Region</div>
          <div class="credential-value">岩手・青森<br>連携医療体制</div>
        </div>
      </div>

      <div class="doctor-bio">
        <p>
          大学病院で循環器内科の専門医として臨床・研究に従事するかたわら、青森県内のクリニックと連携し、地域医療の最前線に立っております。
        </p>
        <p>
          循環器疾患は、サイレントに進行し、ある日突然、人生を変える事態を引き起こします。だからこそ、日常的に信頼できる医師との関係を持つことが、エグゼクティブにとっての真のリスクマネジメントになると考えています。
        </p>
        <p>
          Moon Partners では、最新のエビデンスに基づく医療と、お客様一人ひとりのライフスタイル・価値観を深く理解した上での、真にパーソナルなケアをお届けします。
        </p>
      </div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section class="contact" id="contact">
  <div class="container">
    <div class="section-header">
      <div class="section-eyebrow">Private Inquiry</div>
      <h2 class="section-title">Begin Your <em>Journey</em></h2>
      <p class="section-subtitle">— ご相談・お問い合わせ —</p>
    </div>

    <div class="contact-content">
      <p class="contact-text">
        Moon Partners は完全紹介制のサービスです。<br>
        ご興味をお持ちの方は、以下よりお気軽にお問い合わせください。<br>
        担当者より、個別にご案内させていただきます。
      </p>

      <div class="contact-info">
        <div class="contact-label">Contact</div>
        <div class="contact-value">Private Consultation</div>
        <p class="contact-jp">
          お問い合わせフォームまたは<br>
          ご紹介者様経由にてご連絡ください
        </p>
      </div>

      <p class="privacy-note">
        — お預かりした個人情報は厳重に管理し、<br>
        会員様のプライバシー保護を最優先いたします —
      </p>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-mark">Moon <em>Partners</em></div>
  <div class="footer-tagline">Executive Personal Doctor</div>
  <div class="footer-divider"></div>
  <p class="footer-text">
    © Moon Partners. All Rights Reserved.<br>
    Private Healthcare Concierge for Executives
  </p>
</footer>

</body>
</html>
