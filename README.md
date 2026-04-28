<div align="center">
<img src="logo.png" alt="FUTURA Logo" width="1000"/>
</div>

# Tokyo: Explore the City (Community)

Interactive, pixel-art exploration demo inspired by a Figma concept.

This repository contains a small React + Vite application that renders a stylized Tokyo city scene with interactive pages, music, and pixel characters.

## Quick overview

- Stack: Vite, React (peer), TypeScript (codebase files end in .tsx/.ts), Tailwind CSS, Radix UI primitives and a small custom component set.
- Purpose: local demo and community remix of the Figma concept — ideal for experimenting with scenes, audio, and small interactions.

## Requirements

- Node.js 18+ recommended
- npm, yarn or pnpm (this project uses standard npm scripts)
- Optional: install matching peer dependencies `react` and `react-dom` if you plan to run or build the app in an environment that doesn't provide them.

## Quick start

Install dependencies and run the dev server:

```bash
npm install
npm run dev
```

Open the URL printed by Vite (usually http://localhost:5173).

Build for production:

```bash
npm run build
# optionally preview the production build
npx vite preview
```

If you use pnpm, run `pnpm install` then `npm run dev` (scripts are compatible).

## Available scripts

- `npm run dev` — start Vite dev server
- `npm run build` — build production bundle

These scripts are defined in `package.json`.

## Project structure (high level)

Important files and folders:

- `index.html` — app entry HTML
- `src/main.tsx` — application bootstrap
- `src/app` — top-level app code and routes
  - `App.tsx`, `routes.ts`
- `src/app/components` — visual components and pages (city, characters, music player, UI primitives)
- `public/music` — included audio assets
- `styles` — Tailwind and custom CSS

Explore `src/app/components` to find the interactive pages (e.g., `CityPage.tsx`, `ArcadePage.tsx`, `RamenShop.tsx`).

## Notes and tips

- Peer dependencies: `react` and `react-dom` are declared as peers in `package.json`. If you run into errors like "Cannot find module 'react'", install compatible versions (React 18.x recommended):

```bash
npm install react@18 react-dom@18
```

- If Tailwind utilities don't appear, ensure your local environment supports PostCSS/Vite and that you rebuilt after changes.
- The app expects static assets in `public/` (audio and image files). Keep large files out of the repository for faster installs.

## Troubleshooting

- "Missing React" or peer dependency warnings: install `react` and `react-dom` as shown above.
- Vite dev server doesn't start / port in use: change the port via `--port` or kill the process using the port.
- Build issues related to older Node versions: upgrade to Node 18+.

If you hit an error not covered here, open an issue with the error text and reproduction steps.

## Contributing

Contributions are welcome. Suggested small ways to help:

- Add new pixel scenes or pages under `src/app/components`.
- Improve accessibility (keyboard navigation, labels, focus states).
- Add tests or CI for builds.

Before opening a PR, confirm the dev server runs locally and the production build compiles.

## Credits & license

- This repository is a community bundle based on a Figma design (linked above). Attribution to the original designer is included in the Figma link.
- No license file is included in this repo — add a `LICENSE` if you want to set terms for reuse.

---




