# Edid.io — Personal Portfolio & Studio Landing Page

> **Input. Output. Impact.**  
> The official landing page for [Edid.io](https://edid-io.vercel.app) — a full-stack development studio by Edidiong Apostle

---

## Overview

A single-file, zero-dependency portfolio and studio landing page built with vanilla HTML, CSS, and JavaScript. Designed to represent **Edid.io** — a one-person development studio offering web application development, ERP/business software, payment integrations, and IT consulting across Nigeria and Africa.

---

## Features

- **Git Bash terminal hero** — animated typewriter effect with a real bash-style prompt
- **Light / Dark mode toggle** — preference saved to `localStorage`
- **Responsive design** — mobile-first, adapts cleanly across all screen sizes
- **Contact form** — wired to Formspree, sends submissions directly to email
- **Scroll animations** — fade-up transitions using IntersectionObserver
- **No frameworks, no build step** — pure HTML/CSS/JS, deploys anywhere

---

## Tech Stack

| Layer | Tech |
|---|---|
| Markup | HTML5 |
| Styling | CSS3 (custom properties, grid, flexbox) |
| Scripting | Vanilla JavaScript (ES2020+) |
| Fonts | Space Grotesk, Inter, JetBrains Mono (Google Fonts) |
| Form handling | [Formspree](https://formspree.io) |
| Hosting | [Vercel](https://vercel.com) |

---

## Project Structure

```
edid.io/
├── index.html      # Entire site — markup, styles, and scripts in one file
└── README.md       # This file
```

---

## Sections

| Section | Description |
|---|---|
| Hero | Terminal card with animated typing prompt |
| Services | Web apps, ERP, payments, landing pages, IT consulting |
| Work | Good Success College, Investment Platform, Script Marketplace |
| Stack | All technologies used across projects |
| About | Studio story, stats, and profile card |
| Contact | Formspree form + WhatsApp, Email, GitHub links |

---

## Getting Started

No build tools needed. Just open `index.html` in a browser or deploy directly.

### Local

```bash
git clone https://github.com/edidiongapostle/edid.io.git
cd edid.io
open index.html   # or just drag into a browser
```

### Deploy to Vercel

```bash
# Install Vercel CLI if you haven't
npm i -g vercel

# Deploy from the project root
vercel --prod
```

Or connect the repo to your Vercel project dashboard for automatic deployments on every `git push`.

---

## Contact Form Setup

The contact form uses [Formspree](https://formspree.io). To use your own form endpoint:

1. Sign up at [formspree.io](https://formspree.io)
2. Create a new form and copy your form ID
3. In `index.html`, find this line and replace the ID:

```js
const res = await fetch('https://formspree.io/f/YOUR_FORM_ID', {
```

---

## Customization

All colors are defined as CSS custom properties at the top of the `<style>` block:

```css
:root {
  --void: #0A0A0F;       /* Page background (dark) */
  --surface: #13131A;    /* Card backgrounds */
  --indigo: #6C63FF;     /* Primary accent */
  --white: #E8E8F0;      /* Text color */
  --muted: #7A7A8C;      /* Secondary text */
  --border: #2A2A38;     /* Borders */
  --green: #39FF8A;      /* Terminal green */
}
```

Light mode overrides are under `html.light { ... }`.

---

## Live Demo

[edid-io-edidiongs-projects-b9dcad3a.vercel.app](https://edid-io-edidiongs-projects-b9dcad3a.vercel.app)

---

## Author

**Edidiong Apostle** — Ahpo  

---

## License

MIT — free to use, fork, and modify.
