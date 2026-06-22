# webpack-template

<div align="center">
<img width="200" height="200" alt="Webpack Logo" src="https://webpack.js.org/assets/icon-square-big.svg">
</div>

<br>

A reusable JavaScript project template powered by Webpack. Includes development tooling, code quality enforcement, and a scalable project structure for modern frontend applications.

## Features

- - Webpack 5 configuration for development and production

- Dev server with live reload

- Base CSS with light reset (box-sizing, margin reset, line-height)

- CSS and style support (`style-loader` + `css-loader`)

- HTML template handling (`html-webpack-plugin` + `html-loader`)

- Image assets support (`png`, `jpg`, `svg`, `gif`)

- Organized project structure for quick project starts

- ESLint + Prettier for code quality and formatting

- Husky + lint-staged to enforce linting/formatting before commits (scoped to `src/`)

- Split Webpack configuration (common, development, production)

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
│   └── styles/
│       └── base.css
├── webpack.common.js
├── webpack.dev.js
└── webpack.prod.js
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

- **Base styles:** src/styles/base.css

**4. Build**

    npm run build

**5. Clean build output**

    npm run clean

- Removes the `dist/` directory before a fresh build

## Code Quality

- This template includes **ESLint, Prettier, Husky, and lint-staged** to enforce consistent code style.

- Pre-commit hooks automatically lint and format **only files inside `src/`**, intentionally leaving configuration files and tooling untouched.

- ESLint is configured with environment-specific rules for browser (`src/`) and Node (config files) to avoid false positives.

<br>

---

Maintained by [@nishadnp](https://github.com/nishadnp)
