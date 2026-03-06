# Firebase Auth Demo - React + TypeScript + Vite + Tailwind

<!-- MIT License -->

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

<!-- HTML & CSS -->

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)

<!-- Styling / PostCSS -->

[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/docs/)

<!-- Languages & Web Standards -->

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![ECMAScript Spec](https://img.shields.io/badge/ECMAScript-262-7A0BC0?logo=ecmascript&logoColor=white)](https://www.ecma-international.org/publications-and-standards/standards/ecma-262/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178c6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/docs/)

<!-- Infra & Runtime -->

[![Node.js](https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=white)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)

<!-- Auth & Security -->

[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)](https://firebase.google.com/docs)

<!-- Linting & Formatting -->

[![ESLint](https://img.shields.io/badge/ESLint-4B32C3?logo=eslint&logoColor=white)](https://eslint.org/docs/latest/)
[![Prettier](https://img.shields.io/badge/Prettier-2B3A42?logo=prettier&logoColor=white)](https://prettier.io/docs/)

<!-- Bundler -->

[![Vite](https://img.shields.io/badge/Vite-646cff?logo=vite&logoColor=white)](https://vite.dev/)

A minimal, production-ready demo that shows how to integrate Firebase Authentication (Google, GitHub, Microsoft, Twitter) into a React + TypeScript application scaffolded with Vite and styled with TailwindCSS. This repository is designed to be a clear reference implementation for OAuth sign-in flows and secure setup practices.

## Highlights

- Clean TypeScript + React structure with strict compiler settings ([tsconfig.json](tsconfig.json)).
- Vite for fast dev server and optimized builds ([vite.config.ts](vite.config.ts)).
- TailwindCSS utility-first styling ([tailwind.config.js](tailwind.config.js), [src/index.css](src/index.css)).
- Firebase Authentication with multiple providers configured in [src/firebase.config.ts](src/firebase.config.ts).
- Simple typed user model: [`User`](src/types/user.ts).

### Quick demo

1. Install dependencies:
   npm install
2. Start the dev server:
   npm run dev
3. Open the app: visit http://localhost:5173 (Vite default).
   Project status: stable demo for authentication flows and a good starting point for production apps.

### Why this project is useful

- Demonstrates how to wire multiple OAuth providers with Firebase Auth using a typed frontend.
- Shows a small, opinionated code layout suitable for extensions (state management, backend token exchange, session handling).
- Contains strict TypeScript settings to catch issues early ([tsconfig.json](tsconfig.json)).

### Tech Stack

- React 18 ([package.json](package.json))
- TypeScript ([tsconfig.json](tsconfig.json))
- Vite ([vite.config.ts](vite.config.ts))
- TailwindCSS ([tailwind.config.js](tailwind.config.js), [postcss.config.js](postcss.config.js))
- Firebase v12 ([src/firebase.config.ts](src/firebase.config.ts))

### How it works---> high level

- UI and sign-in buttons: [src/App.tsx](src/App.tsx)
- Firebase initialization and OAuth providers: [src/firebase.config.ts](src/firebase.config.ts)
- User shape: [`User`](src/types/user.ts)

### Security and environment

- The current repo includes a hard-coded Firebase config for demo purposes in [src/firebase.config.ts](src/firebase.config.ts). For production, move config values to environment variables and never commit secrets.
- **Recommended pattern:**
  - Use environment variables in Vite (VITE\_ prefix) and consume them in a secure build pipeline.
  - Keep server-side secrets off the client. Only public Firebase config values should be in the client.

### Recommended production improvements

- Move Firebase config to environment-backed variables.
- Add backend session management and token verification for privileged operations.
- Implement refresh-token / secure cookie handling if using server-side components.
- Add unit and integration tests around auth flows.
- Add proper error reporting and analytics (Sentry, LogRocket, etc.) if needed.

### Key files

- [src/App.tsx](src/App.tsx) - main UI, sign-in, sign-out flows.
- [src/firebase.config.ts](src/firebase.config.ts) - Firebase initialization and provider setup.
- [`User`](src/types/user.ts) - app user type definition.
- [src/main.tsx](src/main.tsx) - app bootstrap.
- [index.html](index.html) - Vite entry HTML.
- [package.json](package.json) - scripts and dependencies.
- [tailwind.config.js](tailwind.config.js), [postcss.config.js](postcss.config.js) - styling toolchain.

### Development commands

- Start dev server: `npm run dev`
- Build for production: `npm run build`
- Preview production build locally: `npm run preview`
- Lint: `npm run lint`

### Contributing

- Open issues and PRs are welcome.
- Follow existing code style and TypeScript strictness.
- Run linters before opening a PR: `npm run lint`.

### Project

```powershell
git clone https://github.com/md-abu-kayser/react-firebase-oauth-starter.git

```

### License

- This project is licensed under the terms of the **[MIT License](./LICENSE)**.
- You may replace or update the license as needed for client or proprietary projects.

---

### Contact & Maintainer

- **Name:** Md Abu Kayser - Full-Stack Engineer
- **Project:** _react-firebase-oauth-starter_
- **Maintainer:** [md-abu-kayser](https://github.com/md-abu-kayser)
- **GitHub:** [github.com/abu.kayser-official](https://github.com/md-abu-kayser)
- **Email:** [abu.kayser.official@gmail.com](mailto:abu.kayser.official@gmail.com)

If you’d like this README tailored for a specific purpose - such as **hiring managers**, **open-source contributors**, or **client deliverables** - feel free to request a custom tone or format.

---

**Thank you for reviewing this project!**

---
