# Bolly Shampoo — Landing Page (WordPress + Elementor + Interactive 3D)

A recreation of the Bolly shampoo landing page built with **WordPress + Elementor**,
featuring a custom **interactive 3D product viewer** built with Three.js.

## 🔗 Live Demo / Screen Recording
[Add your screen recording link here — Loom / YouTube unlisted / Google Drive]

## 🛠 Tech Stack
- **WordPress** — CMS
- **Elementor** (free) — page builder for layout, header, and hero section
- **Custom HTML / CSS / JavaScript** — embedded via Elementor's HTML widget for:
  - The interactive 3D shampoo bottle
  - Header nav pill and cart/heart icons
- **Three.js (r128)** — renders the procedural 3D bottle (body, shoulder, pump,
  spout, canvas-based label texture)
- AI-assisted development (Google AI Studio was used to prototype the initial
  React/Three.js concept, which was then converted to plain HTML/CSS/JS to run
  natively inside an Elementor HTML widget, per assignment guidelines allowing
  custom HTML/CSS/JS/AI tools)

## ✨ Features
- Pixel-close recreation of the reference design: layout, typography, colors,
  spacing
- **Interactive 3D bottle**:
  - Desktop — bottle rotates by following the cursor
  - Mobile/touch — drag with a finger to rotate
  - Idle floating + subtle sway animation
- **Fully responsive** — tested down to 320px width, no horizontal scroll or
  broken layout across desktop, tablet, and mobile

## 📁 What's in this repo
```
├── bolly-elementor-widget.html   → Full HTML/CSS/JS widget (header + hero + 3D bottle)
│                                   Paste this into a single Elementor "HTML" widget
├── elementor-kit-export.zip      → Exported Elementor template/kit (Tools → Export Kit)
└── README.md                     → This file
```

## 🚀 Setup / How to Reproduce
1. Install WordPress locally (e.g. via Local by Flywheel) and activate the
   **Elementor** plugin (free version is sufficient).
2. Create a new Page → set Template to **Elementor Canvas** → Publish → Edit
   with Elementor.
3. Import `elementor-kit-export.zip` via **Elementor → Tools → Import Kit**
   (or rebuild the header/hero sections manually).
4. Add one full-width Section → one Column → drag in an **HTML** widget.
5. Paste the entire contents of `bolly-elementor-widget.html` into that widget.
6. Publish — the interactive 3D bottle and full hero section render
   immediately, no build step required.

## 📱 Responsive Breakpoints
- Desktop: full 3-column hero (headline / 3D bottle / CTA card)
- Tablet & Mobile (≤900px): columns stack, 3D bottle appears first
- 320px: verified no overflow, all text and controls remain usable

## Author
CHITRANSH SAHRAWAT
