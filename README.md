# Ink Bio — Hand-Crafted Interactive Portfolio

A bespoke, tactile landing page inspired by physical printmaking and organic ink simulations. Built with **zero external frameworks** using pure Vanilla HTML5, CSS3, and 2D Canvas.

---

## ✨ Features

- **Blank Scratch-Off Canvas:** The page begins as an untouched sheet of textured paper. Moving or scrolling the cursor scratches through the cover paper, causing the underlying words, cards, and images to softly bloom and fade into view.
- **Continuous Calligraphy Nib & Trailing Ink:**
  - Real-time physics with velocity sensitivity: slow motion creates deep ink puddles, while fast flicks create thin tapers with directional spatter droplets.
  - The ink ribbon renders across the entire viewport on top of all content and evaporates sequentially from tail to cursor over ~1.8s.
  - Active scroll support: Scrolling smoothly shifts existing ink in parallax with the page and scratches open whatever content scrolls under your cursor.
- **Custom Quill Cursor:** Completely suppresses default OS cursors, replacing them with a precision fountain pen nib.
- **Generative Rorschach Blot:** Symmetrical procedural inkblot in the footer that morphs upon click.
- **Paper Grain & Darkroom Aesthetic:** Procedural grain canvas background with high-contrast grayscale photo filtering and an Inked Lightbox modal.
- **Dark Velvet Invert Mode:** Switch between antique cream paper and deep velvet dark mode with inverted ink.

---

## 🚀 Quick Start

### Option 1: Direct File (Zero Dependencies)
You can double-click `index.html` to open and run the project immediately in any modern browser. No installations required.

### Option 2: Local Dev Server (Vite)
If you prefer running a local development server with hot reloading:

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

Visit the displayed local URL (typically `http://localhost:5173`).

---

## 📁 Project Structure

```
ink-bio/
├── index.html       # Complete landing page & INK ENGINE simulation
├── package.json     # Vite development scripts
├── .gitignore       # Git exclusions
└── README.md        # Documentation
```

---

## 🎨 Customization

- **Profile & Bio:** Edit the headlines, discipline, bio paragraphs, and social links inside `<main class="page-wrap">` in `index.html`.
- **Works & Gallery:** Update the `<article class="work-card">` entries with your own titles, descriptions, and image URLs.
- **Color Palette:** Adjust the CSS variables defined in `:root` (e.g. `--paper`, `--ink`, `--vermilion`).
- **Reveal Radius:** Adjust `revealRadius` in `handlePointerMovement()` in `index.html` to make the scratch aperture wider or narrower.
