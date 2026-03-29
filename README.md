# Mes-codes-de-parrainage
Bonjour je vous partage mes codes de parrainage tous les codes sont valables et vérifier
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Codes Parrainage – Manon</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet"/>
  <style>
    :root {
      --gold: #c9a84c;
      --gold-light: #e8c97a;
      --dark: #0d0d0d;
      --dark2: #141414;
      --dark3: #1c1c1c;
      --text: #e8e2d9;
      --muted: #7a7570;
      --accent: #c9a84c;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--dark);
      color: var(--text);
      font-family: 'DM Sans', sans-serif;
      min-height: 100vh;
      overflow-x: hidden;
    }

    /* GRAIN OVERLAY */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.04'/%3E%3C/svg%3E");
      pointer-events: none;
      z-index: 999;
      opacity: 0.35;
    }

    /* HERO */
    header {
      position: relative;
      text-align: center;
      padding: 80px 24px 60px;
      overflow: hidden;
    }

    header::before {
      content: '';
      position: absolute;
      top: -120px; left: 50%;
      transform: translateX(-50%);
      width: 600px; height: 400px;
      background: radial-gradient(ellipse, rgba(201,168,76,0.18) 0%, transparent 70%);
      pointer-events: none;
    }

    .hero-tag {
      display: inline-block;
      font-size: 11px;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--gold);
      border: 1px solid rgba(201,168,76,0.35);
      padding: 5px 16px;
      border-radius: 20px;
      margin-bottom: 28px;
      animation: fadeUp 0.6s ease both;
    }

    h1 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(42px, 7vw, 80px);
      line-height: 1.05;
      font-weight: 700;
      color: var(--text);
      animation: fadeUp 0.7s 0.1s ease both;
    }

    h1 em {
      font-style: italic;
      color: var(--gold);
    }

    .hero-sub {
      margin-top: 18px;
      font-size: 16px;
      color: var(--muted);
      font-weight: 300;
      max-width: 480px;
      margin-left: auto;
      margin-right: auto;
      line-height: 1.7;
      animation: fadeUp 0.7s 0.2s ease both;
    }

    .insta-link {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      margin-top: 28px;
      padding: 11px 24px;
      background: linear-gradient(135deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888);
      border-radius: 30px;
      color: white;
      text-decoration: none;
      font-size: 14px;
      font-weight: 500;
      letter-spacing: 0.03em;
      transition: transform 0.2s, box-shadow 0.2s;
      animation: fadeUp 0.7s 0.3s ease both;
    }

    .insta-link:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 30px rgba(220,39,67,0.35);
    }

    .insta-link svg { width: 18px; height: 18px; }

    /* DIVIDER */
    .divider {
      width: 80px; height: 1px;
      background: linear-gradient(90deg, transparent, var(--gold), transparent);
      margin: 0 auto 60px;
    }

    /* FILTER TABS */
    .filter-bar {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 8px;
      padding: 0 24px 44px;
    }

    .filter-btn {
      padding: 7px 18px;
      border-radius: 20px;
      border: 1px solid rgba(201,168,76,0.2);
      background: transparent;
      color: var(--muted);
      font-family: 'DM Sans', sans-serif;
      font-size: 13px;
      cursor: pointer;
      transition: all 0.2s;
    }

    .filter-btn:hover, .filter-btn.active {
      background: rgba(201,168,76,0.12);
      border-color: var(--gold);
      color: var(--gold);
    }

    /* GRID */
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 20px;
      padding: 0 24px 80px;
      max-width: 1200px;
      margin: 0 auto;
    }

    /* CARD */
    .card {
      background: var(--dark2);
      border: 1px solid rgba(255,255,255,0.06);
      border-radius: 16px;
      padding: 28px;
      position: relative;
      overflow: hidden;
      transition: transform 0.25s, border-color 0.25s, box-shadow 0.25s;
      animation: fadeUp 0.5s ease both;
    }

    .card::before {
      content: '';
      position: absolute;
      inset: 0;
      background: linear-gradient(135deg, rgba(201,168,76,0.04) 0%, transparent 60%);
      pointer-events: none;
    }

    .card:hover {
      transform: translateY(-4px);
      border-color: rgba(201,168,76,0.3);
      box-shadow: 0 12px 40px rgba(0,0,0,0.4), 0 0 0 1px rgba(201,168,76,0.1);
    }

    .card-header {
      display: flex;
      align-items: flex-start;
      gap: 14px;
      margin-bottom: 18px;
    }

    .card-icon {
      width: 46px; height: 46px;
      border-radius: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 22px;
      flex-shrink: 0;
    }

    .card-title {
      font-family: 'Playfair Display', serif;
      font-size: 20px;
      font-weight: 700;
      line-height: 1.2;
    }

    .card-category {
      font-size: 11px;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--muted);
      margin-top: 3px;
    }

    .card-desc {
      font-size: 14px;
      color: var(--muted);
      line-height: 1.65;
      margin-bottom: 20px;
      font-weight: 300;
    }

    .reward-badge {
      display: inline-block;
      background: linear-gradient(135deg, rgba(201,168,76,0.15), rgba(201,168,76,0.08));
      border: 1px solid rgba(201,168,76,0.3);
      color: var(--gold-light);
      font-size: 13px;
      font-weight: 500;
      padding: 5px 12px;
      border-radius: 8px;
      margin-bottom: 18px;
    }

    .code-block {
      background: var(--dark3);
      border: 1px solid rgba(255,255,255,0.07);
      border-radius: 10px;
      padding: 12px 16px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 10px;
      margin-bottom: 14px;
    }

    .code-text {
      font-family: 'Courier New', monospace;
      font-size: 15px;
      font-weight: 600;
      color: var(--gold-light);
      letter-spacing: 0.05em;
      word-break: break-all;
    }

    .copy-btn {
      background: rgba(201,168,76,0.12);
      border: 1px solid rgba(201,168,76,0.25);
      color: var(--gold);
      padding: 6px 14px;
      border-radius: 7px;
      font-size: 12px;
      font-family: 'DM Sans', sans-serif;
      font-weight: 500;
      cursor: pointer;
      transition: all 0.2s;
      white-space: nowrap;
      flex-shrink: 0;
    }

    .copy-btn:hover {
      background: rgba(201,168,76,0.22);
      border-color: var(--gold);
    }

    .copy-btn.copied {
      background: rgba(100,200,100,0.15);
      border-color: rgba(100,200,100,0.4);
      color: #7dd87d;
    }

    .cta-btn {
      display: block;
      text-align: center;
      width: 100%;
      padding: 12px;
      border-radius: 10px;
      background: linear-gradient(135deg, rgba(201,168,76,0.18), rgba(201,168,76,0.08));
      border: 1px solid rgba(201,168,76,0.3);
      color: var(--gold-light);
      text-decoration: none;
      font-size: 14px;
      font-weight: 500;
      transition: all 0.2s;
      letter-spacing: 0.02em;
    }

    .cta-btn:hover {
      background: linear-gradient(135deg, rgba(201,168,76,0.28), rgba(201,168,76,0.14));
      border-color: var(--gold);
      color: var(--gold);
    }

    /* CATEGORY COLORS */
    .cat-finance { background: rgba(59, 130, 246, 0.15); }
    .cat-invest  { background: rgba(16, 185, 129, 0.15); }
    .cat-crypto  { background: rgba(245, 158, 11, 0.15); }
    .cat-shopping{ background: rgba(236, 72, 153, 0.15); }
    .cat-delivery{ background: rgba(139, 92, 246, 0.15); }

    /* FOOTER */
    footer {
      text-align: center;
      padding: 40px 24px;
      border-top: 1px solid rgba(255,255,255,0.05);
      color: var(--muted);
      font-size: 13px;
    }

    footer a { color: var(--gold); text-decoration: none; }
    footer a:hover { text-decoration: underline; }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(18px); }
      to   { opacity: 1; transform: translateY(0); }
    }

    /* HIDDEN cards for filter */
    .card.hidden { display: none; }

    /* Toast */
    #toast {
      position: fixed;
      bottom: 30px; left: 50%;
      transform: translateX(-50%) translateY(60px);
      background: var(--dark3);
      border: 1px solid var(--gold);
      color: var(--gold-light);
      padding: 10px 22px;
      border-radius: 30px;
      font-size: 14px;
      font-weight: 500;
      z-index: 1000;
      transition: transform 0.3s;
      pointer-events: none;
    }
    #toast.show { transform: translateX(-50%) translateY(0); }

    @media (max-width: 480px) {
      .grid { grid-template-columns: 1fr; padding: 0 16px 60px; }
      header { padding: 60px 16px 40px; }
    }
  </style>
</head>
<body>

<header>
  <div class="hero-tag">✦ Offres exclusives</div>
  <h1>Mes codes de<br><em>parrainage</em></h1>
  <p class="hero-sub">Utilisez mes codes pour profiter de bonus à l'inscription — on gagne tous les deux !</p>
  <a class="insta-link" href="https://instagram.com/manon_8897" target="_blank">
    <svg viewBox="0 0 24 24" fill="white"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zM12 0C8.741 0 8.333.014 7.053.072 2.695.272.273 2.69.073 7.052.014 8.333 0 8.741 0 12c0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98C8.333 23.986 8.741 24 12 24c3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98C15.668.014 15.259 0 12 0zm0 5.838a6.162 6.162 0 100 12.324 6.162 6.162 0 000-12.324zM12 16a4 4 0 110-8 4 4 0 010 8zm6.406-11.845a1.44 1.44 0 100 2.881 1.44 1.44 0 000-2.881z"/></svg>
    @manon_8897
  </a>
</header>

<div class="divider"></div>

<div class="filter-bar">
  <button class="filter-btn active" onclick="filterCards('all', this)">Tout</button>
  <button class="filter-btn" onclick="filterCards('finance', this)">🏦 Banque</button>
  <button class="filter-btn" onclick="filterCards('invest', this)">📈 Investissement</button>
  <button class="filter-btn" onclick="filterCards('crypto', this)">🪙 Crypto</button>
  <button class="filter-btn" onclick="filterCards('shopping', this)">🛍️ Shopping</button>
  <button class="filter-btn" onclick="filterCards('delivery', this)">🚴 Livraison</button>
</div>

<div class="grid" id="grid">

  <!-- TRADING 212 -->
  <div class="card" data-cat="invest" style="animation-delay:0.05s">
    <div class="card-header">
      <div class="card-icon cat-invest">📊</div>
      <div>
        <div class="card-title">Trading 212</div>
        <div class="card-category">Investissement</div>
      </div>
    </div>
    <div class="reward-badge">🎁 1 action gratuite</div>
    <p class="card-desc">Investissez en bourse simplement. Recevez une action offerte à l'inscription via mon lien.</p>
    <a class="cta-btn" href="https://www.trading212.com/invite/4Dqc581BZJQ" target="_blank">→ Obtenir mon action gratuite</a>
  </div>

  <!-- BOURSOBANK -->
  <div class="card" data-cat="finance" style="animation-delay:0.1s">
    <div class="card-header">
      <div class="card-icon cat-finance">🏦</div>
      <div>
        <div class="card-title">BoursoBank</div>
        <div class="card-category">Banque en ligne</div>
      </div>
    </div>
    <div class="reward-badge">💰 110€ offerts</div>
    <p class="card-desc">1ère ouverture de compte Ultim ou Welcome + mobilité bancaire EasyMove requise.</p>
    <div class="code-block">
      <span class="code-text">KETE9754</span>
      <button class="copy-btn" onclick="copyCode('KETE9754', this)">Copier</button>
    </div>
  </div>

  <!-- BOURSORAMA -->
  <div class="card" data-cat="finance" style="animation-delay:0.15s">
    <div class="card-header">
      <div class="card-icon cat-finance">🏛️</div>
      <div>
        <div class="card-title">Boursorama Banque</div>
        <div class="card-category">Banque en ligne</div>
      </div>
    </div>
    <div class="reward-badge">💰 Prime 150€</div>
    <p class="card-desc">Ouvrez un compte bancaire Boursorama et bénéficiez d'une prime de parrainage exceptionnelle.</p>
    <p class="card-desc" style="font-size:12px; margin-top:-10px;">Lien disponible en description Instagram ↓</p>
    <a class="cta-btn" href="https://instagram.com/manon_8897" target="_blank">→ Voir le lien sur Instagram</a>
  </div>

  <!-- LIVRET P -->
  <div class="card" data-cat="invest" style="animation-delay:0.2s">
    <div class="card-header">
      <div class="card-icon cat-invest">🏠</div>
      <div>
        <div class="card-title">Livret P.</div>
        <div class="card-category">Épargne immobilière</div>
      </div>
    </div>
    <div class="reward-badge">🎁 10€ au 1er dépôt</div>
    <p class="card-desc">Livret d'Épargne Pierre. Taux de base 4% + boosts. Minimum 100€ de dépôt pour activer le bonus.</p>
    <div class="code-block">
      <span class="code-text">D3C2A2</span>
      <button class="copy-btn" onclick="copyCode('D3C2A2', this)">Copier</button>
    </div>
  </div>

  <!-- CLUBFUNDING -->
  <div class="card" data-cat="invest" style="animation-delay:0.25s">
    <div class="card-header">
      <div class="card-icon cat-invest">🏢</div>
      <div>
        <div class="card-title">ClubFunding</div>
        <div class="card-category">Crowdfunding immobilier</div>
      </div>
    </div>
    <div class="reward-badge">💎 100€ offerts</div>
    <p class="card-desc">Investissez dans l'immobilier et dynamisez votre épargne grâce au crowdfunding immobilier.</p>
    <div class="code-block">
      <span class="code-text">UVORi27e</span>
      <button class="copy-btn" onclick="copyCode('UVORi27e', this)">Copier</button>
    </div>
  </div>

  <!-- LA PREMIERE BRIQUE -->
  <div class="card" data-cat="invest" style="animation-delay:0.3s">
    <div class="card-header">
      <div class="card-icon cat-invest">🧱</div>
      <div>
        <div class="card-title">La Première Brique</div>
        <div class="card-category">Crowdfunding immobilier</div>
      </div>
    </div>
    <div class="reward-badge">📈 Rendement moyen 10%</div>
    <p class="card-desc">Investissez dans le crowdfunding immobilier dès 1€. L'un des meilleurs rendements du marché.</p>
    <div class="code-block">
      <span class="code-text">HJR7N4</span>
      <button class="copy-btn" onclick="copyCode('HJR7N4', this)">Copier</button>
    </div>
  </div>

  <!-- BINANCE -->
  <div class="card" data-cat="crypto" style="animation-delay:0.35s">
    <div class="card-header">
      <div class="card-icon cat-crypto">₿</div>
      <div>
        <div class="card-title">Binance</div>
        <div class="card-category">Crypto-monnaies</div>
      </div>
    </div>
    <div class="reward-badge">🪙 10% sur vos frais</div>
    <p class="card-desc">Recevez 50% de ma commission, soit 10% offerts sur vos frais de trading à l'inscription.</p>
    <div class="code-block">
      <span class="code-text">432820882</span>
      <button class="copy-btn" onclick="copyCode('432820882', this)">Copier</button>
    </div>
    <a class="cta-btn" href="https://accounts.binance.com/fr/register?ref=432820882" target="_blank" style="margin-top:10px;">→ S'inscrire avec le lien</a>
  </div>

  <!-- BONDORA -->
  <div class="card" data-cat="invest" style="animation-delay:0.4s">
    <div class="card-header">
      <div class="card-icon cat-invest">💶</div>
      <div>
        <div class="card-title">Bondora</div>
        <div class="card-category">Prêts & investissement</div>
      </div>
    </div>
    <div class="reward-badge">🎁 5€ offerts</div>
    <p class="card-desc">Plateforme européenne de prêts entre particuliers. Bonus de 5€/£ à l'inscription via mon lien.</p>
    <a class="cta-btn" href="https://bondora.com/ref/kevint44" target="_blank">→ Rejoindre Bondora</a>
  </div>

  <!-- SHOPMIUM -->
  <div class="card" data-cat="shopping" style="animation-delay:0.45s">
    <div class="card-header">
      <div class="card-icon cat-shopping">🧾</div>
      <div>
        <div class="card-title">Shopmium</div>
        <div class="card-category">Cashback courses</div>
      </div>
    </div>
    <div class="reward-badge">🎁 3€ offerts</div>
    <p class="card-desc">Faites vos courses et récupérez du cashback sur vos achats quotidiens en supermarché.</p>
    <div class="code-block">
      <span class="code-text">z54pi9</span>
      <button class="copy-btn" onclick="copyCode('z54pi9', this)">Copier</button>
    </div>
  </div>

  <!-- ALIEXPRESS -->
  <div class="card" data-cat="shopping" style="animation-delay:0.5s">
    <div class="card-header">
      <div class="card-icon cat-shopping">🛒</div>
      <div>
        <div class="card-title">AliExpress</div>
        <div class="card-category">Shopping</div>
      </div>
    </div>
    <div class="reward-badge">💰 19€ offerts</div>
    <p class="card-desc">Profitez de 19€ / 19£ de réduction sur votre première commande via mon lien de parrainage.</p>
    <a class="cta-btn" href="https://a.aliexpress.com/_v6twAQ" target="_blank">→ Obtenir les 19€</a>
  </div>

  <!-- SHOPOPOP -->
  <div class="card" data-cat="delivery" style="animation-delay:0.55s">
    <div class="card-header">
      <div class="card-icon cat-delivery">🚴</div>
      <div>
        <div class="card-title">Shopopop</div>
        <div class="card-category">Livraison collaborative</div>
      </div>
    </div>
    <div class="reward-badge">🎁 5€ offerts</div>
    <p class="card-desc">Service de livraison collaborative. Gagnez 5€ à l'inscription avec mon code promotionnel.</p>
    <div class="code-block">
      <span class="code-text">KHXKG8</span>
      <button class="copy-btn" onclick="copyCode('KHXKG8', this)">Copier</button>
    </div>
  </div>

  <!-- YPER -->
  <div class="card" data-cat="delivery" style="animation-delay:0.6s">
    <div class="card-header">
      <div class="card-icon cat-delivery">📦</div>
      <div>
        <div class="card-title">Yper</div>
        <div class="card-category">Livraison</div>
      </div>
    </div>
    <div class="reward-badge">🎁 5€ à la 1ère livraison</div>
    <p class="card-desc">Inscrivez-vous sur Yper et gagnez 5 euros pour votre première livraison avec mon code.</p>
    <div class="code-block">
      <span class="code-text">KT-OMIUB</span>
      <button class="copy-btn" onclick="copyCode('KT-OMIUB', this)">Copier</button>
    </div>
  </div>

</div>

<footer>
  <p>Fait avec ♥ par <a href="https://instagram.com/manon_8897" target="_blank">@manon_8897</a></p>
  <p style="margin-top:8px; font-size:12px; color:#4a4540;">Ces liens sont des liens d'affiliation. En les utilisant, vous m'aidez et bénéficiez de bonus à l'inscription.</p>
</footer>

<div id="toast">✓ Code copié !</div>

<script>
  function copyCode(code, btn) {
    navigator.clipboard.writeText(code).then(() => {
      const original = btn.textContent;
      btn.textContent = '✓ Copié';
      btn.classList.add('copied');
      showToast();
      setTimeout(() => {
        btn.textContent = original;
        btn.classList.remove('copied');
      }, 2000);
    });
  }

  function showToast() {
    const toast = document.getElementById('toast');
    toast.classList.add('show');
    setTimeout(() => toast.classList.remove('show'), 2000);
  }

  function filterCards(cat, btn) {
    document.querySelectorAll('.filter-btn').forEach(b => b.classList.remove('active'));
    btn.classList.add('active');
    document.querySelectorAll('.card').forEach(card => {
      if (cat === 'all' || card.dataset.cat === cat) {
        card.classList.remove('hidden');
      } else {
        card.classList.add('hidden');
      }
    });
  }
</script>
</body>
</html>
