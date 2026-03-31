# Psychology Landing Page

Official website and service overview for a private psychology practice.

Built with [Astro](https://astro.build) — outputs a fully static site with zero client-side JavaScript (except the mobile navigation toggle).

## Tech stack

- **Framework:** Astro 6
- **Styling:** Scoped CSS per component + global design tokens
- **Fonts:** Cormorant Garamond + Jost via Google Fonts
- **Images:** Astro's built-in `<Image>` component (auto-optimization, WebP output)
- **Deployment:** Vercel

## Project structure

```
landing-page/
├── public/
│   └── favicon.ico / favicon.svg
└── src/
    ├── assets/
    │   └── photos/          # Site images (jpeg)
    ├── components/
    │   ├── Navbar.astro
    │   ├── Hero.astro
    │   ├── About.astro
    │   ├── Services.astro
    │   ├── Gallery.astro
    │   ├── Testimonials.astro
    │   ├── Contact.astro
    │   └── Footer.astro
    ├── layouts/
    │   └── Layout.astro     # Global CSS tokens, reset, fonts, SEO tags
    └── pages/
        └── index.astro      # Page entry point — composes all sections
```

## Getting started

```sh
# Install dependencies
npm install

# Start local dev server at localhost:4321
npm run dev
```

## Commands

| Command            | Action                                   |
| :----------------- | :--------------------------------------- |
| `npm run dev`      | Start dev server at `localhost:4321`     |
| `npm run build`    | Build production site to `./dist/`       |
| `npm run preview`  | Preview the production build locally     |
| `npx astro sync`   | Regenerate TypeScript type declarations  |
