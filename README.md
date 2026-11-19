# EvanCru Studio Landing

A fast, responsive, mobile-first service landing page for **EvanCru Studio**, built with semantic HTML5, modern CSS, and `esbuild` asset bundling.

**Live Demo:** [evancru-studio-landing.netlify.app](https://evancru-studio-landing.netlify.app)

## Features

- **Mobile-First Responsive Layout:** Built using CSS Grid and Flexbox with clean breakpoints for mobile, tablet (`785px+`), and desktop (`1100px+`).
- **Performance Optimized:**
  - CSS minified and bundled via `esbuild`.
  - Optimized WebP hero graphic (`800x436`) with explicit dimensions and `fetchpriority="high"` to prevent Cumulative Layout Shift (CLS) and accelerate Largest Contentful Paint (LCP).
  - Preconnected Google Fonts (`Poppins`) with `display=swap`.
- **Accessibility & UX:**
  - WCAG AA-compliant color contrast (`#0369a1` primary accent on white text).
  - Smooth anchor scrolling gated behind `@media (prefers-reduced-motion: no-preference)` with sticky-header `scroll-margin-top` offsets.
  - Semantic HTML landmarks (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`).

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

3. Build and minify assets:
   ```bash
   npm run build
   ```

4. Open `index.html` with a local development server (such as VS Code Live Server) to preview the site.

## Deployment

This project is deployed on **Netlify** via GitHub integration:

- **Branch:** `main`
- **Build command:** `npm run build`
- **Publish directory:** `.`

## License

&copy; 2026 EvanCru Studio. All rights reserved.