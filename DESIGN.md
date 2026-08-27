# Fuse Fintech Design System

A complete design system extracted from the Fuse Fintech Framer template, ready for cloud products.

---

## 1. Typography

### Font Families

| Role | Font | Weight Range | Used For |
|------|------|-------------|----------|
| **Primary Display** | Google Sans Flex Variable | 400–450 (variable) | H1, H2, H3, H6, large body text |
| **Primary Text** | Google Sans Flex | 400–700 | H4, body copy, small text, buttons |
| **Secondary/Label** | Inter | 400–700 | H5, labels, captions, UI controls |

> **Google Fonts CDN Substitutes:**
> - `Google Sans Flex` → Use **Google Sans** (or **Inter** as fallback, since Google Sans Flex is not publicly available via Google Fonts)
> - `Inter` → Available directly from Google Fonts
> - Best practical pairing: **Inter** for everything (it's the closest free font), with `font-variation-settings: "opsz" 18, "wdth" 100, "wght" 450` for display text to approximate Google Sans Flex's character.

```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
```

### Font Variation Settings (Google Sans Flex Variable)

```
"opsz" 18, "wdth" 100, "wght" 450, "GRAD" 0, "ROND" 0, "slnt" 0
```

### Typography Scale (Desktop ≥1200px)

| Element | Font Family | Size | Weight | Line Height | Letter Spacing | Color | Alignment |
|--------|------------|------|--------|-------------|----------------|-------|-----------|
| **H1** | Google Sans Flex Variable | 60px | 400 (wght 450) | 1.06667em | 0em | `#041319` | center |
| **H2** | Google Sans Flex Variable | 48px | 400 (wght 450) | 120% | 0em | `#041319` | center |
| **H3** | Google Sans Flex Variable | 36px | 400 (wght 450) | 120% | 0em | `#051219` | start |
| **H4** | Google Sans Flex | 32px | 500 | 120% | 0em | `#041319` | start |
| **H5** | Inter | 20px | 600 | 100% | 0em | `#041319` | start |
| **H6** | Google Sans Flex Variable | 18px | 400 | 120% | 0em | `#041319` | start |
| **Body Large** | Google Sans Flex | 18px | 400 | 1.4333em | 0em | `#45474d` | center |
| **Body** | Google Sans Flex | 16px | 400 | 1.4333em | 0em | `#45474d` | center |
| **Small/Label** | Google Sans Flex | 10–14px | 400–500 | 1.3–1.4333em | 0em | `#45474d` | varies |
| **Caption** | Google Sans Flex | 8–10px | 400 | 1.3em | 0em | `#45474d` | varies |
| **Button Text** | Inter / Google Sans Flex | 14–16px | 500–600 | 1.2em | 0em | varies | center |
| **Input Text** | Google Sans Flex Variable | 16px | 400 | 1.3em | 0em | `#000` | start |
| **Counter/Large Number** | Google Sans Flex Variable | 56–60px | 400 | 120% | 0em | `#041319` | center |

### Typography Scale (Tablet 810–1199px)

| Element | Size | Other changes |
|--------|------|---------------|
| H1 | 38px | — |
| H2 | 24px | — |
| H3 | 20px | — |
| H4 | 24px | — |
| H5 | 18px | — |
| Body | 16px | — |

### Typography Scale (Mobile ≤809px)

| Element | Size |
|--------|------|
| H1 | 32px |
| H2 | 32px |
| H3 | 36px |
| H4 | 20px |
| H5 | 16px |
| Body | 18px |

---

## 2. Color Palette

### Primary Colors

| Token | Hex | RGB | Usage |
|-------|-----|-----|-------|
| **Primary Dark** | `#041319` | `rgb(4, 19, 25)` | Headings (H1, H2, H4 text color) |
| **Secondary Dark** | `#051219` | — | H3 headings |
| **Tertiary Dark** | `#05131a` | — | Alternate heading dark |
| **Darkest** | `#0c0c0c` | — | Footer / darkest UI |
| **Dark Alt** | `#0c111d` | `rgb(12, 17, 29)` | Dark cards, panels |
| **Body Text** | `#45474d` | `rgb(69, 71, 77)` | Paragraph text, descriptions |
| **Muted Text** | `#555` | — | Secondary text |
| **Placeholder Gray** | `#767d82` | `rgb(118, 125, 130)` | Input placeholder text |
| **Label Gray** | `#797c86` | `rgb(121, 124, 134)` | Form labels |
| **Secondary Gray** | `#9097a0` | — | Tertiary text |
| **Border Gray** | `#a1a6a8` | `rgb(161, 166, 168)` | Disabled states |
| **Card Border** | `#374248` | `rgb(55, 66, 72)` | Dark card borders |

### Accent / Brand Colors

| Token | Hex | RGB | Usage |
|-------|-----|-----|-------|
| **Brand Blue** | `#1168ea` | `rgb(17, 104, 234)` | Primary accent, links, buttons |
| **Link Blue** | `#0177cc` | `rgb(1, 119, 204)` | Links |
| **Link Blue Alt** | `#0177cb` | — | Links |
| **Light Blue** | `#2e7aff` | `rgb(46, 122, 255)` | Interactive elements |
| **Blue Alt** | `#2f7aff` | — | Interactive elements |
| **Bright Blue** | `#09f` | `rgb(0, 153, 255)` | Link text color |
| **Sky Blue** | `#4ab3ff` | `rgb(124, 171, 254)` | Gradients |
| **Cyan Accent** | `#6af3ff` | `rgb(106, 243, 255)` | Highlights, glow effects |
| **Cyan Light** | `#b0fdfe` | — | Soft accents |
| **Cyan Tint** | `#d3f9fd` | — | Backgrounds |
| **Cyan Bright** | `#60c5d9` | — | Teal accent |
| **Teal** | `#1ac4d7` | `rgb(26, 196, 215)` | Secondary accent |
| **Teal Deep** | `#069c9e` | — | Darker teal |
| **Light Blue BG** | `#def1ff` | — | Light blue backgrounds |
| **Light Blue BG 2** | `#e8f5fd` | — | Light blue backgrounds |
| **Light Blue BG 3** | `#eefbfd` | — | Lightest blue backgrounds |

### Surface Colors

| Token | Hex | RGB | Usage |
|-------|-----|-----|-------|
| **White** | `#fff` | `rgb(255, 255, 255)` | Primary background |
| **Near White** | `#fdfdfe` | `rgb(253, 253, 254)` | Alt white background |
| **Off White** | `#fafafa` | — | Subtle background |
| **Light Gray BG** | `#f7f7f7` | `rgb(247, 247, 247)` | Section backgrounds |
| **Light Gray** | `#f2f2f2` | `rgb(242, 242, 242)` | Card backgrounds |
| **Light Gray Alt** | `#f2f3f5` | `rgb(242, 243, 245)` | Subtle surfaces |
| **Cyan Tint BG** | `#f2fbfd` | — | Cyan-tinted background |
| **Border Light** | `#eaeaea` | `rgb(234, 234, 234)` | Light borders |
| **Border Lighter** | `#e2e2e2` | — | Lighter borders |
| **Border Subtle** | `#e6e7e8` | — | Subtle dividers |
| **Border Gray Light** | `#eceeee` | — | Card borders |
| **Surface Gray** | `#eef0f3` | — | Neutral surface |
| **Divider** | `#dfdede` | `rgb(223, 222, 222)` | Dividers |
| **Dark Border** | `#262020` | — | Dark mode borders |

### Status Colors

| Token | Hex | RGB | Usage |
|-------|-----|-----|-------|
| **Success Green** | `#07ba1b` | — | Success states |
| **Success Green Dark** | `#248830` | `rgb(36, 136, 48)` | Darker success |
| **Success Green Deep** | `#006341` | `rgb(0, 99, 65)` | Deep green |
| **Success Bg** | `#cdffd3` | — | Success background |
| **Warning Orange** | `#fb8000` | — | Warning states |
| **Warning Bg** | `#fbeddf` | — | Warning background |
| **Error Red** | `#e01e5a` | — | Error states |
| **Info Blue** | `#1168ea` | — | Info states |

### Social/Integration Colors (used in logos)

| Token | Hex | Usage |
|-------|-----|-------|
| `#ecb22e` | Slack yellow |
| `#36c5f0` | Slack blue |
| `#2eb67d` | Slack green |
| `#e01e5a` | Slack pink |
| `#975bff` | Purple accent |
| `#9ea3ff` | `rgb(158, 163, 255)` Light purple |
| `#ece2ff` | Light purple background |

### Transparent Overlays

| Token | Value | Usage |
|-------|-------|-------|
| **Overlay 05%** | `rgba(0,0,0,0.05)` | Subtle shadows |
| **Overlay 06%** | `rgba(0,0,0,0.06)` | Card shadows |
| **Overlay 08%** | `rgba(0,0,0,0.08)` | Elevated shadows |
| **Overlay 10%** | `rgba(0,0,0,0.1)` | Dropdown shadows |
| **Overlay 12%** | `rgba(0,0,0,0.12)` | Deep shadows |
| **Overlay 14%** | `rgba(0,0,0,0.14)` | Modal shadows |
| **Overlay 16%** | `rgba(0,0,0,0.16)` | Max shadows |
| **Overlay 92%** | `rgba(0,0,0,0.92199)` | Near-black overlay |
| **Border 06%** | `rgba(33,34,38,0.06)` | Border color |
| **White 22%** | `rgba(255,255,255,0.22)` | Glass effect |
| **White 25%** | `rgba(255,255,255,0.25)` | Glass effect |
| **White 30%** | `rgba(255,255,255,0.3)` | Glass effect |
| **White 40%** | `rgba(255,255,255,0.4)` | Glass effect |
| **White 80%** | `rgba(255,255,255,0.8)` | Hover states |
| **White Alpha** | `#ffffff1a` | White 10% opacity |
| **White Alpha B3** | `#ffffffb3` | White 70% opacity |
| **Dark Alpha** | `#000000eb` | Near-black 92% |
| **Dark Alpha 29** | `#00000029` | Dark 16% |

### Gradients

| Name | Value |
|------|-------|
| **Hero Fade** | `linear-gradient(#f7feff00 0%, #fff 65%)` |
| **Section BG** | `linear-gradient(#fff 19%, #f2fbfd 100%)` |
| **Text Fade** | `linear-gradient(89deg, #041319 0%, rgba(4,19,26,0) 100%)` |
| **Blue Gradient** | `linear-gradient(90deg, rgb(43,167,255) 0%, rgb(136,207,253) 100%)` |

---

## 3. Spacing & Layout

### Section Padding

| Breakpoint | Section Padding |
|------------|----------------|
| Desktop (≥1200px) | `80px 30px` |
| Tablet (810–1199px) | `50px 20px` |
| Mobile (≤809px) | `50px 20px` |

### Page Max Width

| Breakpoint | Max Width |
|------------|-----------|
| Desktop | `min(100vw - 60px, 1312px)` |
| Tablet | `min(100vw - 40px, 1312px)` |
| Mobile | `min(100vw - 40px, 1312px)` |

### Common Padding Values

| Usage | Value |
|-------|-------|
| Card padding | `24px` |
| Card padding (tight) | `16px` |
| Button padding | `12px 16px` |
| Button padding (large) | `16px 24px` |
| Input padding | `14px 14px 13px 14px` |
| Nav padding | `0 48px` / `0 16px` |
| Section inner | `80px 30px` / `50px 20px` |
| Badge padding | `6px 8px` / `8px 12px` |
| Feature gap | `40px` |
| Content gap | `24px` |
| Tight gap | `16px` |

### Gap Values

| Usage | Value |
|-------|-------|
| Feature grid gap | `40px` |
| Card content gap | `24px` |
| Form field gap | `16px` |
| Nav item gap | `24px` |
| Badge gap | `8px` |
| Tight gap | `4px` |
| Section gap | `48px` |
| Hero gap | `32px` |

---

## 4. Border Radius

| Token | Value | Usage |
|-------|-------|-------|
| **None** | `0` | No rounding |
| **XS** | `4px` | Small badges, tags |
| **SM** | `5px` | Small elements |
| **MD** | `8px` | Inputs, small cards |
| **LG** | `12px` | Cards, buttons |
| **XL** | `13px` | Large cards |
| **2XL** | `15px` | Feature cards |
| **3XL** | `16px` | Large cards, inputs |
| **Pill** | `999px` | Pills, badges |
| **Full** | `100%` | Circular / full |
| **Mega** | `695px` | Large rounded sections |

---

## 5. Shadows

| Token | Value | Usage |
|-------|-------|-------|
| **XS** | `0 1px 2px rgba(0,0,0,0.05)` | Subtle elevation |
| **SM** | `0 1px 3px rgba(0,0,0,0.12)` | Cards |
| **SM 2** | `0 1px 2px rgba(0,0,0,0.06)` | Cards subtle |
| **MD** | `0 2px 4px rgba(0,0,0,0.06)` | Raised elements |
| **MD 2** | `0 4px 8px rgba(0,0,0,0.06)` | Raised cards |
| **LG** | `0 10px 20px rgba(0,0,0,0.1)` | Dropdowns |
| **LG 2** | `0 2.2px 20px rgba(0,0,0,0.1)` | Modals |
| **XL** | `0 10px 26px rgba(0,0,0,0.08)` | Floating panels |
| **Button** | `0px 1px 3px 0px rgba(0,0,0,0.12)` | Button shadow |
| **Button Hover** | `0px 2px 4px rgba(0,0,0,0.06)` | Button hover shadow |
| **Deep Card** | `0px 0.6px 1.57px -1.5px rgba(0,0,0,0.17), 0px 2.29px 5.95px -3px rgba(0,0,0,0.14), 0px 10px 26px -4.5px rgba(0,0,0,0.02)` | Premium card shadow |
| **Inset** | `inset 0px 0px 0px 1px rgb(0,0,0)` | Inset border |
| **Card Mini** | `0px 0.55px 3px 0px rgba(0,0,0,0.12)` | Mini card shadow |
| **Card Icon** | `0px 1px 8px 0px rgba(0,0,0,0.08)` | Icon container shadow |

---

## 6. Components

### Buttons

```css
/* Primary Button (dark/black) */
.btn-primary {
  background: #041319;           /* or #0c111d for darker */
  color: #ffffff;
  font-family: 'Inter', sans-serif;
  font-size: 16px;
  font-weight: 500;
  line-height: 1.2em;
  letter-spacing: 0em;
  padding: 12px 16px;
  border-radius: 12px;
  border: none;
  box-shadow: 0px 1px 3px 0px rgba(0,0,0,0.12);
  cursor: pointer;
  transition: all 0.2s ease;
}

/* Secondary Button (white/outline) */
.btn-secondary {
  background: #ffffff;
  color: #041319;
  font-family: 'Inter', sans-serif;
  font-size: 16px;
  font-weight: 500;
  padding: 12px 16px;
  border-radius: 12px;
  border: 1px solid rgba(33,34,38,0.06);
  box-shadow: 0px 1px 3px 0px rgba(0,0,0,0.12);
}

/* Large CTA Button */
.btn-cta {
  background: #041319;
  color: #ffffff;
  font-size: 16px;
  font-weight: 500;
  padding: 16px 24px;
  border-radius: 12px;
}
```

### Cards

```css
.card {
  background: #ffffff;
  border-radius: 16px;
  padding: 24px;
  box-shadow: 0px 1px 3px 0px rgba(0,0,0,0.12);
  border: 1px solid rgba(33,34,38,0.06);
}

.card-feature {
  background: #ffffff;
  border-radius: 16px;
  padding: 24px;
  box-shadow: 0px 2px 4px rgba(0,0,0,0.06);
  gap: 16px;
}

.card-premium {
  background: #ffffff;
  border-radius: 16px;
  box-shadow:
    0px 0.6px 1.57px -1.5px rgba(0,0,0,0.17),
    0px 2.29px 5.95px -3px rgba(0,0,0,0.14),
    0px 10px 26px -4.5px rgba(0,0,0,0.02);
}
```

### Navigation

```css
.nav {
  background: rgba(255,255,255,0.8);
  backdrop-filter: blur(10px);
  border-bottom: 1px solid rgba(33,34,38,0.06);
  padding: 0 48px;
  height: 72px;
}

.nav-link {
  font-family: 'Inter', sans-serif;
  font-size: 14px;
  font-weight: 500;
  color: #45474d;
}

.nav-link:hover {
  color: #041319;
}
```

### Badges / Pills

```css
.badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 6px 8px;
  border-radius: 999px;
  font-family: 'Inter', sans-serif;
  font-size: 12px;
  font-weight: 500;
  background: #f2f3f5;
  color: #45474d;
}

.badge-blue {
  background: #eefbfd;
  color: #0177cc;
}

.badge-success {
  background: #cdffd3;
  color: #006341;
}

.badge-warning {
  background: #fbeddf;
  color: #fb8000;
}
```

### Inputs

```css
.input {
  background: #ffffff;
  border: 1px solid rgba(33,34,38,0.06);
  border-radius: 16px;
  padding: 14px 14px 13px 14px;
  font-family: 'Google Sans Flex Variable', 'Inter', sans-serif;
  font-size: 16px;
  font-weight: 400;
  color: #000000;
  line-height: 1.3em;
  letter-spacing: 0em;
}

.input::placeholder {
  color: #797c86;
}
```

### Footer

```css
.footer {
  background: #041319;
  color: #ffffff;
  padding: 80px 30px;
}

.footer-link {
  color: rgba(255,255,255,0.8);
  font-family: 'Inter', sans-serif;
  font-size: 14px;
  font-weight: 400;
}
```

---

## 7. Responsive Breakpoints

| Name | Min Width | Max Width | Container |
|------|-----------|-----------|-----------|
| **Mobile** | 0px | 809.98px | `min(100vw - 40px, 1312px)` |
| **Tablet** | 810px | 1199.98px | `min(100vw - 60px, 1312px)` |
| **Desktop** | 1200px | — | `min(100vw - 60px, 1312px)` |

---

## 8. CSS Custom Properties (Design Tokens)

```css
:root {
  /* === Colors === */
  --color-primary: #041319;
  --color-primary-alt: #051219;
  --color-secondary: #05131a;
  --color-darkest: #0c0c0c;
  --color-dark-panel: #0c111d;
  --color-body: #45474d;
  --color-muted: #555;
  --color-placeholder: #767d82;
  --color-label: #797c86;
  --color-tertiary: #9097a0;
  --color-border-gray: #a1a6a8;
  --color-card-border: #374248;

  /* Brand */
  --color-brand: #1168ea;
  --color-link: #0177cc;
  --color-link-bright: #0099ff;
  --color-blue: #2e7aff;
  --color-sky: #4ab3ff;
  --color-cyan: #6af3ff;
  --color-cyan-light: #b0fdfe;
  --color-teal: #1ac4d7;
  --color-teal-deep: #069c9e;

  /* Surfaces */
  --color-white: #ffffff;
  --color-near-white: #fdfdfe;
  --color-off-white: #fafafa;
  --color-bg-gray: #f7f7f7;
  --color-surface-gray: #f2f2f2;
  --color-surface-gray-alt: #f2f3f5;
  --color-cyan-tint-bg: #f2fbfd;
  --color-border: #eaeaea;
  --color-border-alt: #e2e2e2;
  --color-border-subtle: #e6e7e8;
  --color-border-card: #eceeee;
  --color-surface: #eef0f3;
  --color-divider: #dfdede;
  --color-dark-border: #262020;

  /* Status */
  --color-success: #07ba1b;
  --color-success-dark: #248830;
  --color-success-deep: #006341;
  --color-success-bg: #cdffd3;
  --color-warning: #fb8000;
  --color-warning-bg: #fbeddf;
  --color-error: #e01e5a;
  --color-info: #1168ea;

  /* Light BGs */
  --color-bg-blue-1: #def1ff;
  --color-bg-blue-2: #e8f5fd;
  --color-bg-blue-3: #eefbfd;

  /* Overlays */
  --overlay-05: rgba(0,0,0,0.05);
  --overlay-06: rgba(0,0,0,0.06);
  --overlay-08: rgba(0,0,0,0.08);
  --overlay-10: rgba(0,0,0,0.1);
  --overlay-12: rgba(0,0,0,0.12);
  --overlay-14: rgba(0,0,0,0.14);
  --overlay-16: rgba(0,0,0,0.16);
  --overlay-92: rgba(0,0,0,0.92);
  --border-06: rgba(33,34,38,0.06);
  --glass-22: rgba(255,255,255,0.22);
  --glass-30: rgba(255,255,255,0.3);
  --glass-40: rgba(255,255,255,0.4);
  --glass-80: rgba(255,255,255,0.8);

  /* === Typography === */
  --font-display: 'Inter', sans-serif; /* Google Sans Flex Variable substitute */
  --font-body: 'Inter', sans-serif;     /* Google Sans Flex substitute */
  --font-label: 'Inter', sans-serif;    /* Inter (exact match) */

  --font-variation-display: "opsz" 18, "wdth" 100, "wght" 450, "GRAD" 0, "ROND" 0, "slnt" 0;

  /* Type Scale (Desktop) */
  --text-h1: 60px;
  --text-h2: 48px;
  --text-h3: 36px;
  --text-h4: 32px;
  --text-h5: 20px;
  --text-h6: 18px;
  --text-body-lg: 18px;
  --text-body: 16px;
  --text-small: 14px;
  --text-caption: 12px;
  --text-tiny: 10px;

  /* Line Heights */
  --leading-h1: 1.06667em;
  --leading-heading: 120%;
  --leading-body: 1.4333em;
  --leading-tight: 100%;
  --leading-input: 1.3em;

  /* Font Weights */
  --weight-regular: 400;
  --weight-medium: 500;
  --weight-semibold: 600;
  --weight-bold: 700;

  /* === Spacing === */
  --space-xs: 4px;
  --space-sm: 8px;
  --space-md: 16px;
  --space-lg: 24px;
  --space-xl: 32px;
  --space-2xl: 40px;
  --space-3xl: 48px;
  --space-4xl: 80px;

  /* === Border Radius === */
  --radius-none: 0;
  --radius-xs: 4px;
  --radius-sm: 8px;
  --radius-md: 12px;
  --radius-lg: 16px;
  --radius-pill: 999px;
  --radius-full: 100%;

  /* === Shadows === */
  --shadow-xs: 0 1px 2px rgba(0,0,0,0.05);
  --shadow-sm: 0 1px 3px rgba(0,0,0,0.12);
  --shadow-md: 0 2px 4px rgba(0,0,0,0.06);
  --shadow-lg: 0 10px 20px rgba(0,0,0,0.1);
  --shadow-xl: 0 10px 26px rgba(0,0,0,0.08);
  --shadow-button: 0px 1px 3px 0px rgba(0,0,0,0.12);
  --shadow-card-premium: 0px 0.6px 1.57px -1.5px rgba(0,0,0,0.17),
                         0px 2.29px 5.95px -3px rgba(0,0,0,0.14),
                         0px 10px 26px -4.5px rgba(0,0,0,0.02);

  /* === Gradients === */
  --gradient-hero-fade: linear-gradient(rgba(247,254,255,0) 0%, #fff 65%);
  --gradient-section: linear-gradient(#fff 19%, #f2fbfd 100%);
  --gradient-blue: linear-gradient(90deg, rgb(43,167,255) 0%, rgb(136,207,253) 100%);

  /* === Layout === */
  --max-width: 1312px;
  --nav-height: 72px;
  --section-padding-desktop: 80px 30px;
  --section-padding-tablet: 50px 20px;
  --section-padding-mobile: 50px 20px;
}
```

---

## 9. Font Details

### Google Sans Flex Variable (Display)
- **Variable Axes:** opsz=18, wdth=100, wght=450, GRAD=0, ROND=0, slnt=0
- **Usage:** H1, H2, H3, H6, large numbers/counters
- **CDN Substitute:** Inter (closest free font; set `font-weight: 450` with `font-variation-settings` if using a variable font)

### Google Sans Flex (Text)
- **Usage:** H4, body text, small labels, captions
- **Weight:** 400 (regular), 500 (medium), 700 (bold)
- **CDN Substitute:** Inter

### Inter (Labels/UI)
- **Usage:** H5, form labels, button text, nav links, UI controls
- **Weight:** 400, 500, 600, 700
- **CDN:** Available directly from Google Fonts

---

## 10. Page Structure

### Typical Section Order

1. **Navigation** — fixed/sticky, glassmorphism (white 80% opacity + blur), logo left, links center/right, CTA button right
2. **Hero** — centered text, H1 + body text + CTA buttons, large dashboard screenshot below
3. **Logo Cloud** — "25,000+ companies" text + grayscale logos row
4. **Features Grid** — section label (eyebrow) + H2 + description + 4 feature cards with icons
5. **Feature Showcase** — alternating image + text, checkmark lists
6. **Stats/Counters** — large numbers with labels
7. **Integrations** — logo grid with "See all" link
8. **Security** — compliance badges + security feature cards
9. **How It Works** — numbered steps (01, 02, 03) with images
10. **Customer Stories** — testimonial cards with company logo, quote, link
11. **Pricing** — 3-tier pricing table (Starter/Growth/Enterprise)
12. **Final CTA** — dark background, centered H2 + buttons
13. **Footer** — dark (#041319), logo + links columns + social icons + compliance badges

### Eyebrow / Section Labels

```css
.eyebrow {
  font-family: 'Inter', sans-serif;
  font-size: 12px;
  font-weight: 500;
  letter-spacing: 0em;
  color: #45474d;
  text-transform: uppercase;
  padding: 6px 8px;
  border-radius: 999px;
  background: #f2f3f5;
  display: inline-flex;
  align-items: center;
  gap: 6px;
}
```

---

## 11. Animation & Motion

The template uses Framer Motion for:
- **Fade + slide up** on scroll-into-view (sections, cards)
- **Hover scale** on interactive elements (cards, buttons)
- **Carousel/scroll** for customer stories and logo clouds
- **Counter animation** for stats numbers
- **Marquee** for notification feed items

Suggested CSS equivalents:
```css
@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

.card:hover {
  transform: translateY(-2px);
  box-shadow: 0px 4px 8px rgba(0,0,0,0.06);
  transition: all 0.3s ease;
}
```

---

## 12. Iconography

The template uses custom SVG icons (inline, from framerusercontent.com). Key characteristics:
- 16–20px size for inline icons
- 20–24px size for feature card icons
- Checkmark icons: simple, single-color (#041319 or contextual color)
- Arrow icons: 13×13px, black, used for "Learn more" links
- Feature icons: 14–18px, contained in a rounded square with subtle background

---

## Implementation Notes for Cloud

1. **Replace** "Fuse" branding with your cloud product name
2. **Swap** fintech-specific imagery/icons for cloud infrastructure equivalents
3. **Keep** the color palette — it's designed for trust/enterprise and works well for cloud/infra
4. **Inter** is the best free font substitute for both Google Sans Flex and Inter roles
5. **Use** `font-variation-settings: "wght" 450` on display headings if you have a variable font
6. **Glassmorphism nav** uses `backdrop-filter: blur(10px)` with `rgba(255,255,255,0.8)` background
7. **Dark sections** use `#041319` or `#0c0c0c` with white text
8. **Cards** use subtle shadows + `rgba(33,34,38,0.06)` border for the "Framer" look
9. **Pills/badges** are `999px` radius with tinted backgrounds (cyan tint for blue, green tint for success)
10. **Section padding** is generous: `80px 30px` on desktop, `50px 20px` on tablet/mobile