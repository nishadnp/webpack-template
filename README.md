# webpack-template

<div align="center">
<img width="200" height="200" alt="Webpack Logo" src="https://webpack.js.org/assets/icon-square-big.svg">
</div>

<br>

A minimal, reusable JavaScript project template using Webpack. Includes setup for development with CSS, HTML, and image support.

## Features

- Webpack 5 configuration for development
- Dev server with live reload
- Base CSS with light reset (box-sizing, margin reset, line-height)
- CSS and style support (`style-loader` + `css-loader`)
- HTML template handling (`html-webpack-plugin` + `html-loader`)
- Image assets support (`png`, `jpg`, `svg`, `gif`)
- Clean, minimal structure for quick project starts


## Folder Structure

```
webpack-template/
├── package.json
├── package-lock.json
├── README.md
├── src/
│ ├── index.html
│ ├── index.js
│ └── style.css
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

## Notes

- This template uses a single Webpack configuration in development mode.

- Production-specific optimizations (separate configs, webpack-merge, deployment scripts) are intentionally left out and can be added per project as needed.

<br>

---

Maintained by [@nishadnp](https://github.com/nishadnp)
