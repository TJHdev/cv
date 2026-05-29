# Thomas Hanna — CV

A personal portfolio and CV site for Thomas Hanna, a frontend developer with 8 years of experience building responsive, user-focused web applications.

Built as a static site with [Astro](https://astro.build), styled with [Tailwind CSS](https://tailwindcss.com), and deployed to GitHub Pages.

## Features

- **About me** — profile photo and professional summary
- **Skills** — interactive cards covering TypeScript, React, Astro, Tailwind CSS, Playwright, and more
- **Experience** — work history from Deel, Chep, Enhance, Superbet, and earlier roles
- **Footer** — links to GitHub, LinkedIn, and email

## Tech stack

- [Astro](https://astro.build) — static site generation
- [Tailwind CSS](https://tailwindcss.com) — utility-first styling
- [astro-icon](https://github.com/natemoo-re/astro-icon) — SVG icon integration
- [astro-compressor](https://github.com/astro-community/astro-compressor) — asset compression at build time

## Project structure

```text
/
├── public/              # Static assets (favicon, logo)
├── src/
│   ├── components/      # Astro components (AboutMe, Skills, Experience, etc.)
│   ├── icons/           # Skill and social SVG icons
│   ├── images/          # Profile photo, background, and employer logos
│   ├── layouts/         # Page layout wrapper
│   └── pages/           # Site routes (index.astro)
├── .github/workflows/   # GitHub Pages deployment
└── package.json
```

## Development

Install dependencies and start the local dev server:

```sh
npm install
npm run dev
```

The site runs at `http://localhost:4321`.

| Command           | Action                                      |
| :---------------- | :------------------------------------------ |
| `npm run dev`     | Start the local dev server                  |
| `npm run build`   | Build the production site to `./dist/`      |
| `npm run preview` | Preview the production build locally        |

## Deployment

Pushes to the `main` branch trigger a GitHub Actions workflow that builds the site and deploys it to GitHub Pages.
