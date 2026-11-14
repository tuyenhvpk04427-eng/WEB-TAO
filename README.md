<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Con chim</title>
<style>
:root{
  --bg:#dff0f2; --sky2:#f4e9c8; --ink:#23323a; --body:#2f7f9e; --belly:#f3d9a4;
  --wing:#1f5f7a; --beak:#e8a33d; --branch:#6b4a33; --leaf:#5f9a5b;
  box-sizing:border-box; padding-top:env(safe-area-inset-top,0px); padding-bottom:env(safe-area-inset-bottom,0px);
}
@media (prefers-color-scheme: dark){
  :root:not([data-theme="light"]){ --bg:#14262d; --sky2:#2b2a24; --ink:#e8f1f3; --body:#4aa3c4; --belly:#e8c98a; --wing:#2a7a9a; --branch:#8a6446; --leaf:#6fb06a; }
}
:root[data-theme="dark"]{ --bg:#14262d; --sky2:#2b2a24; --ink:#e8f1f3; --body:#4aa3c4; --belly:#e8c98a; --wing:#2a7a9a; --branch:#8a6446; --leaf:#6fb06a; }
html{height:100%}
body{margin:0;min-height:100%;display:flex;flex-direction:column;align-items:center;justify-content:center;
  background:linear-gradient(var(--bg),var(--sky2));color:var(--ink);font-family:Georgia,"Times New Roman",serif;padding:16px}
svg{width:min(92vw,560px);height:auto}
h1{font-weight:400;font-size:1.4rem;margin:8px 0 0}
.bird{transform-origin:300px 300px;animation:bob 3.2s ease-in-out infinite}
@keyframes bob{0%,100%{transform:rotate(0)}50%{transform:rotate(-2deg)}}
@media (prefers-reduced-motion: reduce){.bird{animation:none}}
</style>
</head>
<body>
<svg viewBox="0 0 600 460" role="img" aria-label="Một con chim xanh đậu trên cành cây">
  <!-- cành cây -->
  <path d="M30 372 Q300 340 570 368" stroke="var(--branch)" stroke-width="14" fill="none" stroke-linecap="round"/>
  <path d="M470 360 q30 -40 70 -44" stroke="var(--branch)" stroke-width="7" fill="none" stroke-linecap="round"/>
  <ellipse cx="545" cy="312" rx="22" ry="11" fill="var(--leaf)" transform="rotate(-20 545 312)"/>
  <ellipse cx="90" cy="360" rx="20" ry="10" fill="var(--leaf)" transform="rotate(25 90 360)"/>

  <g class="bird">
    <!-- đuôi -->
    <path d="M190 280 L70 330 L90 345 L205 315 Z" fill="var(--wing)"/>
    <!-- thân -->
    <ellipse cx="300" cy="270" rx="125" ry="92" fill="var(--body)"/>
    <!-- bụng -->
    <path d="M230 310 Q300 360 385 300 Q350 345 300 352 Q255 350 230 310Z" fill="var(--belly)"/>
    <!-- cánh -->
    <path d="M215 250 Q290 205 355 270 Q300 330 225 300 Q200 280 215 250Z" fill="var(--wing)"/>
    <path d="M240 265 Q290 245 330 275" stroke="var(--body)" stroke-width="4" fill="none" stroke-linecap="round" opacity=".6"/>
    <!-- đầu -->
    <circle cx="410" cy="200" r="62" fill="var(--body)"/>
    <!-- mỏ -->
    <path d="M465 190 L520 208 L466 224 Z" fill="var(--beak)"/>
    <!-- mắt -->
    <circle cx="428" cy="188" r="11" fill="#fff"/>
    <circle cx="431" cy="188" r="6" fill="#111"/>
    <circle cx="433" cy="185" r="2" fill="#fff"/>
    <!-- chân -->
    <g stroke="var(--beak)" stroke-width="6" stroke-linecap="round" fill="none">
      <path d="M285 355 V362"/><path d="M275 366 l10 -4 l10 4"/>
      <path d="M335 352 V360"/><path d="M325 364 l10 -4 l10 4"/>
    </g>
  </g>
</svg>
<h1>Chim xanh trên cành</h1>
</body>
</html>
