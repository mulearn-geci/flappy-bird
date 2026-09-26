# Flappy Bird Challenge

A Unity WebGL implementation of Flappy Bird with mission objectives and clue unlock system, ready for seamless deployment on Vercel.

## 🎯 Game Objective
- **Mission**: To get the next clue you have to reach score 20!
- When you reach score 20, the game automatically finishes, plays a victory celebration, and displays the **"You Have Won the Game"** screen with a text box revealing the clue.

## 🚀 Deploy to Vercel

This repository is pre-configured with [`vercel.json`](vercel.json) to serve Unity WebGL's Brotli-compressed assets (`.wasm.br`, `.data.br`, `.framework.js.br`) with the required `Content-Encoding: br` headers.

### Deploy in 2 steps:
1. Go to [Vercel Dashboard](https://vercel.com/new).
2. Import this GitHub repository (`https://github.com/mulearn-geci/flappy-bird.git`) and click **Deploy**.
   - Framework Preset: **Other**
   - Root Directory: `./`
   - Build & Output Settings: Defaults

## 📝 Customizing the Clue Text Box

You can customize the clue text that appears inside the text box when the player wins by editing [`index.html`](index.html):

```javascript
// Inside index.html:
const CLUE_CONTENT = "Your secret clue or link goes here!";
```

Or players can type/copy directly in the victory text box on screen.

## 📁 Project Structure

```text
flappy-bird/
├── .gitignore
├── Build/
│   ├── GameBuilds.data.br
│   ├── GameBuilds.framework.js.br
│   ├── GameBuilds.loader.js
│   └── GameBuilds.wasm.br
├── README.md
├── TemplateData/
│   └── webmemd-icon.png
├── index.html
└── vercel.json
```

## 🎮 Running Locally

To run locally with Brotli header support:

Using Node.js:
```bash
npx serve .
```
