# drkooo-site

Personal portfolio site for `dr.KOoo`, built with Astro.

## Tech Stack

- Astro 5
- Tailwind CSS 4
- Optional Vue integration (installed, currently not used by page components)
- Multilingual UI (中文 / English / 日本語)

## Local Development

Run all commands in project root:

| Command         | Description                                   |
| :-------------- | :-------------------------------------------- |
| `npm install`   | Install dependencies                          |
| `npm run dev`   | Start dev server (`http://localhost:4321`)    |
| `npm run build` | Build production output to `dist/`            |
| `npm run preview` | Preview production build locally            |

## Project Structure

```text
.
├── public/
│   └── images/
├── src/
│   ├── components/
│   │   ├── Navigation.astro
│   │   ├── Hero.astro
│   │   ├── About.astro
│   │   ├── Projects.astro
│   │   ├── Skills.astro
│   │   ├── Experience.astro
│   │   ├── Contact.astro
│   │   └── Footer.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
└── astro.config.mjs
```

## Behavior Notes

- Navbar uses sticky positioning and stays pinned at top while scrolling.
- Page uses normal document scrolling (window scroll), not an internal fixed scroll container.
- Global theme and language state are handled in `Layout.astro`.
- If style or script updates appear stale, hard refresh browser with `Cmd + Shift + R`.

## Content Sections

The homepage (`src/pages/index.astro`) renders sections in this order:

1. Navigation
2. Hero
3. About
4. Projects
5. Skills
6. Experience
7. Contact
8. Footer
