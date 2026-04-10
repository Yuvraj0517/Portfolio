# 🚀 Yuvraj Doddale — Full Stack Developer Portfolio

<div align="center">

![Portfolio Banner](https://img.shields.io/badge/Portfolio-Yuvraj%20Doddale-00e5c8?style=for-the-badge&logo=code&logoColor=white)
![Version](https://img.shields.io/badge/Version-1.0.0-6c2ff5?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-f72585?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**A premium, Apple-style personal portfolio website built with pure HTML, CSS & JavaScript.**

[🌐 Live Demo](#) · [📸 Screenshots](#screenshots) · [🐛 Report Bug](#) · [✨ Request Feature](#)

</div>

---

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Sections](#sections)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Customization Guide](#customization-guide)
- [Screenshots](#screenshots)
- [License](#license)

---

## 🧑‍💻 About

This is the personal portfolio of **Yuvraj Doddale**, a BCA student at Walchand Institute of Technology, Solapur. The portfolio showcases projects, skills, certificates, and education — built as a single-file HTML application with a premium Apple-inspired dark/light design system.

> *"Building elegant digital experiences from pixel-perfect UIs to robust back-end systems."*

---

## ✨ Features

| Feature | Description |
|---|---|
| 🎨 **Apple-style Design** | Glassmorphism cards, ambient orbs, grain texture, refined color palette |
| 🌗 **Dark / Light Mode** | One-click theme toggle with smooth CSS transitions |
| ⌨️ **Typing Effect** | Animated role cycling — Full Stack Developer, Web Designer, etc. |
| 📱 **Fully Responsive** | Mobile-first layout with hamburger menu for small screens |
| 🖼️ **Lightbox Gallery** | Click-to-enlarge certificate viewer with keyboard `Esc` support |
| 🎯 **Project Filtering** | Filter by All / Web Apps / API / UI-UX |
| 📊 **Animated Skill Bars** | Intersection Observer–triggered progress bars |
| 🔄 **Scroll Reveal** | Staggered fade-in animations on scroll |
| 📬 **Contact Form** | Client-side validated form with toast notifications |
| ⬆️ **Back to Top** | Smooth-scroll floating button |
| 🏆 **Certificate Showcase** | Real certificate images embedded with hover overlay |
| 🎓 **Education Timeline** | Vertical timeline with gradient line |

---

## 📂 Sections

```
1. 🏠  Hero          — Name, role, CTA buttons, profile photo, floating stat cards
2. 👤  About         — Bio, info grid, profile image, download CV
3. 🛠️  Skills        — Animated progress bars + tech icon grid (9 technologies)
4. 📁  Projects      — 6 project cards with filter tabs and live/code links
5. 🏆  Certificates  — 6 certificate cards (2 real images + 4 placeholders)
6. 🎓  Education     — BCA at Walchand IT Solapur + SSC at Gramin Vidyalay
7. 📬  Contact       — Contact cards + message form with toast feedback
8. 🦶  Footer        — Social links, nav links, copyright
```

---

## 🧰 Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Semantic structure, single-file architecture |
| **CSS3** | Custom properties, Grid, Flexbox, animations, glassmorphism |
| **Vanilla JavaScript** | Typing effect, scroll reveal, theme toggle, lightbox, form validation |
| **Google Fonts** | `Syne` (display / headings) + `DM Sans` (body text) |
| **Font Awesome 6.5** | Icon library (fa-solid, fa-brands) |

> ⚡ **Zero dependencies** — no frameworks, no build tools, no npm. Just open and run.

---

## 📁 Project Structure

```
portfolio/
│
├── index.html          ← Entire portfolio (single file)
│
├── assets/             ← (Optional) External assets if you split them out
│   ├── images/
│   │   ├── profile.jpg
│   │   ├── about.jpg
│   │   ├── cert1.jpg   ← Cisco Networking Academy cert
│   │   ├── cert2.jpg   ← Infosys Springboard cert
│   │   └── cert3-6.jpg ← Additional certificates
│   └── resume.pdf      ← Your CV / Resume
│
└── README.md           ← This file
```

> 💡 Currently all images are embedded as **Base64** inside `index.html` for zero-dependency deployment.

---

## 🚀 Getting Started

### Prerequisites
- Any modern browser (Chrome, Firefox, Edge, Safari)
- A text editor (VS Code recommended)

### Installation

```bash
# Clone the repository
git clone https://github.com/yuvrajdoddale/portfolio.git

# Navigate into the project
cd portfolio

# Open in browser — no build step needed!
open index.html
# or on Windows:
start index.html
# or on Linux:
xdg-open index.html
```

### Using Live Server (VS Code)

1. Install the **Live Server** extension in VS Code
2. Right-click `index.html` → **Open with Live Server**
3. Auto-reloads on every save ✅

---

## 🎨 Customization Guide

### 1. Personal Information

Find and replace these placeholders in `index.html`:

```html
<!-- Hero Section -->
<h1 class="hero-name">Yuvraj Doddale</h1>

<!-- Intro text -->
BCA student at Walchand Institute of Technology, Solapur

<!-- Contact details -->
yuvraj@email.com
+91 98765 43210
github.com/yuvrajdoddale
linkedin.com/in/yuvrajdoddale
```

### 2. Color Palette

Modify CSS custom properties in `:root` to change the theme:

```css
:root {
  --accent-1: #00e5c8;   /* Teal/Cyan — primary accent */
  --accent-2: #6c2ff5;   /* Purple — secondary accent */
  --accent-3: #f72585;   /* Pink — tertiary accent */

  --bg-primary:   #05080f;  /* Main background */
  --bg-secondary: #0a0e1a;  /* Section background */
  --bg-card:      rgba(255,255,255,0.035); /* Card background */

  --text-primary:   #eef2ff; /* Headings */
  --text-secondary: #7f8ea8; /* Body text */
  --text-muted:     #445066; /* Labels */
}
```

### 3. Typing Phrases

Edit the phrases array in the `<script>` tag:

```javascript
const phrases = [
  'Full Stack Developer',
  'Web Designer',
  'UI/UX Enthusiast',
  'API Builder',
  'BCA Student',
  'Problem Solver'
];
```

### 4. Adding a Project Card

Copy and modify this template inside `.projects-grid`:

```html
<div class="project-card reveal" data-category="web">
  <div class="project-banner" style="background:linear-gradient(135deg,#0d1424,#1a2a4a)">
    <div class="project-banner-inner">🚀</div>
    <span class="project-tag" style="background:rgba(0,229,200,0.15);color:var(--accent-1);border:1px solid rgba(0,229,200,0.3)">
      Featured
    </span>
  </div>
  <div class="project-body">
    <h3 class="project-title">Your Project Name</h3>
    <p class="project-desc">Short description of what the project does.</p>
    <div class="tech-chips">
      <span class="chip">HTML</span>
      <span class="chip">CSS</span>
      <span class="chip">JavaScript</span>
    </div>
    <div class="project-links">
      <button class="proj-btn primary"><i class="fa-brands fa-github"></i> Code</button>
      <button class="proj-btn"><i class="fa-solid fa-arrow-up-right-from-square"></i> Live</button>
    </div>
  </div>
</div>
```

**`data-category` options:** `web` · `api` · `ui`

### 5. Adding a Certificate

Replace a placeholder card with a real image:

```html
<div class="cert-card reveal">
  <div class="cert-img-wrap">
    <!-- Option A: External URL -->
    <img src="assets/images/cert3.jpg" alt="Certificate Name" />

    <!-- Option B: Base64 embedded -->
    <img src="data:image/jpeg;base64,/9j/4AAQ..." alt="Certificate Name" />

    <div class="cert-overlay">
      <button class="cert-overlay-btn" onclick="openLightbox(this.closest('.cert-card').querySelector('img').src)">
        <i class="fa-solid fa-eye"></i>
      </button>
    </div>
  </div>
  <div class="cert-body">
    <div class="cert-title">Certificate Title</div>
    <div class="cert-issuer">Issuer — Month Year</div>
  </div>
</div>
```

### 6. Skill Bars

Adjust skill levels by changing `data-width` (0–100):

```html
<div class="skill-item">
  <div class="skill-header">
    <span>JavaScript</span>
    <span class="skill-pct">85%</span>
  </div>
  <div class="skill-track">
    <div class="skill-fill" data-width="85"></div>
  </div>
</div>
```

### 7. Profile Photo

Replace the Base64 image in the `<img>` tags with your own photo:

```html
<!-- Convert your photo to Base64 or use a direct path -->
<img src="assets/images/profile.jpg" alt="Your Name" />
```

---

## 🖼️ Screenshots

| Dark Mode | Light Mode |
|---|---|
| Hero Section | Hero Section |
| Projects Grid | Certificates Grid |

> *Add actual screenshots here after deployment.*

---

## 📦 Deployment

### GitHub Pages (Free)

```bash
# 1. Push to GitHub
git add .
git commit -m "Initial portfolio"
git push origin main

# 2. Go to: Repository → Settings → Pages
# 3. Source: Deploy from branch → main → / (root)
# 4. Your site is live at: https://yourusername.github.io/portfolio
```

### Netlify (Free, Drag & Drop)

1. Go to [netlify.com](https://netlify.com)
2. Drag and drop your `index.html` file (or the whole folder)
3. Get an instant live URL ✅

### Vercel (Free)

```bash
npm i -g vercel
vercel
```

---

## 📱 Responsive Breakpoints

| Breakpoint | Layout |
|---|---|
| `> 1024px` | Full desktop (3-column project grid) |
| `860px – 1024px` | 2-column project grid, 2-column cert grid |
| `600px – 860px` | Single column, hamburger menu, centered hero |
| `< 600px` | Full mobile, stacked everything, hidden scroll indicator |

---

## ⚡ Performance

- **Single file** — one HTTP request for the entire site
- **No JavaScript frameworks** — zero runtime overhead
- **CSS custom properties** — instant theme switching
- **Intersection Observer** — lazy animation triggers
- **Base64 images** — no additional image requests

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 👤 Contact

**Yuvraj Doddale**

- 📧 Email: [yuvraj@email.com](mailto:yuvraj@email.com)
- 💼 LinkedIn: [linkedin.com/in/yuvrajdoddale](https://linkedin.com/in/yuvrajdoddale)
- 🐙 GitHub: [github.com/yuvrajdoddale](https://github.com/yuvrajdoddale)
- 📍 Location: Solapur, Maharashtra, India

---

<div align="center">

Made with ❤️ and a lot of ☕ by **Yuvraj Doddale**

⭐ Star this repo if you found it helpful!

</div>
