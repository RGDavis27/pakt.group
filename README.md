# pakt — Public Marketing Site

> Make the pakt. Show up. Live it.

This repository contains the public-facing marketing website for **pakt** — the social event discovery app that matches friends through shared experiences in real life.

## 🌐 Live Site

Deployed via GitHub Pages: [https://pakt.app](https://pakt.app)

## 📁 Structure

```
pakt-website/
├── index.html              # Main landing page
├── privacy.html            # Privacy policy
├── terms.html              # Terms of service
├── 404.html                # Custom 404 page
├── CNAME                   # pakt.app domain config
├── robots.txt              # SEO crawl rules
├── sitemap.xml             # SEO sitemap
├── README.md               # This file
├── assets/
│   ├── css/
│   │   └── style.css       # Full design system
│   ├── js/
│   │   └── app.js          # Nav scroll, reveal, cursor glow, smooth scroll
│   └── images/
│       ├── favicon.svg     # SVG favicon
│       └── og-image.png    # Open Graph image (add your own 1200×630px)
└── .github/
    └── workflows/
        └── deploy.yml      # Auto-deploy to GitHub Pages on push to main
```

## 🚀 Deployment

### GitHub Pages (automatic)

1. Push to `main` — GitHub Actions deploys automatically.
2. Go to **Settings → Pages** → Source: **GitHub Actions**.
3. (Optional) Add your custom domain → **pakt.app**.

### DNS setup for pakt.app

Add these `A` records at your DNS provider:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```
Or a `CNAME` record: `www` → `yourusername.github.io`

Then enable **Enforce HTTPS** in GitHub Pages settings.

### Local development

Pure HTML/CSS/JS — no build step.

```bash
npx serve .
# or
python3 -m http.server 3000
```

## 🎨 Design System

| Token | Value | Usage |
|-------|-------|-------|
| `--ink` | `#0E0E0F` | Primary text, nav CTA, dark sections |
| `--bone` | `#F5EFE4` | Page background |
| `--cream` | `#FAF4E7` | Steps section background |
| `--paper` | `#F0E9DB` | Showcase section background |
| `--ember` | `#FF5339` | Primary accent — CTAs, highlights, stats |
| `--indigo` | `#2E2F7E` | Feature icon accent 2 |
| `--lime` | `#CAFF3C` | Feature icon accent 4 |
| `--sage` | `#7A8471` | Feature icon accent 3 |
| `--display` | Fraunces | Serif display — headlines, stats, quotes |
| `--body` | DM Sans | Body copy, UI labels |
| `--mono` | JetBrains Mono | Eyebrows, labels, footer text |

## 📄 Pages

| File | Section |
|------|---------|
| `index.html` | Hero · Problem · How it Works · Showcase · Features · Testimonials · CTA |
| `privacy.html` | Full privacy policy |
| `terms.html` | Full terms of service |
| `404.html` | Custom error page |

## 📝 Adding the OG Image

Place a `1200×630px` PNG at `/assets/images/og-image.png`. Referenced in `<meta property="og:image">`.

## 🔗 Related Repos

- `pakt-app` — React Native / Expo mobile app
- `pakt-backend` — Node.js / Express / PostgreSQL API

---

© 2026 pakt, Inc. — Make the pakt. Show up. Live it.
