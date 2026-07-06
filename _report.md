# Hendry Chou — Portfolio Website Rebuild

## 📋 Build Report

**Deliverable:** Complete portfolio rebuild with advanced animations, interactive project detail pages, and resume view.

**Source:** https://github.com/hendrychou/hendrychou.com

**Staging URL:** https://hendrychou.github.io/hendrychou.com/

**Live URL:** https://hendrychou.com/ *(pending DNS update)*

---

## 📦 What Was Built

### Design System
- **Dark theme** — Deep black canvas (`#08090a`) with warm gold accent (`#c9a96e`)
- **Typography** — Inter font family with `cv01`, `ss03` features for precision
- **Color tokens** — 5-tier background system (deep → elevated), 4-tier text system
- **GSAP-powered animations** — scroll-triggered reveals, stagger sequences, counter animations

### Interactive Features

| Feature | Details |
|---------|---------|
| **Custom cursor** | Gold dot + ring with magnetic hover on interactive elements |
| **Smooth navigation** | Client-side view routing (Home / Work / Resume / Contact) |
| **Hero section** | Animated gradient glow, floating stat badges, scroll animations |
| **Personal Values** | 4 animated cards with hover lift effects |
| **Project cards** | 7 portfolio cards with hover line-reveal and stagger animations |
| **Project detail overlays** | Full-screen detail view for each project with transitions |
| **Brand showcase** | Stagger-animated brand chips (35+ brands) |
| **Resume view** | Separate page with experience, toolkit badges, brand history |
| **Mobile responsive** | Hamburger nav, adaptive grid, touch-friendly targets |

### All 7 Portfolio Projects

1. **PINA — Digital Advisory** — Full description, tools, role, timeline
2. **PINA — Wealth Management Tools** — 60K users, 4.5★ rating
3. **Traveloka** — In-store food ordering concept (2020)
4. **BCA** — Small business performance tracking
5. **ParentStory** — Kids' activity platform
6. **IVPL** — Gaming competition platform (MVP in <1 month)
7. **Dancow NutriTods** — Early childhood development

Each has its own detail page with full description, design toolkit badges, role/timeline/company metadata.

### Animations Used
- GSAP ScrollTrigger for section reveals
- Stagger loading for project cards, value cards, brand chips
- Hero entrance sequence (tagline → title → description → buttons → social)
- Hover effects on cards, brands, social links
- Custom cursor with magnetic interaction

---

## 🚀 Deployment

The site is deployed to **GitHub Pages** at `hendrychou/hendrychou.com` with CNAME `hendrychou.com`.

### ⚠️ DNS Setup Required

Your current `hendrychou.com` DNS points to your WordPress host (`46.202.186.162`). To make the new site live:

**Option A — A Records** (recommended for apex domains):
```
hendrychou.com → 185.199.108.153
hendrychou.com → 185.199.109.153
hendrychou.com → 185.199.110.153
hendrychou.com → 185.199.111.153
```

**Option B — CNAME** (if your DNS provider supports CNAME flattening for the apex):
```
hendrychou.com → hendrychou.github.io
```

Once DNS propagates, the new site will be live at `https://hendrychou.com/` automatically with HTTPS via GitHub Pages.

### To Test in the Meantime
Visit: https://hendrychou.github.io/hendrychou.com/  
*(Note: this currently 301 redirects to hendrychou.com due to the CNAME. You may need to use curl without following redirects, or update DNS.)*

---

## 🔧 Tech Stack

| Component | Choice |
|-----------|--------|
| Frontend | Single HTML file (vanilla JS) |
| Animations | GSAP 3.12 + ScrollTrigger |
| Fonts | Inter + JetBrains Mono (Google Fonts) |
| Icons | Unicode/emoji (no icon library dependency) |
| Hosting | GitHub Pages + custom domain |
| CI/CD | GitHub Actions auto-deploy on push |

---

## 📝 Placeholders to Update

- **LinkedIn URL** → `https://www.linkedin.com/in/hendrychou` (verify)
- **Email** → `hendry@zaru.app` (verify)
- **Brand list** → Update with actual brands worked with
- **Project images** → The `image` field is empty in each project — add screenshots/case study images
- **Resume** → Add more detail to experience and education
