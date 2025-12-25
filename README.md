# Horizon Lines - Website

Pre-launch landing page for the cruise idle game.

## Quick Start

```bash
# Install dependencies
npm install

# Run dev server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Configuration

Before deploying, update:

1. **ConvertKit Form ID** - In `src/components/EmailCapture.astro`
2. **Domain** - In `astro.config.mjs` and analytics setup
3. **Contact emails** - In `src/pages/press.astro` and `src/pages/privacy.astro`
4. **Social links** - In `src/components/Footer.astro`

## Deployment

This site is designed for Cloudflare Pages:

1. Connect your Git repository
2. Build command: `npm run build`
3. Output directory: `dist`
4. Add custom domain
5. SSL is auto-configured

## Structure

```
src/
├── layouts/
│   └── Layout.astro        # Base HTML template
├── components/
│   ├── Header.astro        # Navigation
│   ├── Hero.astro          # Main hero section
│   ├── EmailCapture.astro  # ConvertKit form
│   ├── Journey.astro       # Three phases
│   └── Footer.astro        # Footer
├── pages/
│   ├── index.astro         # Landing page
│   ├── press.astro         # Press kit
│   └── privacy.astro       # Privacy policy
└── styles/
    └── global.css          # Brand colors & typography
```

## Brand Assets Needed

- [ ] Logo (PNG, SVG)
- [ ] App icon (1024x1024)
- [ ] OG image (1200x630)
- [ ] Favicon
- [ ] Screenshots (when available)

## Analytics

Plausible Analytics is pre-configured (commented out). Uncomment in `Layout.astro` and update the domain.

