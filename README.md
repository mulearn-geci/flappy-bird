# Flappy Bird

A Unity WebGL implementation of the classic Flappy Bird game.

## Overview

This repository contains the Unity WebGL build for the Flappy Bird game.

## Project Structure

```
flappy-bird/
├── Build/
│   ├── GameBuilds.data.br
│   ├── GameBuilds.framework.js.br
│   ├── GameBuilds.loader.js
│   └── GameBuilds.wasm.br
├── TemplateData/
│   └── webmemd-icon.png
├── index.html
└── README.md
```

## Running Locally

Because WebGL builds use WebAssembly (`.wasm`) and Brotli-compressed assets (`.br`), you need to serve the files using a local HTTP server:

Using Python:
```bash
python -m http.server 8000
```

Using Node.js:
```bash
npx serve .
```

Then navigate to `http://localhost:8000` (or the port provided) in your browser.
