* {
  box-sizing: border-box;
}

:root {
  --bg: #f9f3ee;
  --panel: #fffaf7;
  --card: #f5e8e0;
  --text: #221915;
  --muted: #6f5d56;
  --gold: #cda66e;
  --deep: #2c1a1a;
  --sage: #dfe9dc;
  --soft: #f1d9d7;
  --shadow: 0 18px 40px rgba(49, 29, 23, 0.12);
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  font-family: 'Inter', sans-serif;
  background: linear-gradient(180deg, #f8f2ee 0%, #fffaf8 100%);
  color: var(--text);
}

img {
  max-width: 100%;
  display: block;
}

button,
input {
  font: inherit;
}

button {
  border: none;
  cursor: pointer;
}

.page-shell {
  width: min(1200px, calc(100% - 32px));
  margin: 0 auto;
  padding: 28px 0 64px;
}

.topbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  padding: 18px 24px;
  border: 1px solid rgba(34, 25, 21, 0.07);
  border-radius: 999px;
  background: rgba(255, 255, 255, 0.55);
  backdrop-filter: blur(8px);
  box-shadow: 0 12px 26px rgba(34, 25, 21, 0.04);
  position: sticky;
  top: 18px;
  z-index: 10;
}

.brand-wrap {
  display: flex;
  align-items: center;
  gap: 12px;
}

.brand-mark {
  width: 42px;
  height: 42px;
  border-radius: 50%;
  display: grid;
  place-items: center;
  background: linear-gradient(135deg, #2b1a18, #5f3b2d);
  color: #f9efe8;
  font-family: 'Cormorant Garamond', serif;
  font-size: 2rem;
  font-weight: 700;
}

.brand-name {
  margin: 0;
  font-family: 'Cormorant Garamond', serif;
  font-size: 2.1rem;
  line-height: 1;
  font-weight: 700;
}

.brand-sub {
  color: var(--muted);
  font-size: 0.72rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}

.nav {
  display: flex;
  align-items: center;
  gap: 26px;
}

.nav a,
.text-link {
  text-decoration: none;
  color: var(--text);
  font-weight: 500;
}

.nav-actions {
  display: flex;
  align-items: center;
  gap: 12px;
}

.primary-btn,
.secondary-btn,
.ghost-btn,
.card-btn,
.filter-btn {
  border-radius: 999px;
  padding: 0.9rem 1.3rem;
  font-weight: 600;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.primary-btn,
.card-btn {
  background: linear-gradient(135deg, #2a1a18, #5a372e);
  color: #fff;
  box-shadow: 0 12px 22px rgba(56, 33, 28, 0.18);
}

.secondary-btn,
.ghost-btn,
.filter-btn {
  background: rgba(255, 255, 255, 0.6);
  border: 1px solid rgba(34, 25, 21, 0.08);
  color: var(--text);
}

.primary-btn:hover,
.secondary-btn:hover,
.ghost-btn:hover,
.card-btn:hover,
.filter-btn:hover {
  transform: translateY(-1px);
}

.hero-section {
  display: grid;
  grid-template-columns: 1.1fr 0.9fr;
  align-items: center;
  gap: 48px;
  padding: 60px 10px 30px;
}

.eyebrow {
  display: inline-block;
  margin-bottom: 10px;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  font-size: 0.72rem;
  color: var(--gold);
  font-weight: 700;
}

.hero-copy h1,
.section-heading h2,
.craft-copy h2 {
  margin: 0;
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(3rem, 6vw, 5.4rem);
  line-height: 0.95;
  letter-spacing: -0.04em;
}

.hero-copy p,
.craft-copy p {
  margin-top: 18px;
  max-width: 560px;
  color: var(--muted);
  font-size: 1.08rem;
  line-height: 1.8;
}

.cta-row {
  display: flex;
  flex-wrap: wrap;
  gap: 14px;
  margin-top: 28px;
}

.hero-stats {
  margin-top: 34px;
  display: grid;
  grid-template-columns: repeat(4, minmax(110px, 1fr));
  gap: 16px;
}

.stat-box {
  background: rgba(255, 255, 255, 0.6);
  border: 1px solid rgba(34, 25, 21, 0.06);
  border-radius: 18px;
  padding: 16px 12px;
  display: flex;
  flex-direction: column;
  gap: 6px;
}

.stat-box strong {
  font-size: 1.3rem;
}

.stat-box span {
  color: var(--muted);
  font-size: 0.72rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

.hero-visual {
  position: relative;
  min-height: 640px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.hero-image-wrap {
  width: min(560px, 100%);
  height: 640px;
  border-radius: 36px 36px 180px 36px;
  overflow: hidden;
  box-shadow: var(--shadow);
}

.hero-image-wrap img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.floating-card {
  position: absolute;
  padding: 16px 20px;
  border-radius: 18px;
  background: rgba(255, 249, 246, 0.88);
  border: 1px solid rgba(34, 25, 21, 0.05);
  box-shadow: 0 18px 32px rgba(56, 33, 28, 0.08);
  display: flex;
  flex-direction: column;
  gap: 4px;
}

.floating-card span {
  font-size: 0.72rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--muted);
}

.floating-card strong {
  font-size: 1.05rem;
}

.card-one {
  top: 40px;
  left: 13px;
}

.card-two {
  right: 0;
  bottom: 30px;
}

.section-heading {
  margin-bottom: 24px;
}

.section-heading h2,
.craft-copy h2 {
  font-size: clamp(2.5rem, 4vw, 4rem);
}

.category-section,
.product-section,
.testimonial-section {
  padding-top: 50px;
}

.filter-row {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-bottom: 18px;
}

.filter-btn {
  min-width: 110px;
}

.filter-btn.active {
  background: linear-gradient(135deg, #2a1a18, #5a372e);
  color: white;
  box-shadow: 0 12px 22px rgba(56, 33, 28, 0.18);
}

.product-grid,
.testimonial-grid {
  display: grid;
  gap: 24px;
}

.product-grid {
  grid-template-columns: repeat(4, minmax(0, 1fr));
}

.product-card {
  border-radius: 28px;
  overflow: hidden;
  background: rgba(255, 255, 255, 0.55);
  border: 1px solid rgba(34, 25, 21, 0.06);
}

.product-media {
  position: relative;
  height: 360px;
}

.product-media img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.product-badge {
  position: absolute;
  top: 18px;
  left: 18px;
  font-size: 0.69rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  background: rgba(255, 255, 255, 0.9);
  border-radius: 999px;
  padding: 8px 12px;
}

.product-info {
  padding: 20px 18px 22px;
}

.meta-row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 12px;
  color: var(--muted);
  font-size: 0.8rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

.meta-row strong {
  color: var(--text);
  font-size: 1rem;
  letter-spacing: 0;
  text-transform: none;
}

.product-info h3 {
  margin: 14px 0 18px;
  font-size: 1.6rem;
  font-family: 'Cormorant Garamond', serif;
}

.card-btn {
  width: 100%;
  padding: 0.85rem 1rem;
}

.craft-section {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
  align-items: center;
  padding-top: 70px;
}

.craft-copy ul {
  list-style: none;
  padding: 0;
  margin: 24px 0 0;
  display: grid;
  gap: 14px;
}

.craft-copy li {
  display: flex;
  align-items: center;
  gap: 12px;
  color: var(--text);
  font-weight: 500;
}

.craft-copy li::before {
  content: '✦';
  color: var(--gold);
}

.craft-image-panel {
  border-radius: 32px;
  overflow: hidden;
  box-shadow: var(--shadow);
}

.craft-image-panel img {
  width: 100%;
  height: 620px;
  object-fit: cover;
}

.testimonial-grid {
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.testimonial-card {
  margin: 0;
  background: rgba(255, 255, 255, 0.56);
  border: 1px solid rgba(34, 25, 21, 0.06);
  border-radius: 28px;
  padding: 28px 24px;
  box-shadow: 0 14px 28px rgba(43, 25, 21, 0.06);
}

.testimonial-card p {
  margin: 0;
  font-size: 1.08rem;
  line-height: 1.8;
  color: var(--text);
}

.testimonial-card footer {
  margin-top: 18px;
  color: var(--muted);
  font-weight: 700;
}

.footer {
  margin-top: 72px;
  padding: 32px 0 20px;
  border-top: 1px solid rgba(34, 25, 21, 0.08);
  display: flex;
  justify-content: space-between;
  align-items: end;
  gap: 30px;
}

.footer-brand span {
  display: block;
  margin-top: 8px;
  color: var(--muted);
}

.newsletter-box {
  width: min(420px, 100%);
}

.newsletter-box label {
  display: block;
  margin-bottom: 10px;
  font-weight: 600;
}

.newsletter-form {
  display: flex;
  gap: 12px;
}

.newsletter-form input {
  flex: 1;
  border-radius: 999px;
  border: 1px solid rgba(34, 25, 21, 0.08);
  background: rgba(255, 255, 255, 0.7);
  padding: 0.95rem 1rem;
}

.split-heading {
  display: flex;
  justify-content: space-between;
  align-items: end;
  gap: 20px;
}

@media (max-width: 1024px) {
  .hero-section,
  .craft-section,
  .product-grid {
    grid-template-columns: 1fr 1fr;
  }

  .hero-copy {
    grid-column: 1 / -1;
  }

  .hero-visual {
    grid-column: 1 / -1;
  }

  .nav {
    display: none;
  }
}

@media (max-width: 700px) {
  .page-shell {
    width: min(100% - 24px, 1200px);
  }

  .topbar {
    border-radius: 28px;
    padding: 16px 18px;
    flex-wrap: wrap;
  }

  .nav-actions {
    width: 100%;
    justify-content: space-between;
  }

  .hero-section,
  .craft-section,
  .product-grid,
  .testimonial-grid {
    grid-template-columns: 1fr;
  }

  .hero-image-wrap,
  .craft-image-panel img {
    height: 460px;
  }

  .hero-stats {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .footer {
    flex-direction: column;
    align-items: stretch;
  }

  .newsletter-form {
    flex-direction: column;
  }
}
