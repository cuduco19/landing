# EvanCru Studio — Service Landing Page

A fast, responsive, and accessible service landing page built with semantic HTML5, modern mobile-first CSS, and bundled/minified with **esbuild**.

## Live Demo

- **Production URL:** `https://your-site-name.netlify.app` *(replace with your live Netlify link)*

## Features

- **Mobile-First Responsive Design:** Adapts cleanly across phones, tablets, and desktop viewports using CSS Grid and Flexbox.
- **High Performance & Optimization:**
  - Minified and bundled CSS via `esbuild` (`dist/styles/main.min.css`).
  - Properly sized `.webp` hero graphic (`800x436`) with `fetchpriority="high"` and explicit dimensions to prevent Cumulative Layout Shift (CLS).
  - Preconnected Google Fonts (`Poppins`) with `display=swap` for non-blocking typography.
- **Accessibility-Focused:**
  - WCAG AA compliant color contrast (`#0369a1` accent on white text).
  - Semantic HTML landmarks (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`).
  - Smooth anchor scrolling wrapped in `@media (prefers-reduced-motion: no-preference)` with sticky-header `scroll-margin-top` offsets.

## Project Structure

```text
landing/
├── assets/
│   ├── icons/
│   │   └── favicon.svg
│   └── images/
│       └── gospel-with-legs.webp
├── dist/
│   └── styles/
│       └── main.min.css
├── styles/
│   └── main.css
├── index.html
├── package.json
└── README.md
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher recommended)

### Installation & Build

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/landing.git
   cd landing
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Build and minify the stylesheet:
   ```bash
   npm run build
   ```

4. Open `index.html` in your browser (or use a local dev server such as VS Code Live Server).

## Deployment

This project is configured for continuous deployment via **GitHub + Netlify**:

- **Build command:** `npm run build`
- **Publish directory:** `.`

## License

&copy; 2026 EvanCru Studio. All rights reserved.