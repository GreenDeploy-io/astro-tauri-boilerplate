# Web app to run as a Website & as a Desktop App

Web app is based on [Astro](https://astro.build) (Astro for us is a framework on top of React).

- in browser, this web app runs as a website as-is
- in desktop, the web app has an extra wrapper around it to run as a desktop app
  - the wrapper we use is [Tauri](https://tauri.app)

## Features

A complete Blog feature:

- 🎈 Syntax Highlighting
- 🤖 SEO friendly with sitemap.xml and robots.txt
- ⚙️ RSS feed
- 📖 Pagination
- 🌈 Include a dark blog theme
- ⬇️ Markdown
- 📦 Image lazy loading
- 💎 Responsive design

Developer experience first:

- 🔥 Astro
- 🎨 Tailwind CSS with aspect ratio and typography plugin
- 🎉 TypeScript
- ✏️ ESLint compatible with .astro files
- 🛠 Prettier compatible with .astro files
- 🦊 Husky
- 🚫 lint-staged
- 🚨 Commitlint
- 🔧 One-click deploy on Netlify (or, manual if you prefer)

ESLint with:

- Airbnb styled guide
- TypeScript compatible
- Astro compatible
- Automatically remove unused imports
- Import sorting
- Tailwind CSS plugin

### Philosophy

- Minimal code
- SEO-friendly
- 🚀 Production-ready

### Requirements

- Node.js and npm (refer to `engines` in `package.json` for the versions ranges)
  - you can either install Node.js and npm system-wide, or use [nvm](https://github.com/nvm-sh/nvm)
- Rust; refer to [Install Rust](https://www.rust-lang.org/tools/install)
  - for MacOS, run: `brew install rust`
- If using VSCode, install recommended extensions, mentioned in `.vscode/extensions.json`

### Run locally

#### In Browser

```bash
npm run start
```

Open [http://localhost:4321](http://localhost:4321) with your favorite browser
to see your project.

#### Desktop App

```bash
npm run desktop:start
```

### Deploy to production (manual)

#### Website

You can create an optimized production build with:

```shell
npm run build
```

All generated files are located in `dist` folder.
You can deploy the folder to any hosting provider you prefer.

#### Desktop App

```shell
npm run desktop:build
```

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command           | Action                                       |
|:----------------  |:-------------------------------------------- |
| `npm run start`     | Starts local dev server at `localhost:4321`  |
| `npm run build`   | Build your production site to `./dist/`      |
| `npm run desktop:start`   | To run the desktop app locally      |
| `npm run desktop:build`   | To build the desktop app |
| `npm run preview` | Preview your build locally, before deploying |
| `npm run lint:es`    | Run ESLint and report styling errors          |
| `npm run lint:ts`    | Run TypeScript type checking |
