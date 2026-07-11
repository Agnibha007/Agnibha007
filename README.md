<div align="center">

<!-- ─── HERO: Animated SVG with gradient text, glowing orb, pulse rings ─── -->
<svg width="100%" height="240" viewBox="0 0 800 240" fill="none" xmlns="http://www.w3.org/2000/svg" style="max-width:800px;">
  <defs>
    <linearGradient id="heroGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#ffffff">
        <animate attributeName="stop-color" values="#ffffff;#888888;#ffffff" dur="4s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="#555555">
        <animate attributeName="stop-color" values="#555555;#ffffff;#555555" dur="4s" repeatCount="indefinite" />
      </stop>
    </linearGradient>
    <radialGradient id="glowGrad" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.08)" />
      <stop offset="100%" stop-color="rgba(255,255,255,0)" />
    </radialGradient>
    <radialGradient id="glowPulse" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.06)" />
      <stop offset="50%" stop-color="rgba(255,255,255,0.02)" />
      <stop offset="100%" stop-color="rgba(255,255,255,0)" />
    </radialGradient>

  </defs>

  <!-- Ambient glow orbs -->
  <circle cx="200" cy="120" r="180" fill="url(#glowPulse)">
    <animate attributeName="r" values="140;200;140" dur="6s" repeatCount="indefinite" />
    <animate attributeName="opacity" values="0.5;1;0.5" dur="6s" repeatCount="indefinite" />
  </circle>
  <circle cx="600" cy="100" r="160" fill="url(#glowPulse)">
    <animate attributeName="r" values="160;120;160" dur="5s" repeatCount="indefinite" />
    <animate attributeName="opacity" values="0.3;0.8;0.3" dur="5s" repeatCount="indefinite" />
  </circle>

  <!-- Pulse rings -->
  <circle cx="400" cy="130" r="60" fill="none" stroke="rgba(255,255,255,0.04)" stroke-width="1">
    <animate attributeName="r" values="40;200;40" dur="8s" repeatCount="indefinite" />
    <animate attributeName="opacity" values="1;0;1" dur="8s" repeatCount="indefinite" />
  </circle>
  <circle cx="400" cy="130" r="60" fill="none" stroke="rgba(255,255,255,0.03)" stroke-width="0.5">
    <animate attributeName="r" values="40;200;40" dur="8s" begin="2s" repeatCount="indefinite" />
    <animate attributeName="opacity" values="1;0;1" dur="8s" begin="2s" repeatCount="indefinite" />
  </circle>
  <circle cx="400" cy="130" r="60" fill="none" stroke="rgba(255,255,255,0.02)" stroke-width="0.3">
    <animate attributeName="r" values="40;200;40" dur="8s" begin="4s" repeatCount="indefinite" />
    <animate attributeName="opacity" values="1;0;1" dur="8s" begin="4s" repeatCount="indefinite" />
  </circle>

  <!-- Grid lines -->
  <g opacity="0.03">
    <line x1="0" y1="40" x2="800" y2="40" stroke="white" stroke-width="0.5" />
    <line x1="0" y1="80" x2="800" y2="80" stroke="white" stroke-width="0.5" />
    <line x1="0" y1="120" x2="800" y2="120" stroke="white" stroke-width="0.5" />
    <line x1="0" y1="160" x2="800" y2="160" stroke="white" stroke-width="0.5" />
    <line x1="0" y1="200" x2="800" y2="200" stroke="white" stroke-width="0.5" />
  </g>

  <!-- Title -->
  <text x="400" y="80" text-anchor="middle" font-family="system-ui,-apple-system,sans-serif" font-size="52" font-weight="700" letter-spacing="-1" fill="url(#heroGrad)">Building products</text>
  <text x="400" y="130" text-anchor="middle" font-family="system-ui,-apple-system,sans-serif" font-size="52" font-weight="700" letter-spacing="-1" fill="url(#heroGrad)" opacity="0.7">people actually use.</text>

  <!-- Subtitle -->
  <text x="400" y="175" text-anchor="middle" font-family="system-ui,-apple-system,sans-serif" font-size="16" fill="#555555">
    Agnibha Mukherjee · Product Engineering
    <animate attributeName="opacity" values="0.4;1;0.4" dur="3s" repeatCount="indefinite" />
  </text>

  <!-- Divider line -->
  <line x1="250" y1="205" x2="550" y2="205" stroke="rgba(255,255,255,0.06)" stroke-width="1">
    <animate attributeName="x1" values="350;250;350" dur="6s" repeatCount="indefinite" />
    <animate attributeName="x2" values="450;550;450" dur="6s" repeatCount="indefinite" />
  </line>
</svg>

<br>

</div>

<!-- ─── ANIMATED SVG TERMINAL ─── -->
<svg width="100%" height="260" viewBox="0 0 700 260" fill="none" xmlns="http://www.w3.org/2000/svg" style="max-width:700px;display:block;margin:0 auto;">
  <defs>
    <style>
      @keyframes blink { 0%,100% { opacity:1; } 50% { opacity:0; } }
      @keyframes slideIn { from { opacity:0; transform:translateY(8px); } to { opacity:0.7; transform:translateY(0); } }
      @keyframes fadeLine { 0% { opacity:0; } 30% { opacity:0; } 100% { opacity:0.7; } }
      .cursor { animation:blink 1s step-end infinite; }
      .l1 { animation:fadeLine 0.3s ease-out forwards; }
      .l2 { animation:fadeLine 0.3s 0.3s ease-out forwards; opacity:0; }
      .l3 { animation:fadeLine 0.3s 0.6s ease-out forwards; opacity:0; }
      .l4 { animation:fadeLine 0.3s 0.9s ease-out forwards; opacity:0; }
      .l5 { animation:fadeLine 0.3s 1.2s ease-out forwards; opacity:0; }
      .l6 { animation:fadeLine 0.3s 1.5s ease-out forwards; opacity:0; }
    </style>
  </defs>

  <!-- Terminal window -->
  <rect x="20" y="20" width="660" height="230" rx="12" fill="#0d0d0d" stroke="rgba(255,255,255,0.06)" stroke-width="1" />
  <!-- Title bar dots -->
  <circle cx="50" cy="48" r="6" fill="rgba(255,255,255,0.08)" />
  <circle cx="70" cy="48" r="6" fill="rgba(255,255,255,0.08)" />
  <circle cx="90" cy="48" r="6" fill="rgba(255,255,255,0.08)" />

  <!-- Lines -->
  <text x="50" y="90" font-family="monospace" font-size="14" fill="#22c55e" class="l1">$ whoami</text>
  <text x="50" y="115" font-family="monospace" font-size="14" fill="#888888" class="l2">→ Agnibha Mukherjee</text>

  <text x="50" y="145" font-family="monospace" font-size="14" fill="#22c55e" class="l3">$ craft</text>
  <text x="50" y="170" font-family="monospace" font-size="14" fill="#888888" class="l4">→ Software products people remember</text>

  <text x="50" y="200" font-family="monospace" font-size="14" fill="#22c55e" class="l5">$ building</text>
  <text x="50" y="225" font-family="monospace" font-size="14" fill="#888888" class="l6">→ Strumm — AI-powered music intelligence</text>

  <!-- Blinking cursor -->
  <rect x="680" y="215" width="8" height="16" rx="1" fill="#ffffff" class="cursor" />
</svg>

<br>
<br>

<div align="center">

## Currently Building — Strumm

</div>

<!-- ─── ANIMATED STRUMM SHOWCASE ─── -->
<svg width="100%" height="180" viewBox="0 0 700 180" fill="none" xmlns="http://www.w3.org/2000/svg" style="max-width:700px;display:block;margin:0 auto;">
  <defs>
    <linearGradient id="strummBorder" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.08)" />
      <stop offset="50%" stop-color="rgba(255,255,255,0.02)" />
      <stop offset="100%" stop-color="rgba(255,255,255,0.08)" />
    </linearGradient>
    <linearGradient id="barGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#ffffff" />
      <stop offset="100%" stop-color="#444444" />
    </linearGradient>
  </defs>
  <rect x="20" y="10" width="660" height="160" rx="12" fill="#111111" stroke="url(#strummBorder)" stroke-width="1" />
  <rect x="45" y="35" width="200" height="4" rx="2" fill="url(#barGrad)" opacity="0.8">
    <animate attributeName="width" values="0;200;200" dur="2s" fill="freeze" />
  </rect>
  <text x="45" y="65" font-family="system-ui,sans-serif" font-size="14" fill="#888888">Replay your listening history. Visualize your sound DNA.</text>
  <rect x="45" y="85" width="160" height="3" rx="1.5" fill="rgba(255,255,255,0.06)">
    <animate attributeName="width" values="0;160;160" dur="1.5s" begin="0.5s" fill="freeze" />
  </rect>
  <text x="45" y="115" font-family="monospace" font-size="12" fill="#22c55e">Live Demo</text>
  <text x="45" y="135" font-family="monospace" font-size="12" fill="#555555">strumm.me ←</text>
  <text x="260" y="115" font-family="monospace" font-size="12" fill="#22c55e">Stack</text>
  <text x="260" y="135" font-family="monospace" font-size="12" fill="#555555">React · Node.js · MongoDB · PWA</text>
  <rect x="540" y="105" width="120" height="32" rx="16" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.08)" stroke-width="1">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="3s" repeatCount="indefinite" />
  </rect>
  <text x="600" y="126" text-anchor="middle" font-family="system-ui,sans-serif" font-size="12" fill="#888888">Featured Project</text>
</svg>

<br>

> A full-featured music platform — Progressive Web App with AI-driven recommendations, offline support, and a listening experience that respects your attention. Analyzes patterns, profiles sound DNA using collaborative filtering, and surfaces recommendations that feel intentional.

<br>

<div align="center">

## Selected Work

</div>

| Project | Stack | What it does |
|---------|-------|-------------|
| **Talkfusion** | Socket.io, Node.js | Real-time messaging with room-based chat |
| **Shortify** | Next.js, MongoDB | URL shortener with click analytics |
| **AI AQI Assistant** | Python, Flask, ML | Air quality prediction with ML insights |
| **MoneyMate** | React, Chart.js | Interactive expense tracking with analytics |
| **Typester** | React, JavaScript | Real-time WPM typing speed benchmark |
| **Uncrackable** | JavaScript, HTML/CSS | Password management with local storage |

<br>

<div align="center">

## Engineering Philosophy

</div>

<br>

**Write code for humans first.** Machines interpret anything — but the next engineer reading your code at 2 AM needs clarity. I optimize for maintainability over cleverness.

**Ship before it's perfect.** Perfect is a moving target. I build a solid foundation, launch, then iterate based on real usage. Users don't care about your roadmap — they see what you ship.

**Every pixel has a purpose.** Whether it's the spacing between two buttons or the timing of a hover transition, nothing in the UI should feel accidental. Detail is not detail. It *is* the design.

**Choose simple over easy.** Simple requires discipline. Fewer dependencies, cleaner abstractions, systems that don't break when you look at them wrong.

**The best code is deleted code.** Every feature, every dependency comes with a cost. I ship less code than most — and what remains works harder.

<br>

<div align="center">

## Technologies

</div>

<!-- ─── ANIMATED TECH BARS ─── -->
<svg width="100%" height="280" viewBox="0 0 700 280" fill="none" xmlns="http://www.w3.org/2000/svg" style="max-width:700px;display:block;margin:0 auto;">
  <defs>
    <linearGradient id="fb" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.3)" />
      <stop offset="100%" stop-color="rgba(255,255,255,0.06)" />
    </linearGradient>
    <linearGradient id="be" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.25)" />
      <stop offset="100%" stop-color="rgba(255,255,255,0.06)" />
    </linearGradient>
    <linearGradient id="db" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.2)" />
      <stop offset="100%" stop-color="rgba(255,255,255,0.06)" />
    </linearGradient>
    <linearGradient id="cl" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.18)" />
      <stop offset="100%" stop-color="rgba(255,255,255,0.06)" />
    </linearGradient>
    <linearGradient id="tl" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.22)" />
      <stop offset="100%" stop-color="rgba(255,255,255,0.06)" />
    </linearGradient>
    <linearGradient id="ai" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.16)" />
      <stop offset="100%" stop-color="rgba(255,255,255,0.06)" />
    </linearGradient>
  </defs>

  <rect x="20" y="20" width="660" height="240" rx="12" fill="#0d0d0d" stroke="rgba(255,255,255,0.04)" stroke-width="1" />

  <!-- Frontend -->
  <text x="45" y="55" font-family="monospace" font-size="11" fill="#555555">FRONTEND</text>
  <rect x="45" y="68" height="6" rx="3" fill="rgba(255,255,255,0.04)" width="610" />
  <rect x="45" y="68" height="6" rx="3" fill="url(#fb)" width="610">
    <animate attributeName="width" values="0;610;610" dur="1.5s" fill="freeze" />
  </rect>
  <text x="660" y="73" text-anchor="end" font-family="monospace" font-size="10" fill="#444444">React · Next.js · TS · CSS · GSAP · Three</text>

  <!-- Backend -->
  <text x="45" y="100" font-family="monospace" font-size="11" fill="#555555">BACKEND</text>
  <rect x="45" y="113" height="6" rx="3" fill="rgba(255,255,255,0.04)" width="610" />
  <rect x="45" y="113" height="6" rx="3" fill="url(#be)" width="520">
    <animate attributeName="width" values="0;520;520" dur="1.5s" begin="0.2s" fill="freeze" />
  </rect>
  <text x="660" y="118" text-anchor="end" font-family="monospace" font-size="10" fill="#444444">Node.js · Python · Express · Socket.io</text>

  <!-- Databases -->
  <text x="45" y="145" font-family="monospace" font-size="11" fill="#555555">DATABASES</text>
  <rect x="45" y="158" height="6" rx="3" fill="rgba(255,255,255,0.04)" width="610" />
  <rect x="45" y="158" height="6" rx="3" fill="url(#db)" width="380">
    <animate attributeName="width" values="0;380;380" dur="1.5s" begin="0.4s" fill="freeze" />
  </rect>
  <text x="660" y="163" text-anchor="end" font-family="monospace" font-size="10" fill="#444444">MongoDB · PostgreSQL · Redis</text>

  <!-- Cloud -->
  <text x="45" y="190" font-family="monospace" font-size="11" fill="#555555">CLOUD</text>
  <rect x="45" y="203" height="6" rx="3" fill="rgba(255,255,255,0.04)" width="610" />
  <rect x="45" y="203" height="6" rx="3" fill="url(#cl)" width="450">
    <animate attributeName="width" values="0;450;450" dur="1.5s" begin="0.6s" fill="freeze" />
  </rect>
  <text x="660" y="208" text-anchor="end" font-family="monospace" font-size="10" fill="#444444">Vercel · Netlify · Docker · Linux</text>

  <!-- Tools -->
  <text x="45" y="235" font-family="monospace" font-size="11" fill="#555555">TOOLS</text>
  <rect x="45" y="248" height="6" rx="3" fill="rgba(255,255,255,0.04)" width="610" />
  <rect x="45" y="248" height="6" rx="3" fill="url(#tl)" width="320">
    <animate attributeName="width" values="0;320;320" dur="1.5s" begin="0.8s" fill="freeze" />
  </rect>
  <text x="660" y="253" text-anchor="end" font-family="monospace" font-size="10" fill="#444444">Git · Figma · Linear · VS Code</text>
</svg>

<br>

<div align="center">

## Development Environment

</div>

| | |
|---|---|
| **OS** | macOS / Linux |
| **Editor** | VS Code — Mona Sans, minimal UI |
| **Terminal** | Warp / iTerm2 — fish shell |
| **Browser** | Arc — tabs that don't take over your life |
| **Font** | Mona Sans — built for code, beautiful at every weight |
| **Shell** | fish — autosuggestions, sane defaults |
| **Package Manager** | npm / pnpm |

<br>

<div align="center">

## Experience

</div>

```
2018 · Foundation with Java & DSA
  →  Object-oriented programming, algorithms, disciplined coding habits

2020 · Frontend Development
  →  HTML, CSS, JavaScript — responsive layouts, DOM, interactions

2022 · Full-Stack & Backend
  →  React, Next.js, Node.js, Python — production apps, APIs, deployment
```

<br>

<div align="center">

## Roadmap

</div>

<!-- ─── ANIMATED ROADMAP TIMELINE ─── -->
<svg width="100%" height="280" viewBox="0 0 700 280" fill="none" xmlns="http://www.w3.org/2000/svg" style="max-width:700px;display:block;margin:0 auto;">
  <defs>
    <style>
      @keyframes pulseDot { 0%,100% { opacity:0.6; } 50% { opacity:1; } }
    </style>
  </defs>

  <!-- Timeline line -->
  <line x1="100" y1="30" x2="100" y2="260" stroke="rgba(255,255,255,0.08)" stroke-width="1" stroke-dasharray="4 4" />

  <g>
    <!-- Completed -->
    <text x="120" y="50" font-family="monospace" font-size="12" fill="#22c55e" opacity="0.8">●</text>
    <text x="140" y="50" font-family="system-ui,sans-serif" font-size="14" fill="#888888">AI AQI Platform</text>
    <text x="140" y="68" font-family="system-ui,sans-serif" font-size="11" fill="#555555">Air quality prediction with machine learning</text>
  </g>

  <g>
    <text x="120" y="98" font-family="monospace" font-size="12" fill="#22c55e" opacity="0.8">●</text>
    <text x="140" y="98" font-family="system-ui,sans-serif" font-size="14" fill="#888888">Shortify</text>
    <text x="140" y="116" font-family="system-ui,sans-serif" font-size="11" fill="#555555">URL shortener with real-time click analytics</text>
  </g>

  <g>
    <text x="120" y="146" font-family="monospace" font-size="12" fill="#22c55e" opacity="0.8">●</text>
    <text x="140" y="146" font-family="system-ui,sans-serif" font-size="14" fill="#888888">MoneyMate · Typester · Talkfusion</text>
    <text x="140" y="164" font-family="system-ui,sans-serif" font-size="11" fill="#555555">Expense tracking, typing benchmark, real-time chat</text>
  </g>

  <!-- Current -->
  <g>
    <circle cx="118" cy="196" r="6" fill="none" stroke="#ffffff" stroke-width="2" opacity="0.6">
      <animate attributeName="opacity" values="0.6;1;0.6" dur="2s" repeatCount="indefinite" />
    </circle>
    <text x="140" y="200" font-family="system-ui,sans-serif" font-size="14" fill="#ffffff">Strumm</text>
    <text x="140" y="218" font-family="system-ui,sans-serif" font-size="11" fill="#555555">Music intelligence · Sound DNA Engine · Portfolio v2</text>
  </g>

  <!-- Upcoming -->
  <g>
    <text x="120" y="252" font-family="monospace" font-size="12" fill="rgba(255,255,255,0.15)">○</text>
    <text x="140" y="252" font-family="system-ui,sans-serif" font-size="14" fill="rgba(255,255,255,0.2)">Android · Desktop · AI Radio · Open API</text>
  </g>
</svg>

<br>

<div align="center">

## GitHub Presence

</div>

> **116 public repositories** — forks, experiments, tools, and products.
> Every repo tells a story. Some are well-told. Some are lessons learned.

<!-- ─── ANIMATED PULSING STATS ─── -->
<svg width="100%" height="100" viewBox="0 0 700 100" fill="none" xmlns="http://www.w3.org/2000/svg" style="max-width:700px;display:block;margin:0 auto;">
  <defs>
    <linearGradient id="statGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="rgba(255,255,255,0.04)" />
      <stop offset="50%" stop-color="rgba(255,255,255,0.06)" />
      <stop offset="100%" stop-color="rgba(255,255,255,0.04)" />
    </linearGradient>
  </defs>

  <rect x="20" y="10" width="200" height="80" rx="10" fill="url(#statGrad)" stroke="rgba(255,255,255,0.04)" stroke-width="1" />
  <text x="120" y="45" text-anchor="middle" font-family="monospace" font-size="24" fill="#ffffff" opacity="0.8">116</text>
  <text x="120" y="68" text-anchor="middle" font-family="system-ui,sans-serif" font-size="11" fill="#555555">Public Repositories</text>

  <rect x="250" y="10" width="200" height="80" rx="10" fill="url(#statGrad)" stroke="rgba(255,255,255,0.04)" stroke-width="1" />
  <text x="350" y="45" text-anchor="middle" font-family="monospace" font-size="24" fill="#ffffff" opacity="0.8">2018</text>
  <text x="350" y="68" text-anchor="middle" font-family="system-ui,sans-serif" font-size="11" fill="#555555">Years Active</text>

  <rect x="480" y="10" width="200" height="80" rx="10" fill="url(#statGrad)" stroke="rgba(255,255,255,0.04)" stroke-width="1" />
  <text x="580" y="45" text-anchor="middle" font-family="monospace" font-size="24" fill="#ffffff" opacity="0.8">8</text>
  <text x="580" y="68" text-anchor="middle" font-family="system-ui,sans-serif" font-size="11" fill="#555555">Products Shipped</text>
</svg>

<br>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com/?user=Agnibha007&theme=dark&hide_border=true&background=0a0a0a&stroke=ffffff15&ring=ffffff40&fire=ffffff80&currStreakNum=ffffff80&sideNums=ffffff50&sideLabels=ffffff30&dates=ffffff20)](https://git.io/streak-stats)

<br>

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Agnibha007&show_icons=true&count_private=true&hide_border=true&bg_color=0a0a0a&text_color=ffffff60&icon_color=ffffff30&title_color=ffffff90)](https://github.com/anuraghazra/github-readme-stats)

---

<br>

## Let's build something worth remembering.

If you have a project, an idea, or just want to talk about software — I read every message.

<!-- ─── ANIMATED CONTACT DIVIDER ─── -->
<svg width="100%" height="30" viewBox="0 0 400 30" fill="none" xmlns="http://www.w3.org/2000/svg" style="max-width:400px;display:block;margin:0 auto;">
  <rect x="50" y="14" width="300" height="1" rx="0.5" fill="rgba(255,255,255,0.06)" />
  <circle cx="200" cy="14" r="4" fill="rgba(255,255,255,0.08)">
    <animate attributeName="r" values="2;5;2" dur="3s" repeatCount="indefinite" />
    <animate attributeName="opacity" values="0.3;0.8;0.3" dur="3s" repeatCount="indefinite" />
  </circle>
</svg>

<br>

[agnibha.me](https://agnibha.me) · [strumm.me](https://strumm.me) · [blog.agnibha.me](https://blog.agnibha.me)

<br>

<sub>— Agnibha Mukherjee · Kolkata, India —</sub>

</div>
