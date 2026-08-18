# Purav Maloo — Personal Portfolio

Live at **[personal-portfolio-theta-eosin-24.vercel.app](https://personal-portfolio-theta-eosin-24.vercel.app/)**

Cloud engineer portfolio and the canonical home for project write-ups — including [Sensitii](https://sensitii.com), whose source now lives in a private org repo. This site carries the public-facing architecture, security controls, and lessons learned for that build and others, independent of which repos still exist. Built from the [beautiful-react-tailwind-portfolio](https://github.com/machadop1407/beautiful-react-tailwind-portfolio) template.

## Features

- Featured projects (Sensitii, automation, IoT, cloud reliability)
- Blog with a **standard write-up template** on every post:
  - Overview
  - Cloud services used
  - Security controls
  - Architecture flow
  - Metrics chart
  - Screenshot slot
  - Lessons learned
- Light/dark theme, responsive layout
- Deployed on Vercel

## Local development

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
npm run preview
```

## Blog scaffolding

Posts live in `src/data/blogPosts.js`. Regenerate scaffolds with:

```bash
node scripts/generate-blog-posts.mjs
```

Add screenshots under `public/blog/` and set `screenshot.src` on each post.

## Updating project links

Featured project cards are in `src/data/projects.js`. Most `githubUrl` fields point to the [profile page](https://github.com/1Puma) rather than a specific repo, since several of the source repos behind those write-ups no longer exist or moved to a private org. Update a card's `githubUrl` if and when a project gets its own public repo again.
