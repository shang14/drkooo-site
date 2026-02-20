# Project: drkooo-site

## Overview

This is a personal website built using Astro and deployed on Cloudflare Pages.

Primary goals:

- Clean and minimal UI
- Fast performance
- Mobile-first responsive design
- Experiment with UI layouts safely using Git branches

---

## Stack

Framework:
- Astro

Build tool:
- Vite

Deployment:
- Cloudflare Pages

Version control:
- GitHub

---

## Key Commands

Development:

npm run dev

Build:

npm run build

Preview build:

npm run preview

Build output directory:

dist/

---

## Project Structure

Important directories:

src/layouts/
→ global layouts

src/components/
→ reusable UI components

src/pages/
→ Astro pages (routes)

public/
→ static assets

dist/
→ production build output (generated)

---

## Deployment

Cloudflare Pages deploys from:

Branch:
main → production

Other branches:
ui-* → preview deployments

dist/ directory is used as output.

Do NOT edit dist/ manually.

---

## Development Workflow

Always follow this process:

1. Create or switch to a feature branch

example:
git checkout -b ui-mobile

2. Run dev server

npm run dev

3. Make changes in src/

4. Build if needed

npm run build

5. Commit changes

git add .
git commit -m "describe change"

6. Push branch

git push

Cloudflare Pages will automatically deploy preview.

---

## UI Guidelines

Always prioritize:

- mobile-first layout
- responsive design
- clean spacing
- minimal visual clutter
- fast loading

Avoid:

- unnecessary libraries
- heavy animations
- blocking rendering

---

## Editing Rules

When modifying UI:

Prefer editing:

src/layouts/
src/components/

Avoid modifying:

dist/
node_modules/

---

## Performance Priorities

Optimize for:

- Lighthouse performance
- fast first contentful paint
- minimal JavaScript
- static rendering when possible

---

## Branch Strategy

main:
production-ready code only

ui-*:
experimental UI branches

feature-*:
new features

Never break main.

---

## Deployment Safety

Always test changes locally using:

npm run dev

before committing.

---

## Cloudflare Pages Notes

Deployment is automatic on git push.

Production URL:
https://www.drkooo.com

Preview URLs:
https://<branch>.drkooo-site.pages.dev

---

## Instructions for Claude

When editing code:

- Always preserve Astro structure
- Prefer reusable components
- Ensure mobile responsiveness
- Avoid breaking build

When unsure, ask before making destructive changes.

Prioritize clarity, performance, and maintainability.