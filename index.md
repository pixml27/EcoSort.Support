---
layout: default
title: EcoSort — Support & Download
---

<div class="container">
  <header class="app-header" role="banner">
    <img src="/screenshots/logo.svg" alt="EcoSort logo" class="logo" />
  </header>

  <main role="main" aria-labelledby="hero-title">
    <!-- HERO -->
    <section class="hero" role="region" aria-label="EcoSort hero">
      <div class="left">
        <h1 id="hero-title" class="main-title">EcoSort</h1>
        <p class="subtitle">Support & download — make recycling effortless in Europe.</p>

        <div class="cta-buttons" role="group" aria-label="Primary calls to action">
          <a href="https://apps.apple.com/us/app/ecosort-barcelona/id6747254846"
             class="cta-button" aria-label="Download EcoSort on the App Store">📱 Download on the App Store</a>

          <a href="#web-lookup" class="cta-outline" aria-label="Try web lookup">🔍 Try web lookup</a>
        </div>
      </div>

      <div class="visual" aria-hidden="true">
        <img src="/screenshots/logo.svg" alt="" style="width:220px; height:auto;">
      </div>
    </section>

    <!-- HOW TO USE -->
    <section class="how-to-use" aria-labelledby="how-title">
      <h2 id="how-title">How to use EcoSort</h2>
      <div class="instructions" role="list">
        <p role="listitem">1. Select language & your city</p>
        <p role="listitem">2. Scan the packaging of your item</p>
        <p role="listitem">3. Get clear sorting instructions and eco-friendly tips</p>
      </div>

      <p class="description">
        EcoSort isn’t just another recycling app. We make it effortless to dispose of waste correctly—no more confusion about bins, colors, or local rules.
        With EcoSort you'll spend less time wondering "where does this go?" and more time helping the planet.
      </p>

      <p class="description">
        If you have feedback, feature requests, or questions — reach out anytime at <a href="mailto:akor@ecosort.app">akor@ecosort.app</a>.
      </p>

      <!-- Feature cards -->
      <div class="features" aria-hidden="false">
        <div class="feature">
          <h3 style="color:var(--brand)">Local rules</h3>
          <p>Get bin and schedule details for your neighbourhood and city district.</p>
        </div>
        <div class="feature">
          <h3 style="color:var(--accent)">Nearby drop-off points</h3>
          <p>Find glass, electronics and bulky waste locations on a map.</p>
        </div>
        <div class="feature">
          <h3 style="color:var(--cta)">Report an issue</h3>
          <p>See something wrong? Tell us and we’ll investigate and fix it.</p>
        </div>
      </div>
    </section>

    <!-- SCREENSHOTS -->
    <section class="screenshots-section" aria-label="App screenshots">
      <h2>App Screenshots</h2>
      <div class="screenshots-container">
        <img src="/screenshots/screen1.png" alt="EcoSort - Main screen" data-full="/screenshots/screen1.png" />
        <img src="/screenshots/screen2.png" alt="EcoSort - Scan result" data-full="/screenshots/screen2.png" />
        <img src="/screenshots/screen3.png" alt="EcoSort - Item details" data-full="/screenshots/screen3.png" />
        <img src="/screenshots/screen4.png" alt="EcoSort - Map / Locations" data-full="/screenshots/screen4.png" />
      </div>
    </section>

    <!-- WEB LOOKUP (simple modal anchor) -->
    <section id="web-lookup" style="margin-top:18px;">
      <h2>Quick web lookup</h2>
      <p class="description">Try a fast lookup from your browser — search by product name or barcode (coming soon: image lookup).</p>
      <div style="max-width:520px; margin: 12px 0;">
        <form action="/lookup" method="get" aria-label="Search product or barcode">
          <input name="q" type="search" placeholder="Search product or paste barcode" style="width:100%; padding:12px; border-radius:8px; border:1px solid var(--stroke);">
          <div style="height:8px"></div>
          <button type="submit" class="cta-button" style="width:100%; max-width:none;">Search</button>
        </form>
      </div>
    </section>

  </main>

  <!-- Footer -->
  <footer class="app-footer" role="contentinfo">
    <p><strong>DISCLAIMER:</strong> EcoSort offers guidance based on public recycling guidelines. Always double-check local regulations — rules can change. We do not provide legal or professional waste-management advice.</p>
    <p>Currently operating in Spain, Portugal, Italy (Rome & Naples), Germany, Austria, Netherlands and France.</p>

    <div class="contact-links">
      <a href="/privacy">Privacy Policy</a>
      <span>|</span>
      <a href="mailto:akor@ecosort.app">Contact us: akor@ecosort.app</a>
    </div>
  </footer>
</div>

<!-- Simple image lightbox script -->
<script>
  (function(){
    const images = document.querySelectorAll('.screenshots-container img');
    if (!images.length) return;

    const modal = document.createElement('div');
    modal.className = 'image-modal';
    modal.innerHTML = '<button class="visually-hidden" id="lb-close">Close</button><img alt="" /><button class="visually-hidden">next</button>';
    document.body.appendChild(modal);
    const modalImg = modal.querySelector('img');

    images.forEach(img => {
      img.addEventListener('click', () => {
        const src = img.getAttribute('data-full') || img.src;
        modalImg.src = src;
        modal.classList.add('open');
        document.body.style.overflow = 'hidden';
      });
    });

    modal.addEventListener('click', (e) => {
      if (e.target === modal || e.target === modalImg) {
        modal.classList.remove('open');
        document.body.style.overflow = '';
      }
    });

    // close on Esc
    document.addEventListener('keydown', (e) => {
      if (e.key === 'Escape') {
        modal.classList.remove('open');
        document.body.style.overflow = '';
      }
    });
  })();
</script>
