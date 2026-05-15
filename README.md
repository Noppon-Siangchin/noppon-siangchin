# Noppon Siangchin — Digital Business Card

A personal landing page and digital business card built as a static site, designed to be shared via QR code.

🔗 **Live site:** https://noppon-siangchin.github.io/noppon-siangchin/

## About

This is the personal digital calling card for **Noppon "Sun" Siangchin**, Senior Data Analyst at Senestia Company Limited. Built as a static HTML/CSS/JS site, it serves as the destination for QR codes printed on physical business cards.

## Features

- 📇 **Hero section** with business card display
- 💾 **Save Contact** button — downloads a vCard (.vcf) file with all contact details
- 🎨 **Editorial design** with custom typography (Fraunces, Inter Tight, JetBrains Mono)
- 📱 **Fully responsive** — works on mobile, tablet, and desktop
- 🔒 **HTTPS by default** via GitHub Pages
- ⚡ **Fast loading** — single HTML file, optimized assets

## Stack

- Pure HTML / CSS / JavaScript (no frameworks)
- Google Fonts (Fraunces, Inter Tight, JetBrains Mono)
- No build process required — just static files

## Structure

```
.
├── index.html          # Main landing page
├── business-card.png   # Hero image of the physical business card
├── qr-generator.html   # In-browser QR code generator tool (bonus)
├── README.md           # This file
├── CLAUDE.md           # Instructions for Claude Code
├── DEPLOYMENT.md       # Step-by-step deployment guide
├── LICENSE             # MIT License
└── .gitignore
```

## Local Development

Just open `index.html` directly in any browser. No build step, no dependencies.

```bash
# Optional: serve locally with Python
python3 -m http.server 8000
# Then visit http://localhost:8000
```

## Deployment

See [DEPLOYMENT.md](./DEPLOYMENT.md) for full deployment instructions to GitHub Pages.

## Contact

- 📧 noppon [at] senestia [dot] com
- 💼 [LinkedIn](https://linkedin.com/in/noppon-siangchin)
- 🏢 Senestia Company Limited

## License

MIT License — feel free to use this as inspiration for your own digital business card. See [LICENSE](./LICENSE).
