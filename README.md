# Gokulkrishna S — Robotics Portfolio

Personal portfolio website for Gokulkrishna S, Robotics Engineer and MSc Data Science student at the University of Surrey.

**Live site:** [gokulkrishnas.github.io](https://gokulkrishnas.github.io) *(coming soon)*

---

## Tech Stack

- **Framework:** [Astro](https://astro.build) v6
- **Styling:** Tailwind CSS + custom CSS (Apple-inspired light theme)
- **3D Scenes:** Spline (`@splinetool/runtime`) — Hero section
- **Language:** TypeScript

## Features

- Single-page scroll with smooth section navigation
- Glass morphism UI with dot-grid background
- Custom glass button system (conic-border gradient + animated shine)
- Responsive across desktop, tablet, and mobile
- Auto-populating robot image gallery — drop images into `src/assets/robots/`
- "Show More Projects" modal for non-featured projects
- Pixel art robot in Contact section

## Sections

| Section | Description |
|---|---|
| Home | Hero with Spline 3D robot scene |
| About | Bio, stats, profile photo |
| Projects | 2 featured robotics projects + modal for additional work |
| Experience | Timeline of roles at EY GDS and university |
| Skills | Robotics, ML, cloud, and data stack |
| Gallery | Auto-loaded robot photo gallery |
| Certifications | Professional certifications |
| Contact | Email, LinkedIn, GitHub links |

## Getting Started

```sh
npm install
npm run dev        # http://localhost:4321
npm run build      # Production build → ./dist/
npm run preview    # Preview production build
```

## Adding Content

**Robot gallery images** — Drop `.jpg`, `.png`, or `.webp` files into `src/assets/robots/`. They appear automatically on rebuild.

**Profile photo** — Place `profile.jpg` in the `public/` directory.

**CV** — Place `cv.pdf` in the `public/` directory for the Download CV button.

**Project links** — Update `src/components/sections/Projects.astro` to add real URLs to the `moreInfo` and `paper` fields.

## Project Structure

```
/
├── public/
│   ├── favicon.svg
│   ├── profile.jpg       ← add your photo here
│   └── cv.pdf            ← add your CV here
├── src/
│   ├── assets/
│   │   └── robots/       ← drop robot images here
│   ├── components/
│   │   ├── Navbar.astro
│   │   ├── SplineScene.astro
│   │   └── sections/
│   │       ├── Hero.astro
│   │       ├── About.astro
│   │       ├── Projects.astro
│   │       ├── Experience.astro
│   │       ├── Skills.astro
│   │       ├── RobotGallery.astro
│   │       ├── Certifications.astro
│   │       └── Contact.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
└── package.json
```
