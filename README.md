# Swapnil Gautam — Portfolio

React + Vite + strict TypeScript + Tailwind CSS v4 + Framer Motion + Lucide React.

## Run locally

Requires Node.js 20.19+ or 22.12+.

```sh
npm ci
npm run dev
npm run build
npm run preview
```

## Architecture

- `src/App.tsx`: page composition and footer
- `src/components/`: Header, Hero, About, Projects, Experience, Contact, shared reveal/heading
- `src/data/portfolio.ts`: resume content, categorized skills, career history, typed project data
- `src/types/index.ts`: strict content interfaces
- `src/styles.css`: Tailwind import, theme tokens, component styling, responsive rules, reduced-motion support
- `public/avatar.png`: female digital portrait based on the supplied old-portfolio photo

## Customize

Update `src/data/portfolio.ts` for contact, LinkedIn, GitHub, skills, experience, projects and optional `demoUrl` / `sourceUrl`. Missing links are shown as unavailable and never navigate to fake destinations. Hero and About narrative copy is in their respective components. Edit theme tokens in `src/styles.css`. Page title and description live in `index.html`.

The attached resume supplies the content. The 2.5+ years figure and performance metrics are reproduced from that resume, not independently verified. Project previews are illustrative HTML interfaces, not original application screenshots. No university, GitHub URL, or proficiency rating was invented; DineQr uses the project URL supplied by the old portfolio.

## Contact behavior

Client-side validation requires a name, a valid email and a message of at least 10 characters. Submission opens the visitor's email application using `mailto:` and does not send automatically. For server delivery, replace the mailto action with a secured backend endpoint; never put provider secrets in browser code.

## Accessibility

Semantic sections, labelled inputs and icon actions, native modal dialogs with Escape support and focus management, visible focus rings, skip link, responsive layouts and reduced-motion support.

## Dependencies

Runtime: React, React DOM, Framer Motion, Lucide React.
Build: TypeScript, Vite, React Vite plugin, Tailwind CSS and Tailwind Vite plugin, React types.

Production output: `dist/` (static deployable assets). No server required.

## September 2026 portfolio update

- Female 3D-style avatar based on the portrait from the supplied old portfolio.
- React/TypeScript positioning in the hero and skill categories.
- Filterable React, Web Design, Photoshop, and All Work project collection.
- Original DineQr screenshot and destination plus six Photoshop artworks from https://swapnil-portfolio-5c9ca.web.app/.
- LinkedIn URL updated from the old portfolio; CV download uses the resume supplied in this conversation.
- DineQr is classified as web design because its implementation stack was not specified. React work remains grounded in the resume.
- Update `webProjects` and `designs` in `src/data/portfolio.ts` to extend the collection.
