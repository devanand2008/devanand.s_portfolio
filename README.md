# 🚀 Devanand.S — AI/ML Developer Portfolio

<div align="center">

![Portfolio Banner](./src/assets/hero-1.jpg)

[![React](https://img.shields.io/badge/React-18.3-61DAFB?style=for-the-badge&logo=react)](https://react.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8-3178C6?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org)
[![Vite](https://img.shields.io/badge/Vite-5.4-646CFF?style=for-the-badge&logo=vite)](https://vitejs.dev)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-38BDF8?style=for-the-badge&logo=tailwindcss)](https://tailwindcss.com)
[![Framer Motion](https://img.shields.io/badge/Framer_Motion-12.x-FF0055?style=for-the-badge&logo=framer)](https://www.framer.com/motion)

**A cinematic, data-rich professional portfolio showcasing AI/ML development, full-stack projects, and creative problem solving.**

[🌐 Live Demo](#) · [📂 Source Code](#) · [📧 Contact](mailto:devanand@example.com)

</div>

---

## ✨ Features

### 🎬 Advanced Animations
| Feature | Description |
|---|---|
| **Cinematic Loading Screen** | Letter-by-letter name reveal, triple orbit rings, animated SVG progress ring, percentage counter |
| **Particle Physics Engine** | 140 multi-color particles with mouse-attract gravity, shooting stars with trails, breathing opacity |
| **Glitch Text Effect** | CSS double-layer glitch on hero name with cyan/purple flicker |
| **Magnetic Buttons** | Spring-physics magnetic hover attraction on CTA buttons |
| **Aurora Background** | Multi-layered radial gradient aurora that shifts across all sections |
| **Animated Timeline** | Scroll-triggered vertical line draw with staggered card reveals |
| **3D Tilt Cards** | Perspective-based mouse-tracking tilt with light reflection glare |
| **Typing Effect** | Multi-role typewriter with delete animation and code brackets |
| **Custom Cursor** | Spring-lagged ring + dot cursor with click scaling on desktop |
| **Scroll Progress** | Neon gradient top-bar scroll indicator |

### 📄 Sections
- **Hero** — Slideshow background, glitch name, stat counters, social links, scroll indicator
- **About** — Profile with orbit rings, personal story, education card, stats row, role cards, inspirational quote
- **Experience** — Animated vertical timeline with 7 milestones (education, projects, achievements)
- **Projects** — 8 project cards with filters, status badges, impact metrics, GitHub/Live links, detailed modal
- **Skills** — Tab-switched technical bars + tools grid with glow hover effects
- **Contact** — Two-column layout with info cards, location badge, social links + contact form
- **Footer** — 3-column footer with quick links, skills tags, availability CTA

### 🎨 Design System
- **Dark theme** with deep navy background (`hsl(230 25% 4%)`)
- **Neon color palette**: Cyan · Purple · Blue · Pink · Green · Orange
- **Glassmorphism** cards with `backdrop-filter: blur(24px)`
- **Fonts**: Orbitron (display) · Space Grotesk (heading) · Rajdhani (body) · JetBrains Mono (code)
- **Custom scrollbar** with neon cyan accent

---

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| **Framework** | React 18 + TypeScript |
| **Build Tool** | Vite 5 |
| **Styling** | Tailwind CSS 3 + Custom CSS |
| **Animations** | Framer Motion 12 |
| **Icons** | Lucide React |
| **UI Components** | Radix UI primitives |
| **Form Validation** | Zod |
| **Notifications** | Sonner |
| **Routing** | React Router DOM |

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+  
- npm or bun

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/portfolio.git
cd portfolio

# Install dependencies
npm install

# Start development server
npm run dev
```

Open [http://localhost:8080](http://localhost:8080) in your browser.

### Build for Production

```bash
npm run build
npm run preview
```

---

## 📁 Project Structure

```
src/
├── assets/                    # Images and media
│   ├── hero-1.jpg
│   ├── hero-2.jpg
│   ├── hero-3.jpg
│   └── profife image.jpeg     # Profile photo
├── components/
│   └── portfolio/
│       ├── AboutSection.tsx   # About + education + stats
│       ├── BackToTop.tsx      # Back to top button
│       ├── ContactSection.tsx # Contact form + info cards
│       ├── CustomCursor.tsx   # Neon ring cursor
│       ├── ExperienceSection.tsx  # Animated timeline (NEW)
│       ├── Footer.tsx         # 3-column footer
│       ├── HeroSection.tsx    # Cinematic hero
│       ├── LoadingScreen.tsx  # Orbit ring + letter reveal
│       ├── Navbar.tsx         # Sticky nav + active tracking
│       ├── ParticleBackground.tsx # Canvas particle physics
│       ├── ProjectsSection.tsx    # Project cards + modal
│       ├── ScrollProgress.tsx     # Progress bar
│       └── SkillsSection.tsx      # Skill bars + tools grid
├── pages/
│   ├── Index.tsx              # Main page composition
│   └── NotFound.tsx           # 404 page
├── index.css                  # Global styles + all animations
└── main.tsx                   # App entry point
```

---

## 🎯 Projects Showcased

| Project | Category | Stack | Metric |
|---|---|---|---|
| AI Job Role Predictor | AI | Python, Scikit-learn, NLP | 92% Accuracy |
| TNEA College Predictor | ML | Python, Pandas, Streamlit | 5000+ Users |
| DWLR Monitoring System | IoT | Python, Streamlit, Sensors | Real-time |
| Intern & Course Predictor | ML | Python, ML, Pandas | Smart Recs |
| Worker Management Hub | Web | Python, SQL, CRUD | Full CRUD |
| Portfolio Dashboard | Web | React, TypeScript, Framer | This Site! |
| Resume Skill Extractor | AI | Python, spaCy, NLP | 95% F1 Score |
| Data Insights Dashboard | ML | Python, Plotly, Pandas | 10+ Chart Types |

---

## 💡 Key Concepts

### Particle Physics Engine
The particle background (`ParticleBackground.tsx`) uses an HTML canvas with:
- **Mouse attraction** — particles within 160px orbit toward the cursor using vector math
- **Speed limiting** — velocity capped at 2.5px/frame to prevent runaway physics
- **Shooting stars** — randomly spawned with 16-frame trail history
- **Breathing opacity** — sine wave opacity oscillation for organic feel
- **Multi-color connections** — line color blends between two connected particles' colors

### Cinematic Loading Screen
The loader (`LoadingScreen.tsx`) provides:
- SVG circular progress ring with animated `stroke-dashoffset`
- Letter-by-letter reveal with `rotateX` 3D flip using Framer Motion stagger
- Triple concentric orbit rings at different speeds/directions
- Progress state driven by `setInterval` with progressive slowdown (fast → slow)

### Magnetic Buttons
The `MagneticBtn` component in `HeroSection.tsx` uses Framer Motion's `useMotionValue` + `useSpring` to create physical magnetic attraction that follows the cursor within the button bounds, with spring damping for smooth snap-back.

---

## 📞 Contact

**Devanand.S** — AI/ML Developer & Full Stack Engineer

- 📍 Salem, Tamil Nadu, India
- 📧 [devanand@example.com](mailto:devanand@example.com)
- 🔗 [LinkedIn](#)
- 💻 [GitHub](#)

---

<div align="center">
Built with ❤️ and neon glow by <strong>Devanand.S</strong>  
© 2026 — All rights reserved
</div>
