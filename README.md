# GitHub Repository Browser

A lightweight, zero-cost GitHub repository browser that runs entirely in your browser — no API key required, no backend needed.

**[→ Live Demo](https://nuhbodyok.github.io/repo-browser/)**

![Dark Theme](https://img.shields.io/badge/theme-dark%20slate-818cf8)
![No API Key](https://img.shields.io/badge/API-none%20needed-22c55e)
![GitHub Pages](https://img.shields.io/badge/host-GitHub%20Pages-blue)

## Features

- **Zero Setup** — Works immediately with GitHub's public API (60 requests/hour)
- **Dark Theme** — Easy on the eyes with a modern slate/indigo palette
- **Repository Browsing** — Navigate folders, view files, preview images/audio/video
- **Code Viewing** — Syntax highlighting with copy-to-clipboard
- **Markdown Rendering** — README files render with full formatting
- **Download Options** — Single file download or ZIP export
- **Repository Search** — Search GitHub repositories by keyword
- **Statistics** — Stars, forks, language distribution
- **Rate Limit Tracking** — Live counter showing remaining API calls
- **URL Persistence** — Share links to specific files/folders; back/forward navigation works
- **Recent History** — Quickly revisit previously browsed repos
- **Owner Repo List** — Quick access to all `nuhbodyok` repositories

## Usage

### Option 1: GitHub Pages (Recommended)
1. Fork or clone this repo
2. Go to **Settings → Pages** in your repo
3. Set source to `main` branch
4. Visit `https://yourusername.github.io/repo-browser/`

### Option 2: Local File
1. Download `index.html`
2. Double-click to open in your browser
3. No server required — works entirely client-side

### Option 3: RawGitHack
Use for temporary testing with proper content headers:
```
https://raw.githack.com/nuhbodyok/repo-browser/main/index.html
```

## How to Browse

1. **Enter a repo** — Type `owner/repo` (e.g., `nuhbodyok/repo-browser`) or paste a full GitHub URL
2. **Search** — Prefix with `repos:` to search GitHub (e.g., `repos:react`)
3. **Navigate** — Click folders in the left panel, use breadcrumbs to go back
4. **View files** — Click any file to view with syntax highlighting
5. **Download** — Use the ZIP or Download buttons in the top bar

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Escape` | Close any modal |
| `Enter` | Submit search |

## API Limits

GitHub's unauthenticated API allows **60 requests per hour per IP**. The app tracks usage in real-time and shows when the limit resets.

**Tips to stay under the limit:**
- Stats are cached per repo (no duplicate calls)
- ZIP downloads batch file fetches efficiently
- Avoid rapidly clicking through large repositories

## Tech Stack

- [Tailwind CSS](https://tailwindcss.com/) — Utility-first styling
- [Font Awesome](https://fontawesome.com/) — Icons
- [Marked](https://marked.js.org/) — Markdown parsing
- [Highlight.js](https://highlightjs.org/) — Syntax highlighting
- [JSZip](https://stuk.github.io/jszip/) — ZIP generation
- GitHub REST API v3 — Repository data

## Browser Support

Works in all modern browsers with ES6+ support:
- Chrome/Edge 80+
- Firefox 75+
- Safari 13+

## File Structure

```
repo-browser/
└── index.html          # Single-file application (all CSS/JS inline)
└── README.md           # This file
```

## License

MIT — feel free to fork, modify, and use however you like.

---

Built by [nuhbodyok](https://github.com/nuhbodyok)
