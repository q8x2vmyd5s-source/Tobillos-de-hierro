<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TOBILLOS DE HIERRO — Guía de Recuperación 7 Días</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=DM+Sans:ital,wght@0,300;0,400;0,500;0,700;1,300&family=DM+Serif+Display:ital@0;1&display=swap" rel="stylesheet">
<style>
  :root {
    --iron: #0a0a0f;
    --steel: #12131a;
    --slate: #1c1e2a;
    --edge: #e8e0d4;
    --warm: #c8bfad;
    --gold: #d4a853;
    --amber: #e8961e;
    --rust: #c45c2a;
    --muted: #6b6a72;
    --signal: #3d9e7a;
    --warn: #d4734a;
    --alert: #8b4513;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  html {
    scroll-behavior: smooth;
  }

  body {
    background: var(--iron);
    color: var(--edge);
    font-family: 'DM Sans', sans-serif;
    font-size: 17px;
    line-height: 1.75;
    overflow-x: hidden;
  }

  /* ── COVER ── */
  .cover {
    min-height: 100vh;
    background: var(--iron);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 60px 32px;
    position: relative;
    overflow: hidden;
  }

  .cover::before {
    content: '';
    position: absolute;
    inset: 0;
    background:
      radial-gradient(ellipse 80% 60% at 50% 100%, rgba(212,168,83,0.12) 0%, transparent 70%),
      radial-gradient(ellipse 40% 40% at 80% 20%, rgba(196,92,42,0.08) 0%, transparent 60%);
    pointer-events: none;
  }

  .cover-badge {
    display: inline-block;
    font-family: 'DM Sans', sans-serif;
    font-size: 11px;
    font-weight: 700;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    color: var(--gold);
    border: 1px solid rgba(212,168,83,0.35);
    padding: 6px 20px;
    border-radius: 2px;
    margin-bottom: 40px;
    animation: fadeUp 0.8s ease forwards;
    opacity: 0;
  }

  .cover-title {
    font-family: 'Bebas Neue', sans-serif;
    font-size: clamp(72px, 14vw, 148px);
    letter-spacing: 0.04em;
    line-height: 0.88;
    color: var(--edge);
    position: relative;
    animation: fadeUp 0.8s 0.2s ease forwards;
    opacity: 0;
  }

  .cover-title span {
    display: block;
    color: var(--gold);
    font-size: clamp(48px, 9vw, 96px);
    letter-spacing: 0.12em;
  }

  .cover-divider {
    width: 60px;
    height: 2px;
    background: linear-gradient(90deg, transparent, var(--gold), transparent);
    margin: 36px auto;
    animation: fadeUp 0.8s 0.4s ease forwards;
    opacity: 0;
  }

  .cover-sub {
    font-family: 'DM Serif Display', serif;
    font-style: italic;
    font-size: clamp(18px, 3vw, 26px);
    color: var(--warm);
    max-width: 520px;
    line-height: 1.5;
    animation: fadeUp 0.8s 0.6s ease forwards;
    opacity: 0;
  }

  .cover-tag {
    margin-top: 48px;
    display: flex;
    gap: 28px;
    justify-content: center;
    flex-wrap: wrap;
    animation: fadeUp 0.8s 0.8s ease forwards;
    opacity: 0;
  }

  .cover-tag span {
    font-size: 13px;
    color: var(--muted);
    letter-spacing: 0.08em;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .cover-tag span::before {
    content: '◆';
    color: var(--gold);
    font-size: 8px;
  }

  .scroll-hint {
    position: absolute;
    bottom: 32px;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 8px;
    color: var(--muted);
    font-size: 11px;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    animation: fadeUp 1s 1.2s ease forwards, bob 2s 2s ease-in-out infinite;
    opacity: 0;
  }

  .scroll-hint::after {
    content: '↓';
    font-size: 18px;
    color: var(--gold);
  }

  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(24px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes bob {
    0%, 100% { transform: translateX(-50%) translateY(0); }
    50% { transform: translateX(-50%) translateY(6px); }
  }

  /* ── SECTIONS ── */
  .section {
    max-width: 740px;
    margin: 0 auto;
    padding: 80px 32px;
  }

  .section + .section {
    border-top: 1px solid rgba(255,255,255,0.05);
  }

  /* ── CHAPTER MARKER ── */
  .chapter-marker {
    display: flex;
    align-items: center;
    gap: 16px;
    margin-bottom: 48px;
  }

  .chapter-number {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 72px;
    line-height: 1;
    color: rgba(212,168,83,0.15);
    letter-spacing: -0.02em;
  }

  .chapter-info {
    border-left: 2px solid var(--gold);
    padding-left: 16px;
  }

  .chapter-label {
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 4px;
  }

  .chapter-title {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 28px;
    letter-spacing: 0.06em;
    color: var(--edge);
  }

  /* ── TYPOGRAPHY ── */
  h2 {
    font-family: 'Bebas Neue', sans-serif;
    font-size: clamp(32px, 5vw, 48px);
    letter-spacing: 0.06em;
    line-height: 1.05;
    color: var(--edge);
    margin-bottom: 24px;
  }

  h3 {
    font-family: 'DM Serif Display', serif;
    font-size: clamp(20px, 3vw, 26px);
    color: var(--warm);
    margin: 36px 0 16px;
    font-style: italic;
  }

  p {
    color: var(--warm);
    margin-bottom: 18px;
    font-weight: 300;
  }

  strong {
    color: var(--edge);
    font-weight: 700;
  }

  /* ── HOOK BLOCK ── */
  .hook-block {
    background: var(--steel);
    border-left: 3px solid var(--rust);
    padding: 32px 36px;
    margin: 36px 0;
    border-radius: 0 4px 4px 0;
  }

  .hook-block p {
    font-size: 18px;
    line-height: 1.6;
    margin-bottom: 12px;
  }

  .hook-block p:last-child { margin-bottom: 0; }

  /* ── PAIN LIST ── */
  .pain-list {
    list-style: none;
    margin: 24px 0;
  }

  .pain-list li {
    display: flex;
    align-items: flex-start;
    gap: 14px;
    padding: 12px 0;
    border-bottom: 1px solid rgba(255,255,255,0.04);
    color: var(--warm);
    font-size: 16px;
  }

  .pain-list li::before {
    content: '→';
    color: var(--rust);
    font-size: 14px;
    margin-top: 2px;
    flex-shrink: 0;
  }

  /* ── HIGHLIGHT PHRASE ── */
  .impact {
    font-family: 'DM Serif Display', serif;
    font-style: italic;
    font-size: clamp(22px, 3.5vw, 30px);
    color: var(--gold);
    text-align: center;
    padding: 40px 0;
    line-height: 1.4;
    position: relative;
  }

  .impact::before, .impact::after {
    content: '';
    display: block;
    width: 40px;
    height: 1px;
    background: var(--gold);
    margin: 0 auto 20px;
    opacity: 0.4;
  }
  .impact::after { margin: 20px auto 0; }

  /* ── PROMISE BOX ── */
  .promise-box {
    background: linear-gradient(135deg, rgba(61,158,122,0.08), rgba(61,158,122,0.03));
    border: 1px solid rgba(61,158,122,0.25);
    padding: 36px;
    border-radius: 4px;
    margin: 36px 0;
  }

  .promise-box .promise-title {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 13px;
    letter-spacing: 0.25em;
    color: var(--signal);
    margin-bottom: 20px;
  }

  .promise-list {
    list-style: none;
  }

  .promise-list li {
    display: flex;
    align-items: flex-start;
    gap: 12px;
    padding: 10px 0;
    color: var(--warm);
    font-size: 16px;
  }

  .promise-list li::before {
    content: '✓';
    color: var(--signal);
    font-weight: 700;
    flex-shrink: 0;
  }

  /* ── DIAGNÓSTICO ── */
  .test-card {
    background: var(--slate);
    border-radius: 6px;
    padding: 32px;
    margin: 24px 0;
    border-top: 2px solid var(--gold);
  }

  .test-card .test-label {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 13px;
    letter-spacing: 0.25em;
    color: var(--gold);
    margin-bottom: 12px;
  }

  .test-card h4 {
    font-family: 'DM Serif Display', serif;
    font-size: 20px;
    color: var(--edge);
    margin-bottom: 20px;
  }

  .test-steps {
    list-style: none;
    margin-bottom: 24px;
  }

  .test-steps li {
    display: flex;
    gap: 12px;
    padding: 8px 0;
    color: var(--warm);
    font-size: 15px;
  }

  .test-steps li .step-num {
    background: rgba(212,168,83,0.15);
    color: var(--gold);
    font-size: 11px;
    font-weight: 700;
    width: 22px;
    height: 22px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    margin-top: 1px;
  }

  .result-grid {
    display: grid;
    gap: 8px;
  }

  .result-item {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 10px 16px;
    border-radius: 4px;
    font-size: 14px;
    font-weight: 500;
  }

  .result-item.ok { background: rgba(61,158,122,0.1); color: #7ecfb0; }
  .result-item.warn { background: rgba(212,168,83,0.1); color: #d4a853; }
  .result-item.bad { background: rgba(196,92,42,0.1); color: #d4734a; }

  /* ── ERROR BLOCK ── */
  .error-block {
    background: rgba(196,92,42,0.08);
    border: 1px solid rgba(196,92,42,0.2);
    border-radius: 6px;
    padding: 32px;
    margin: 32px 0;
    position: relative;
  }

  .error-block .error-label {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 11px;
    letter-spacing: 0.3em;
    color: var(--warn);
    margin-bottom: 16px;
  }

  .error-block p {
    color: var(--warm);
    font-size: 15px;
  }

  /* ── FLOW DIAGRAM ── */
  .flow {
    display: flex;
    flex-direction: column;
    gap: 4px;
    margin: 24px 0;
  }

  .flow-item {
    display: flex;
    align-items: center;
    gap: 16px;
    padding: 14px 20px;
    background: var(--slate);
    border-radius: 4px;
  }

  .flow-item .flow-icon {
    font-size: 18px;
    flex-shrink: 0;
  }

  .flow-item p {
    margin: 0;
    font-size: 15px;
    color: var(--warm);
  }

  .flow-arrow {
    text-align: center;
    color: var(--muted);
    font-size: 12px;
    padding: 2px 0;
  }

  /* ── EXERCISE CARD ── */
  .exercise-card {
    background: var(--steel);
    border-radius: 6px;
    padding: 28px;
    margin: 20px 0;
    display: grid;
    grid-template-columns: 1fr;
    gap: 16px;
    border-bottom: 2px solid transparent;
    transition: border-color 0.2s;
  }

  .exercise-card:hover {
    border-bottom-color: var(--gold);
  }

  .exercise-num {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 11px;
    letter-spacing: 0.3em;
    color: var(--gold);
  }

  .exercise-name {
    font-family: 'DM Serif Display', serif;
    font-size: 22px;
    color: var(--edge);
    margin-bottom: 4px;
  }

  .exercise-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin-top: 4px;
  }

  .tag {
    font-size: 12px;
    font-weight: 600;
    padding: 4px 12px;
    border-radius: 2px;
    letter-spacing: 0.05em;
  }

  .tag-ok { background: rgba(61,158,122,0.15); color: #7ecfb0; }
  .tag-bad { background: rgba(196,92,42,0.15); color: #d4734a; }
  .tag-tip { background: rgba(212,168,83,0.1); color: var(--gold); }

  .exercise-tip {
    font-size: 14px;
    color: var(--muted);
    font-style: italic;
  }

  /* ── ROUTINE BOX ── */
  .routine-box {
    background: linear-gradient(135deg, var(--slate), var(--steel));
    border: 1px solid rgba(212,168,83,0.2);
    border-radius: 8px;
    padding: 40px;
    margin: 36px 0;
  }

  .routine-title {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 20px;
    letter-spacing: 0.15em;
    color: var(--gold);
    margin-bottom: 28px;
    text-align: center;
  }

  .routine-item {
    display: flex;
    align-items: center;
    gap: 20px;
    padding: 14px 0;
    border-bottom: 1px solid rgba(255,255,255,0.05);
  }

  .routine-item:last-child { border-bottom: none; }

  .routine-icon {
    font-size: 22px;
    flex-shrink: 0;
  }

  .routine-text {
    flex: 1;
  }

  .routine-text strong {
    display: block;
    font-size: 15px;
    color: var(--edge);
    margin-bottom: 2px;
  }

  .routine-text span {
    font-size: 13px;
    color: var(--muted);
  }

  .routine-reps {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 22px;
    color: var(--gold);
    letter-spacing: 0.05em;
  }

  /* ── LIMITATION BLOCK (CRÍTICO CONVERSIÓN) ── */
  .limitation-block {
    background: var(--iron);
    border: 1px solid rgba(212,168,83,0.15);
    border-top: 3px solid var(--gold);
    border-radius: 0 0 8px 8px;
    padding: 48px 40px;
    margin: 40px 0;
    position: relative;
    overflow: hidden;
  }

  .limitation-block::before {
    content: '⚠';
    position: absolute;
    top: -20px;
    right: 32px;
    font-size: 120px;
    color: rgba(212,168,83,0.04);
    font-style: normal;
    line-height: 1;
  }

  .limitation-label {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 11px;
    letter-spacing: 0.35em;
    color: var(--gold);
    margin-bottom: 20px;
  }

  .limitation-block h2 {
    font-size: clamp(26px, 4vw, 38px);
  }

  .need-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
    margin: 32px 0;
  }

  @media (max-width: 560px) {
    .need-grid { grid-template-columns: 1fr; }
  }

  .need-card {
    background: var(--steel);
    border-radius: 6px;
    padding: 20px;
    text-align: center;
  }

  .need-card .need-icon {
    font-size: 28px;
    margin-bottom: 12px;
  }

  .need-card .need-title {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 15px;
    letter-spacing: 0.1em;
    color: var(--edge);
    margin-bottom: 8px;
  }

  .need-card p {
    font-size: 13px;
    color: var(--muted);
    margin: 0;
  }

  /* ── TRANSITION SECTION ── */
  .transition-block {
    background: linear-gradient(180deg, rgba(212,168,83,0.06) 0%, transparent 100%);
    border-top: 1px solid rgba(212,168,83,0.2);
    padding: 60px 32px;
    text-align: center;
  }

  .transition-block .transition-eyebrow {
    font-size: 11px;
    font-weight: 700;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 20px;
  }

  .insight-text {
    font-family: 'DM Serif Display', serif;
    font-size: clamp(20px, 3.5vw, 28px);
    color: var(--edge);
    line-height: 1.5;
    max-width: 560px;
    margin: 0 auto 32px;
  }

  .insight-sub {
    color: var(--muted);
    font-size: 15px;
    max-width: 480px;
    margin: 0 auto;
  }

  /* ── PRODUCT INTRO (TOBILLERA) ── */
  .product-intro {
    background: var(--steel);
    border-radius: 8px;
    padding: 48px 40px;
    margin: 0 32px 40px;
    max-width: 676px;
    margin-left: auto;
    margin-right: auto;
    position: relative;
  }

  .product-intro::before {
    content: '';
    position: absolute;
    inset: 0;
    background: radial-gradient(ellipse 80% 60% at 50% 100%, rgba(212,168,83,0.06), transparent);
    border-radius: 8px;
    pointer-events: none;
  }

  .product-label {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 11px;
    letter-spacing: 0.35em;
    color: var(--signal);
    margin-bottom: 20px;
    display: flex;
    align-items: center;
    gap: 10px;
  }

  .product-label::before {
    content: '';
    display: block;
    width: 24px;
    height: 1px;
    background: var(--signal);
  }

  .product-intro h2 {
    font-size: clamp(26px, 4vw, 38px);
    margin-bottom: 20px;
  }

  .product-intro p {
    font-size: 16px;
    line-height: 1.7;
  }

  .vs-block {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 16px;
    margin: 32px 0;
  }

  @media (max-width: 480px) {
    .vs-block { grid-template-columns: 1fr; }
  }

  .vs-col {
    padding: 24px;
    border-radius: 6px;
  }

  .vs-col.no {
    background: rgba(196,92,42,0.08);
    border: 1px solid rgba(196,92,42,0.15);
  }

  .vs-col.yes {
    background: rgba(61,158,122,0.08);
    border: 1px solid rgba(61,158,122,0.2);
  }

  .vs-label {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 11px;
    letter-spacing: 0.25em;
    margin-bottom: 16px;
  }

  .vs-col.no .vs-label { color: var(--warn); }
  .vs-col.yes .vs-label { color: var(--signal); }

  .vs-list {
    list-style: none;
  }

  .vs-list li {
    font-size: 14px;
    color: var(--warm);
    padding: 7px 0;
    border-bottom: 1px solid rgba(255,255,255,0.04);
    display: flex;
    gap: 10px;
  }

  .vs-list li:last-child { border-bottom: none; }

  .vs-col.no .vs-list li::before { content: '✕'; color: var(--warn); flex-shrink: 0; }
  .vs-col.yes .vs-list li::before { content: '✓'; color: var(--signal); flex-shrink: 0; }

  .soft-cta {
    background: rgba(212,168,83,0.06);
    border: 1px solid rgba(212,168,83,0.2);
    border-radius: 4px;
    padding: 24px 28px;
    margin-top: 32px;
  }

  .soft-cta p {
    font-size: 15px;
    color: var(--warm);
    margin: 0 0 16px;
  }

  .soft-cta .cta-link {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    font-family: 'DM Sans', sans-serif;
    font-size: 14px;
    font-weight: 700;
    color: var(--gold);
    text-decoration: none;
    letter-spacing: 0.05em;
    transition: gap 0.2s;
  }

  .soft-cta .cta-link:hover { gap: 16px; }
  .soft-cta .cta-link::after { content: '→'; }

  /* ── CLOSE SECTION ── */
  .close-section {
    max-width: 740px;
    margin: 0 auto;
    padding: 80px 32px;
  }

  .result-cards {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
    margin: 36px 0;
  }

  @media (max-width: 560px) {
    .result-cards { grid-template-columns: 1fr; }
  }

  .result-card {
    background: var(--slate);
    border-radius: 6px;
    padding: 24px;
    text-align: center;
  }

  .result-card .r-icon {
    font-size: 32px;
    margin-bottom: 12px;
  }

  .result-card .r-title {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 16px;
    letter-spacing: 0.1em;
    color: var(--edge);
    margin-bottom: 6px;
  }

  .result-card p {
    font-size: 13px;
    color: var(--muted);
    margin: 0;
  }

  /* ── SUMMARY STRIP ── */
  .summary {
    background: var(--steel);
    border-top: 1px solid rgba(255,255,255,0.06);
    border-bottom: 1px solid rgba(255,255,255,0.06);
    padding: 56px 32px;
    margin: 40px 0;
  }

  .summary-inner {
    max-width: 740px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 40px;
  }

  @media (max-width: 640px) {
    .summary-inner { grid-template-columns: 1fr; gap: 32px; }
  }

  .summary-col h4 {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 13px;
    letter-spacing: 0.2em;
    color: var(--gold);
    margin-bottom: 16px;
  }

  .summary-col ul {
    list-style: none;
  }

  .summary-col ul li {
    font-size: 14px;
    color: var(--warm);
    padding: 6px 0;
    border-bottom: 1px solid rgba(255,255,255,0.04);
    display: flex;
    gap: 10px;
  }

  .summary-col ul li::before {
    color: var(--gold);
    font-size: 10px;
    flex-shrink: 0;
    margin-top: 4px;
  }

  .summary-col.green ul li::before { content: '✓'; color: var(--signal); }
  .summary-col.warn ul li::before { content: '✕'; color: var(--warn); }
  .summary-col.action ul li::before { content: '→'; color: var(--gold); }

  /* ── FINAL CTA ── */
  .final-cta {
    text-align: center;
    padding: 80px 32px;
    background: linear-gradient(180deg, var(--iron) 0%, rgba(212,168,83,0.06) 50%, var(--iron) 100%);
  }

  .final-cta .big-line {
    font-family: 'Bebas Neue', sans-serif;
    font-size: clamp(40px, 7vw, 80px);
    letter-spacing: 0.04em;
    color: var(--edge);
    line-height: 1;
    margin-bottom: 8px;
  }

  .final-cta .big-line span { color: var(--gold); }

  .final-cta p {
    font-size: 16px;
    color: var(--muted);
    max-width: 400px;
    margin: 20px auto 40px;
  }

  .cta-button {
    display: inline-flex;
    align-items: center;
    gap: 12px;
    background: var(--gold);
    color: var(--iron);
    font-family: 'DM Sans', sans-serif;
    font-size: 15px;
    font-weight: 700;
    padding: 16px 36px;
    border-radius: 3px;
    text-decoration: none;
    letter-spacing: 0.05em;
    transition: background 0.2s, gap 0.2s;
  }

  .cta-button:hover {
    background: var(--amber);
    gap: 18px;
  }

  .cta-button::after { content: '→'; font-size: 18px; }

  .cta-note {
    margin-top: 16px;
    font-size: 13px;
    color: var(--muted);
    letter-spacing: 0.04em;
  }

  /* ── FOOTER ── */
  footer {
    text-align: center;
    padding: 40px 32px;
    font-size: 12px;
    color: rgba(255,255,255,0.15);
    letter-spacing: 0.1em;
    border-top: 1px solid rgba(255,255,255,0.04);
  }

  /* ── UTILITIES ── */
  .gold { color: var(--gold); }
  .signal { color: var(--signal); }
  .warn-c { color: var(--warn); }
  .muted { color: var(--muted); }

  .text-center { text-align: center; }
  .mb-0 { margin-bottom: 0; }

  .separator {
    width: 100%;
    height: 1px;
    background: linear-gradient(90deg, transparent, rgba(212,168,83,0.3), transparent);
    margin: 0;
    border: none;
  }

  .kicker {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 13px;
    letter-spacing: 0.3em;
    color: var(--gold);
    display: block;
    margin-bottom: 12px;
  }

  .big-insight {
    font-family: 'DM Serif Display', serif;
    font-size: clamp(18px, 2.8vw, 24px);
    color: var(--edge);
    line-height: 1.6;
    text-align: center;
    max-width: 560px;
    margin: 0 auto 16px;
  }

  /* ── PRINT / A4 CONSIDERATIONS ── */
  @media print {
    body { background: white; color: #111; }
    .cover { background: white; }
  }
</style>
</head>
<body>

<!-- ████████ PORTADA ████████ -->
<section class="cover">
  <div class="cover-badge">Guía de recuperación · Edición gratuita</div>

  <h1 class="cover-title">
    TOBILLOS
    <span>DE HIERRO</span>
  </h1>

  <div class="cover-divider"></div>

  <p class="cover-sub">
    Recupera movilidad, elimina molestias y vuelve a moverte sin dolor<br>
    <strong>en solo 7 días</strong> — sin dejar de entrenar
  </p>

  <div class="cover-tag">
    <span>Plan de 5 minutos al día</span>
    <span>Diagnóstico rápido incluido</span>
    <span>Sin tecnicismos</span>
  </div>

  <div class="scroll-hint">Empieza aquí</div>
</section>

<hr class="separator">


<!-- ████████ HOOK EMOCIONAL ████████ -->
<section class="section">

  <div class="chapter-marker">
    <div class="chapter-number">01</div>
    <div class="chapter-info">
      <div class="chapter-label">Antes de empezar</div>
      <div class="chapter-title">¿Te suena esto?</div>
    </div>
  </div>

  <div class="hook-block">
    <p>No es un dolor insoportable.</p>
    <p>Pero está ahí.</p>
    <p>Y no se va.</p>
  </div>

  <ul class="pain-list">
    <li>Notas rigidez al bajar escaleras por la mañana</li>
    <li>Sientes molestias al correr, saltar o cambiar de dirección</li>
    <li>Tu tobillo "no responde" con la misma firmeza que antes</li>
    <li>Has descansado semanas… y al volver, vuelve igual</li>
    <li>Tienes la sensación de que algo no está bien, pero no sabes exactamente qué</li>
  </ul>

  <div class="impact">
    "Aquí es donde la mayoría comete el error más grande."
  </div>

  <p>O ignoran el problema y siguen adelante cruzando los dedos.<br>
  O paran completamente esperando que el tiempo lo arregle solo.</p>

  <p><strong>Ninguna de las dos funciona.</strong></p>

  <p>Porque el tobillo no necesita descanso absoluto.<br>
  Necesita el <em>estímulo correcto</em>.</p>

  <p>Y eso es exactamente lo que vas a encontrar aquí.</p>

</section>

<hr class="separator">


<!-- ████████ PROMESA CLARA ████████ -->
<section class="section">

  <div class="chapter-marker">
    <div class="chapter-number">02</div>
    <div class="chapter-info">
      <div class="chapter-label">La promesa</div>
      <div class="chapter-title">Qué vas a conseguir</div>
    </div>
  </div>

  <h2>En los próximos 7 días</h2>

  <div class="promise-box">
    <div class="promise-title">✦ Plan de acción inmediata</div>
    <ul class="promise-list">
      <li>Detectar exactamente en qué punto está tu tobillo ahora mismo</li>
      <li>Entender el error que está frenando tu recuperación sin que lo sepas</li>
      <li>Aplicar una rutina de 5 minutos al día con resultados reales</li>
      <li>Sentir una diferencia tangible antes de que acabe la semana</li>
    </ul>
  </div>

  <p>No es magia.<br>
  Es aplicar el estímulo correcto, en el orden correcto.</p>

  <p class="muted" style="font-size:14px; font-style: italic;">
    Nota: si ahora mismo tienes dolor agudo, inflamación importante o sospechas de una lesión sin diagnosticar, consulta con un profesional antes de empezar.
  </p>

</section>

<hr class="separator">


<!-- ████████ DIAGNÓSTICO ████████ -->
<section class="section">

  <div class="chapter-marker">
    <div class="chapter-number">03</div>
    <div class="chapter-info">
      <div class="chapter-label">Paso 1</div>
      <div class="chapter-title">Diagnóstico rápido</div>
    </div>
  </div>

  <h2>Primero necesitas saber dónde estás</h2>

  <p>Antes de hacer un solo ejercicio, haz estos tres tests.<br>
  Tardan menos de 2 minutos y te dicen todo lo importante.</p>

  <!-- TEST 1 -->
  <div class="test-card">
    <div class="test-label">Test 01 — Movilidad</div>
    <h4>Rodilla a la pared</h4>
    <ul class="test-steps">
      <li><span class="step-num">1</span>Coloca el pie a unos 10 cm de una pared</li>
      <li><span class="step-num">2</span>Intenta tocar la pared con la rodilla sin levantar el talón</li>
      <li><span class="step-num">3</span>Observa si llegas, si te cuesta o si el talón se levanta</li>
    </ul>
    <div class="result-grid">
      <div class="result-item ok">✓ Llegas sin compensar → movilidad aceptable</div>
      <div class="result-item warn">⚠ Te cuesta o compensas → restricción moderada</div>
      <div class="result-item bad">✕ No llegas o el talón sube → restricción clara</div>
    </div>
  </div>

  <!-- TEST 2 -->
  <div class="test-card">
    <div class="test-label">Test 02 — Estabilidad</div>
    <h4>Equilibrio a una pierna</h4>
    <ul class="test-steps">
      <li><span class="step-num">1</span>Levanta un pie y mantente en equilibrio sobre el otro</li>
      <li><span class="step-num">2</span>Intenta aguantar 20 segundos con los ojos abiertos</li>
      <li><span class="step-num">3</span>Observa si hay temblor o si pierdes el control</li>
    </ul>
    <div class="result-grid">
      <div class="result-item ok">✓ Estable durante 20 s → buen control</div>
      <div class="result-item warn">⚠ Temblor visible → déficit de control</div>
      <div class="result-item bad">✕ Pierdes equilibrio → control muy limitado</div>
    </div>
  </div>

  <!-- TEST 3 -->
  <div class="test-card">
    <div class="test-label">Test 03 — Sensación subjetiva</div>
    <h4>¿Qué notas tú?</h4>
    <ul class="test-steps">
      <li><span class="step-num">→</span>¿Rigidez al levantarte o al empezar a moverte?</li>
      <li><span class="step-num">→</span>¿Molestia al cargar tu propio peso?</li>
      <li><span class="step-num">→</span>¿Sensación de "tobillo débil" o poco fiable?</li>
    </ul>
    <div class="result-grid">
      <div class="result-item warn">⚠ Si has respondido sí a 1 o más → tu tobillo necesita trabajo activo ahora</div>
    </div>
  </div>

  <div class="impact">
    Guarda estos resultados. Los vas a necesitar al final de los 7 días.
  </div>

</section>

<hr class="separator">


<!-- ████████ ERROR Nº1 ████████ -->
<section class="section">

  <div class="chapter-marker">
    <div class="chapter-number">04</div>
    <div class="chapter-info">
      <div class="chapter-label">El problema real</div>
      <div class="chapter-title">Por qué no mejoras</div>
    </div>
  </div>

  <h2>El error que comete casi todo el mundo</h2>

  <div class="error-block">
    <div class="error-label">⚠ Error número 1</div>
    <p><strong>"Tengo molestias → mejor descanso"</strong></p>
    <p>Este es el mayor freno para la recuperación. Y lo aplica la mayoría.</p>
  </div>

  <h3>¿Qué está pasando dentro?</h3>

  <p>Tu cuerpo funciona por adaptación.<br>
  Cuando dejas de usar una estructura, esa estructura <em>pierde capacidad</em>.</p>

  <p>No porque empeore la lesión. Sino porque sin estímulo, el tejido se vuelve más rígido, la musculatura pierde tono y el sistema nervioso pierde el "mapa" del movimiento.</p>

  <div class="flow">
    <div class="flow-item">
      <span class="flow-icon">🔕</span>
      <p>Menos movimiento → menos señal al sistema nervioso</p>
    </div>
    <div class="flow-arrow">↓</div>
    <div class="flow-item">
      <span class="flow-icon">📉</span>
      <p>Menos señal → menos adaptación del tejido</p>
    </div>
    <div class="flow-arrow">↓</div>
    <div class="flow-item">
      <span class="flow-icon">🔒</span>
      <p>Resultado → más rigidez, menos control, mayor riesgo de recaída</p>
    </div>
  </div>

  <div class="impact">
    "No necesitas dejar de usarlo.<br>Necesitas usarlo bien."
  </div>

  <p>Esa es la diferencia entre quedarte atascado y empezar a mejorar de verdad.</p>

</section>

<hr class="separator">


<!-- ████████ PLAN PRÁCTICO ████████ -->
<section class="section">

  <div class="chapter-marker">
    <div class="chapter-number">05</div>
    <div class="chapter-info">
      <div class="chapter-label">El sistema</div>
      <div class="chapter-title">Plan de recuperación</div>
    </div>
  </div>

  <h2>No necesitas 20 ejercicios.<br>Necesitas los correctos.</h2>

  <p>Estos cuatro ejercicios atacan exactamente lo que tu tobillo necesita recuperar:</p>

  <!-- EJ 1 -->
  <div class="exercise-card">
    <div class="exercise-num">Ejercicio 01</div>
    <div class="exercise-name">Movilidad en pared</div>
    <p style="font-size:14px; color: var(--muted); margin: 0;">Rodilla hacia la pared, talón sin despegar del suelo. Movimiento lento y controlado.</p>
    <div class="exercise-tags">
      <span class="tag tag-ok">Talón siempre apoyado</span>
      <span class="tag tag-ok">Movimiento sin rebotes</span>
      <span class="tag tag-bad">Sin levantar el talón</span>
      <span class="tag tag-tip">Acércate más si no llegas</span>
    </div>
    <p class="exercise-tip">Objetivo: recuperar el rango de flexión dorsal, el más limitado en casi todos los casos.</p>
  </div>

  <!-- EJ 2 -->
  <div class="exercise-card">
    <div class="exercise-num">Ejercicio 02</div>
    <div class="exercise-name">Elevaciones de talón</div>
    <p style="font-size:14px; color: var(--muted); margin: 0;">Sube despacio. Baja más despacio todavía. La bajada es donde se construye la fuerza real.</p>
    <div class="exercise-tags">
      <span class="tag tag-ok">Subida controlada</span>
      <span class="tag tag-ok">Bajada lenta (3-4 segundos)</span>
      <span class="tag tag-bad">Sin hacerlo rápido</span>
      <span class="tag tag-tip">Empieza con dos piernas si hay molestia</span>
    </div>
    <p class="exercise-tip">Objetivo: activar el complejo sóleo-gemelo, responsable de absorber impacto en cada paso.</p>
  </div>

  <!-- EJ 3 -->
  <div class="exercise-card">
    <div class="exercise-num">Ejercicio 03</div>
    <div class="exercise-name">Equilibrio a una pierna</div>
    <p style="font-size:14px; color: var(--muted); margin: 0;">Mantén la postura. Activa el pie contra el suelo. Mira al frente, no al suelo.</p>
    <div class="exercise-tags">
      <span class="tag tag-ok">Postura estable</span>
      <span class="tag tag-ok">Pie activo</span>
      <span class="tag tag-bad">Sin mirar al suelo</span>
      <span class="tag tag-tip">Usa un punto fijo para la mirada</span>
    </div>
    <p class="exercise-tip">Objetivo: reconectar el sistema nervioso con el tobillo. Aquí es donde se reeducra el equilibrio.</p>
  </div>

  <!-- EJ 4 -->
  <div class="exercise-card">
    <div class="exercise-num">Ejercicio 04</div>
    <div class="exercise-name">Círculos de tobillo</div>
    <p style="font-size:14px; color: var(--muted); margin: 0;">Movimiento lento, con control total. No es girar rápido — es explorar el rango disponible.</p>
    <div class="exercise-tags">
      <span class="tag tag-ok">Círculo completo y pausado</span>
      <span class="tag tag-ok">Máximo rango sin forzar</span>
      <span class="tag tag-bad">Sin movimiento mecánico sin control</span>
      <span class="tag tag-tip">Reduce el rango si hay molestia</span>
    </div>
    <p class="exercise-tip">Objetivo: mantener la sinovial activa y el rango articular completo en todos los planos.</p>
  </div>

</section>

<hr class="separator">


<!-- ████████ RUTINA DIARIA ████████ -->
<section class="section">

  <div class="chapter-marker">
    <div class="chapter-number">06</div>
    <div class="chapter-info">
      <div class="chapter-label">El sistema diario</div>
      <div class="chapter-title">5 minutos al día</div>
    </div>
  </div>

  <h2>Esto es lo único que necesitas hacer</h2>

  <p>No una hora en el gimnasio. No equipamiento especial.<br>
  Solo este bloque, cada día, durante 7 días.</p>

  <div class="routine-box">
    <div class="routine-title">◆ RUTINA DIARIA — TOBILLOS DE HIERRO ◆</div>

    <div class="routine-item">
      <span class="routine-icon">🧱</span>
      <div class="routine-text">
        <strong>Movilidad en pared</strong>
        <span>Talón apoyado · Movimiento lento</span>
      </div>
      <span class="routine-reps">2 × 10</span>
    </div>

    <div class="routine-item">
      <span class="routine-icon">⬆️</span>
      <div class="routine-text">
        <strong>Elevaciones de talón</strong>
        <span>Subida controlada · Bajada lenta</span>
      </div>
      <span class="routine-reps">2 × 12</span>
    </div>

    <div class="routine-item">
      <span class="routine-icon">🦶</span>
      <div class="routine-text">
        <strong>Equilibrio a una pierna</strong>
        <span>Pie activo · Mirada al frente</span>
      </div>
      <span class="routine-reps">2 × 20s</span>
    </div>

    <div class="routine-item">
      <span class="routine-icon">🔄</span>
      <div class="routine-text">
        <strong>Círculos de tobillo</strong>
        <span>Control total · Máximo rango cómodo</span>
      </div>
      <span class="routine-reps">2 × 10</span>
    </div>
  </div>

  <h3>¿Por qué funciona?</h3>

  <p>Estás dando al tobillo exactamente lo que necesita:<br>
  <strong>movimiento + carga + reeducación neuromuscular.</strong></p>

  <p>La clave no es hacer mucho un día.<br>
  Es hacer poco <em>todos los días</em>.</p>

  <div class="impact">
    "5 minutos diarios construyen más que una sesión perfecta una vez a la semana."
  </div>

  <p>En los primeros días notarás:</p>
  <ul class="pain-list">
    <li>Más rango de movimiento al levantarte</li>
    <li>Menos rigidez a lo largo del día</li>
    <li>Mayor confianza en el tobillo al caminar o bajar escaleras</li>
  </ul>

</section>

<hr class="separator">


<!-- ████████ BLOQUE LIMITACIÓN — CRÍTICO CONVERSIÓN ████████ -->
<section class="section">

  <div class="limitation-block">
    <div class="limitation-label">⚠ Lo que nadie te dice</div>

    <h2>Ya estás mejorando.<br>Pero esto no es suficiente.</h2>

    <p>Aquí es donde la mayoría se queda atascada.</p>
    <p>Las primeras mejoras llegan rápido. La rigidez baja. El movimiento vuelve.<br>
    Y entonces parece que ya está. Que el problema está resuelto.</p>
    <p><strong>Pero no lo está.</strong></p>

    <h3>El problema no es solo movilidad</h3>

    <p>Tu tobillo tiene que hacer tres cosas bien al mismo tiempo para ser realmente funcional:</p>

    <div class="need-grid">
      <div class="need-card">
        <div class="need-icon">🏋️</div>
        <div class="need-title">Estabilidad</div>
        <p>Aguantar carga sin ceder. La base de todo lo demás.</p>
      </div>
      <div class="need-card">
        <div class="need-icon">🎯</div>
        <div class="need-title">Control en movimiento</div>
        <p>No solo en estático. Correr, girar, aterrizar.</p>
      </div>
      <div class="need-card">
        <div class="need-icon">🔗</div>
        <div class="need-title">Integración total</div>
        <p>Trabajar junto con rodilla, cadera y el resto del cuerpo.</p>
      </div>
    </div>

    <p>Esta guía trabaja la movilidad y el control básico. Y eso ya es muchísimo.<br>
    Pero la recuperación completa exige más:</p>

    <div class="flow" style="margin: 24px 0;">
      <div class="flow-item">
        <span class="flow-icon">📐</span>
        <p>Progresión de carga gradual (no hacer siempre lo mismo)</p>
      </div>
      <div class="flow-arrow">+</div>
      <div class="flow-item">
        <span class="flow-icon">🔀</span>
        <p>Trabajo en diferentes planos de movimiento</p>
      </div>
      <div class="flow-arrow">+</div>
      <div class="flow-item">
        <span class="flow-icon">⚡</span>
        <p>Adaptación a impacto real (correr, saltar, cambiar de dirección)</p>
      </div>
    </div>

    <p>Si te quedas solo con los ejercicios de esta guía, vas a mejorar. Sin duda.<br>
    Pero cuando aumentes la intensidad — vuelve al entrenamiento real, al deporte, a cargar peso — hay muchas posibilidades de que el problema reaparezca.</p>

    <div class="impact">
      "Esto te saca del problema.<br>Pero no te lleva al nivel de antes."
    </div>

    <p>Falta una pieza.</p>
  </div>

</section>

<hr class="separator">


<!-- ████████ TRANSICIÓN: LO QUE FALTA ████████ -->
<div class="transition-block">
  <div class="transition-eyebrow">La pieza que falta</div>
  <p class="insight-text">
    El problema no es que los ejercicios sean malos.<br>
    Es que el tobillo necesita algo más que movilidad para estar realmente seguro.
  </p>
  <p class="insight-sub">
    Necesita soporte. Especialmente cuando la carga aumenta.
  </p>
</div>


<!-- ████████ INTRODUCCIÓN TOBILLERA ████████ -->
<div class="product-intro">

  <div class="product-label">La siguiente fase</div>

  <h2>Soporte externo:<br>cuando el ejercicio no es suficiente</h2>

  <p>Hay un momento en la recuperación de tobillo que muy poca gente anticipa.</p>

  <p>Después de recuperar movilidad, la estructura articular sigue siendo vulnerable bajo carga real. No porque los ejercicios no funcionen — es que el tejido necesita tiempo para adaptarse completamente. Y durante ese tiempo, hay un riesgo silencioso.</p>

  <p>Aquí es donde muchas personas empiezan a usar soporte externo.</p>

  <h3>¿Qué diferencia hace un buen soporte?</h3>

  <div class="vs-block">
    <div class="vs-col no">
      <div class="vs-label">Sin soporte externo</div>
      <ul class="vs-list">
        <li>El tobillo trabaja sin red de seguridad</li>
        <li>Cualquier movimiento imprevisto puede forzar la articulación</li>
        <li>Más miedo a moverse con intensidad</li>
        <li>Recuperación más lenta por exceso de precaución</li>
      </ul>
    </div>
    <div class="vs-col yes">
      <div class="vs-label">Con soporte adecuado</div>
      <ul class="vs-list">
        <li>La articulación está contenida en su rango seguro</li>
        <li>Puedes cargar más sin miedo a ceder</li>
        <li>El sistema nervioso "confía" más en el tobillo</li>
        <li>Entrenas con más libertad durante la fase de adaptación</li>
      </ul>
    </div>
  </div>

  <p>Una tobillera bien elegida no sustituye los ejercicios.<br>
  <strong>Los acelera.</strong></p>

  <p>Porque te permite hacer más — y mejor — durante la fase donde el tobillo todavía está consolidando la recuperación. No es una muleta. Es un acelerador.</p>

  <p class="muted" style="font-size: 14px; font-style: italic; margin-top: 12px;">
    Lo importante: no cualquier tobillera sirve. Necesitas una que ofrezca soporte lateral real sin limitar la flexión dorsal — la que acabas de trabajar en estos 7 días.
  </p>

  <div class="soft-cta">
    <p>Si quieres entender exactamente qué tipo de soporte necesita tu tobillo según los resultados de tu diagnóstico, aquí puedes ver cómo elegir bien:</p>
    <a href="#" class="cta-link">Ver cómo elegir el soporte correcto</a>
  </div>

</div>


<hr class="separator">


<!-- ████████ CIERRE ████████ -->
<section class="close-section">

  <div class="chapter-marker">
    <div class="chapter-number">07</div>
    <div class="chapter-info">
      <div class="chapter-label">El resultado</div>
      <div class="chapter-title">Lo que has conseguido</div>
    </div>
  </div>

  <h2>Si has llegado hasta aquí, ya tienes algo que la mayoría no tiene.</h2>

  <p>Un plan claro. Y el entendimiento de por qué funciona.</p>

  <div class="result-cards">
    <div class="result-card">
      <div class="r-icon">📐</div>
      <div class="r-title">Más rango</div>
      <p>Menos rigidez. Más libertad de movimiento en cada paso.</p>
    </div>
    <div class="result-card">
      <div class="r-icon">⚖️</div>
      <div class="r-title">Mejor control</div>
      <p>El tobillo vuelve a "escuchar" las señales del sistema nervioso.</p>
    </div>
    <div class="result-card">
      <div class="r-icon">🔒</div>
      <div class="r-title">Más confianza</div>
      <p>Vuelves a fiarte de tu tobillo. Eso es más importante de lo que parece.</p>
    </div>
  </div>

  <div class="impact">
    "Esto es el primer paso.<br>No el destino."
  </div>

  <p>Ahora sabes qué le pasa a tu tobillo. Sabes qué error evitar. Sabes qué hacer desde hoy.<br>
  Eso ya es más que el 90% de las personas que tienen el mismo problema.</p>

  <p>El siguiente nivel es darle a tu tobillo lo que necesita para estar <em>realmente</em> fuerte.<br>
  No solo mejor. Fuerte.</p>

</section>


<!-- ████████ RESUMEN ████████ -->
<div class="summary">
  <div class="summary-inner">

    <div class="summary-col green">
      <h4>Lo que funciona</h4>
      <ul>
        <li>Estímulo diario, no descanso absoluto</li>
        <li>Progresión gradual de carga</li>
        <li>5 minutos todos los días</li>
        <li>Movilidad + estabilidad juntas</li>
      </ul>
    </div>

    <div class="summary-col warn">
      <h4>Lo que no funciona</h4>
      <ul>
        <li>Parar completamente y esperar</li>
        <li>Hacer mucho un día y nada el resto</li>
        <li>Quedarse solo con la movilidad</li>
        <li>Ignorar el déficit de control</li>
      </ul>
    </div>

    <div class="summary-col action">
      <h4>Acción ahora</h4>
      <ul>
        <li>Repite los 3 tests del diagnóstico</li>
        <li>Aplica la rutina durante 7 días</li>
        <li>Evalúa si necesitas soporte externo</li>
        <li>Da el siguiente paso cuando estés listo</li>
      </ul>
    </div>

  </div>
</div>


<!-- ████████ FINAL CTA ████████ -->
<div class="final-cta">
  <div class="big-line">TU TOBILLO PUEDE</div>
  <div class="big-line">VOLVER A SER <span>FUERTE.</span></div>

  <p>La diferencia está en cómo lo trabajas a partir de ahora. Ya tienes el primer bloque. El siguiente es el que lo cambia todo.</p>

  <a href="#" class="cta-button">Ver el siguiente paso</a>

  <p class="cta-note">Sin compromiso · Solo para ver si encaja contigo</p>
</div>


<!-- ████████ FOOTER ████████ -->
<footer>
  TOBILLOS DE HIERRO · Guía Gratuita de Recuperación · Uso personal
</footer>

</body>
</html>
