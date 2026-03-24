# Vite + React + TypeScript Template Updated for 2026

This starter combines React, TypeScript, Vite, Vitest, ESLint, and Prettier in a setup intended for Northwestern CS394 projects and similar coursework. The template now targets the 2026 major-version baseline verified in this repository on March 24, 2026.

## Toolchain Baseline

- Node.js `22+` recommended
- npm `10+`
- React `19.2.x`
- TypeScript `5.9.x`
- ESLint `9.39.x`
- Vite `8.0.x`
- Vitest `4.1.x`

## Installation

Clone the repo and install dependencies:

```bash
npm install
```

If you use `nvm`, run:

```bash
nvm use
```

To create a fresh copy from GitHub:

```bash
npx degit toddwseattle/pretty-vitest-react-ts-template project-name
```

## Scripts

- `npm run dev` starts the Vite dev server.
- `npm run build` runs TypeScript and creates a production build.
- `npm run type-check` runs the TypeScript compiler without emitting files.
- `npm run lint` runs Prettier and ESLint across the repo.
- `npm test` runs Vitest without the browser UI.
- `npm test -- --run` runs the Vitest suite once without watch mode.
- `npm run test:ui` starts the Vitest UI.
  - The UI server is pinned to `127.0.0.1:51204`.

## VS Code Setup

For the smoothest editing experience:

1. Install the ESLint extension.
2. Install the Prettier extension.
3. Enable `formatOnSave`.
4. Open a `.tsx` file and confirm both ESLint and Prettier are active in the editor.

## Pre-commit Hook

The repo includes Husky setup and keeps the historical `pre-commit` lint flow in `package.json`. Running `npm run lint` before committing is still the safest way to ensure formatting and lint fixes are already applied.

## Upgrade Notes

The detailed 2026 upgrade record, including verification results and package decisions, is in [docs/upgrade-2026.md](/Users/toddwseattle/dev/cs394-template/docs/upgrade-2026.md).

## Acknowledgments

This template builds on earlier starter work from [theSwordBreaker](https://github.com/TheSwordBreaker/vite-reactts-eslint-prettier) and the React/Vitest teaching materials used in Northwestern CS394.
