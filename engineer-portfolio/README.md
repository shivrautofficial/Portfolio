# Shiv Raut — Portfolio

A responsive React, TypeScript, and Vite portfolio for Shiv Raut, a first-year B.Tech Computer Science (AI/ML) student at Newton School of Technology. The site presents verified project contributions, current cybersecurity training, education, and interests in AI and robotics.

## Personalise the content

Edit **`src/data/portfolio.ts`** to update the profile, About copy, links, interests, goals, skills, projects, education, and experience.

- Replace `profile.photoUrl` with `"/profile-photo.jpg"` after adding your own image at `public/profile-photo.jpg`. Until then, the portfolio uses an initials-based placeholder.
- The résumé link points to the Google Drive URL supplied for this portfolio.
- Add achievements or certifications to their typed arrays when you have verified details. Empty arrays are intentionally not displayed.
- Project skills are labelled as contribution areas or interests; the portfolio does not assign proficiency scores.
- LifeOS links use the supplied repository and demo. ANANTA is labelled ongoing and does not link to a finished demo.

SEO title, description, favicon, and social preview are in `index.html` and `public/`. Update them if the public-facing name or content changes.

## Run locally

From the repository root:

```bash
cd engineer-portfolio
npm ci
npm run dev
```

Open the local URL printed by Vite. Verify a production build with:

```bash
npm run build
npm run preview
```

The production files are written to `dist/`.

## Deploy with Vercel

1. Import the GitHub repository into Vercel.
2. Set **Root Directory** to `engineer-portfolio` (the Vite app is in this subfolder).
3. Use the Vite preset, build command `npm run build`, output directory `dist`, and install command `npm ci`.
4. Deploy and check the page on both desktop and mobile.

`vercel.json` provides the SPA rewrite. The site has no backend, private keys, analytics, or third-party form service.

## Contact behaviour

The contact form opens the visitor's default email application with a prefilled draft to `shivrautofficial@gmail.com`. It does not send, store, or forward the message. The Copy message action is available if the visitor does not use a mail application.

## Project layout

```text
engineer-portfolio/
├── public/                 # Favicon and social preview; add profile-photo.jpg here
├── src/
│   ├── data/portfolio.ts   # Typed personal and project information
│   ├── App.tsx             # Sections, navigation, filters, and contact interaction
│   ├── main.tsx            # React entry
│   └── styles.css          # Responsive design, light theme, and motion preferences
├── index.html              # Page and social metadata
└── vercel.json             # SPA routing
```
