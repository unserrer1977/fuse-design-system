# Fuse Design System for Cloud

A complete design system extracted from the Fuse Fintech Framer template, adapted for cloud products.

## What's Inside

| File | Description |
|------|-------------|
| `reference.html` | Live reference page demonstrating the full design system |
| `palette.html` | Color palette swatch reference (all 126 colors) |
| `DESIGN.md` | Complete design system specification |
| `tokens.css` | CSS custom properties (importable design tokens) |
| `lovable-prompt.md` | Ready-to-paste prompt for Lovable AI |
| `server.js` | Static file server for hosting |

## Run Locally

```bash
node server.js
```

Then open `http://localhost:3000` — serves `reference.html` by default.

## Design System Overview

- **Fonts:** Inter (Google Sans Flex substitute), weights 400–700
- **Primary color:** `#041319` (near-black with cyan tint)
- **Brand accent:** `#1168ea` (blue)
- **Body text:** `#45474d` (warm gray)
- **Section BG gradient:** `#ffffff → #f2fbfd` (white to cyan tint)
- **Max width:** 1312px
- **Card radius:** 16px
- **Nav:** Glassmorphism (`rgba(255,255,255,0.8)` + `backdrop-filter: blur(10px)`)
- **Footer:** Dark `#041319`