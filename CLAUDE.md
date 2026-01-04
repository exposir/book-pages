# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML repository for hosting book content pages on GitHub Pages. The project contains standalone HTML files for《红色赌盘》(Red Roulette) analysis, each designed to be self-contained and directly accessible via GitHub Pages.

**Live Site:** https://exposir.github.io/book-pages/

## Repository Structure

```
book-pages/
├── red-roulette-chapters.html    # Multi-chapter detailed version with navigation
├── red-roulette-timeline.html    # Visual analysis version with Mermaid diagrams
└── README.md                      # Basic deployment instructions
```

## Architecture

### HTML File Design Pattern

Each HTML file is completely self-contained:
- **No build step required** - files use CDN imports for all dependencies
- **React via UMD** - Uses unpkg.com for React/ReactDOM in production mode
- **Babel Standalone** - JSX compilation happens in-browser via `<script type="text/babel">`
- **Tailwind CSS** - Loaded via CDN script tag
- **Mermaid.js** - Used in timeline version for relationship diagrams

### Why This Architecture?

This repository is designed for **zero-dependency deployment**. Anyone can:
1. Clone the repo
2. Push to GitHub
3. Enable GitHub Pages
4. Get a live website immediately

No `npm install`, no build process, no CI/CD configuration needed.

## Common Development Workflow

### Adding New HTML Pages

1. Create a new `.html` file with a descriptive name (use kebab-case)
2. Use the existing files as templates for the self-contained pattern
3. Add and commit via Git
4. Push to GitHub - the page will be automatically available at `https://exposir.github.io/book-pages/your-file-name.html`

### Deployment Commands

```bash
# After making changes to any HTML file:
git add .
git commit -m "Update content"
git push

# GitHub Pages will auto-update within 1-2 minutes
```

### File Naming Convention

- Use **descriptive names** that reflect content (e.g., `red-roulette-chapters.html`)
- Use **kebab-case** (lowercase with hyphens)
- Avoid generic names like `1.html`, `page2.html`

## Git Workflow

When renaming files, always use `git mv` to preserve history:
```bash
git mv old-name.html new-name.html
```

## Important Notes

- **Each HTML file gets a unique URL** - structure your content accordingly
- **No server-side rendering** - all interactivity must be client-side
- **CDN dependencies** - ensure external script sources remain available
- **Chinese content** - Use `lang="zh-CN"` and UTF-8 encoding
