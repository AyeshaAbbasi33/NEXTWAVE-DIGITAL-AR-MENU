# NextWave Digital AR

A WebAR experience built with MindAR.js and A-Frame. Point your phone camera at the marker image to see 3D content appear in augmented reality.

## Project Structure

```
nextwave-digital-ar/
│
├── index.html          ← Main AR scene
│
├── assets/
│   ├── targets.mind    ← Compiled marker file (generate from MindAR compiler)
│   └── dish.glb        ← 3D food model (added later)
│
└── README.md
```

## Setup

### 1. Generate your marker file
Go to [MindAR Compiler](https://hiukim.github.io/mind-ar-js-doc/tools/compile), upload your marker image, compile it, and download `targets.mind`. Place it in the `assets/` folder.

### 2. Deploy via GitHub Pages
```bash
git add .
git commit -m "Day 1: First MindAR.js AR scene"
git push origin main
```
Then enable GitHub Pages in Settings → Pages → Source: main branch.

### 3. Test
Open your GitHub Pages URL on your phone. Point the camera at the marker image — a purple 3D box with "Next Wave AR" label will appear floating in AR.

## Tech Stack
- [MindAR.js](https://hiukim.github.io/mind-ar-js-doc/) — Image tracking & marker detection
- [A-Frame](https://aframe.io/) — 3D scene rendering
