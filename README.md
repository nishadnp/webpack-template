# webpack-template

<div align="center">
<img width="200" height="200" alt="Webpack Logo" src="https://webpack.js.org/assets/icon-square-big.svg">
</div>

<br>

A minimal, reusable JavaScript project template powered by Webpack. Includes development setup with CSS, HTML, image support, and code quality tooling.

## Features

- Webpack 5 configuration for development

- Dev server with live reload

- Base CSS with light reset (box-sizing, margin reset, line-height)

- CSS and style support (`style-loader` + `css-loader`)

- HTML template handling (`html-webpack-plugin` + `html-loader`)

- Image assets support (`png`, `jpg`, `svg`, `gif`)

- Clean, minimal structure for quick project starts

- ESLint + Prettier for code quality and formatting

- Husky + lint-staged to enforce linting/formatting before commits (scoped to `src/`)

## Folder Structure

```bash
webpack-template/
├── eslint.config.mjs
├── .gitignore
├── .husky/
│   ├── _
│   └── pre-commit
├── package.json
├── package-lock.json
├── .prettierignore
├── .prettierrc
├── README.md
├── src/
│   ├── index.html
│   ├── index.js
│   └── style.css
└── webpack.config.js
```

## Requirements

Node.js 18+ recommended

## Usage

**1. Clone the template**

    git clone <repo-clone-url> project-name
    cd project-name

**2. Install dependencies**

    npm install

**3. Start development server**

    npm run dev

- **Opens a local server** with live reload

- **Entry point:** src/index.js

- **HTML template:** src/index.html

- **Base styles:** src/style.css

**4. Build**

    npm run build

**5. Clean build output**

    npm run clean

- Removes the `dist/` directory before a fresh build

## Code Quality

This template includes **ESLint, Prettier, Husky, and lint-staged** to enforce consistent code style.

Pre-commit hooks automatically lint and format **only files inside `src/`**, intentionally leaving configuration files and tooling untouched.

## Notes

- This template uses a single Webpack configuration in development mode.

- Production-specific optimizations (separate configs, webpack-merge, deployment scripts) are intentionally left out and can be added per project as needed.

<br>

---

Maintained by [@nishadnp](https://github.com/nishadnp)
