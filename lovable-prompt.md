# Lovable Prompt — Fuse Design System for Cloud

Copy everything below this line and paste it into Lovable as your prompt.

---

Build a cloud platform landing page using this exact design system. Replicate every color, font, spacing, shadow, and component style precisely.

## Design Tokens (use these as CSS variables / Tailwind config)

### Colors
```css
--color-primary: #041319;        /* Headings, dark sections */
--color-primary-alt: #051219;
--color-body: #45474d;           /* Paragraph text */
--color-muted: #555555;
--color-placeholder: #767d82;
--color-label: #797c86;
--color-tertiary: #9097a0;

--color-brand: #1168ea;          /* Primary accent / buttons / links */
--color-link: #0177cc;
--color-link-bright: #0099ff;
--color-blue: #2e7aff;
--color-sky: #4ab3ff;
--color-cyan: #6af3ff;
--color-cyan-light: #b0fdfe;
--color-cyan-tint: #d3f9fd;
--color-teal: #1ac4d7;

--color-white: #ffffff;
--color-near-white: #fdfdfe;
--color-off-white: #fafafa;
--color-bg-gray: #f7f7f7;
--color-surface-gray: #f2f2f2;
--color-surface-gray-alt: #f2f3f5;
--color-cyan-tint-bg: #f2fbfd;   /* Light section background */
--color-border: #eaeaea;
--color-border-subtle: #e6e7e8;
--color-surface: #eef0f3;
--color-divider: #dfdede;

--color-success: #07ba1b;
--color-success-bg: #cdffd3;
--color-warning: #fb8000;
--color-warning-bg: #fbeddf;
--color-error: #e01e5a;
```

### Typography
- **Font family for everything:** `'Inter', system-ui, sans-serif` (loaded from Google Fonts)
- **Display headings (H1, H2, H3):** font-weight 400, with `font-variation-settings: "opsz" 18, "wdth" 100, "wght" 450` if variable font is available
- **H4:** font-weight 500
- **H5, labels, buttons, nav:** font-weight 600
- **Body text:** font-weight 400

| Element | Desktop | Tablet | Mobile | Line Height |
|--------|---------|--------|--------|-------------|
| H1 | 60px | 38px | 32px | 1.06667em |
| H2 | 48px | 24px | 32px | 120% |
| H3 | 36px | 20px | 36px | 120% |
| H4 | 32px | 24px | 20px | 120% |
| H5 | 20px | 18px | 16px | 100% |
| H6 | 18px | 18px | 18px | 120% |
| Body | 18px | 16px | 18px | 1.4333em |
| Small | 16px | 16px | 16px | 1.4333em |
| Caption | 12px | 12px | 12px | 1.3em |

All letter-spacing: 0em. Headings color: #041319. Body color: #45474d.

### Spacing
- Section padding: 80px 30px (desktop), 50px 20px (tablet/mobile)
- Max width container: 1312px, with 30px horizontal padding
- Card padding: 24px
- Button padding: 12px 16px (normal), 16px 24px (large CTA)
- Input padding: 14px 14px 13px 14px
- Feature grid gap: 24px
- Section gap between elements: 40px
- Nav height: 72px

### Border Radius
- Cards: 16px
- Buttons: 12px
- Inputs: 16px
- Badges/pills: 999px
- Small elements: 8px

### Shadows
- Card: `0 1px 3px rgba(0,0,0,0.12)` + `1px solid rgba(33,34,38,0.06)` border
- Card hover: `0 2px 4px rgba(0,0,0,0.06)`
- Premium card: `0px 0.6px 1.57px -1.5px rgba(0,0,0,0.17), 0px 2.29px 5.95px -3px rgba(0,0,0,0.14), 0px 10px 26px -4.5px rgba(0,0,0,0.02)`
- Dropdown: `0 10px 20px rgba(0,0,0,0.1)`
- Button: `0px 1px 3px 0px rgba(0,0,0,0.12)`

### Gradients
- Hero section: `linear-gradient(180deg, #ffffff 0%, #f2fbfd 100%)`
- Section background: `linear-gradient(#ffffff 19%, #f2fbfd 100%)`
- Blue gradient (for accents): `linear-gradient(90deg, rgb(43,167,255) 0%, rgb(136,207,253) 100%)`

### Navigation
- Sticky, height 72px
- Background: `rgba(255,255,255,0.8)` with `backdrop-filter: blur(10px)`
- Border-bottom: `1px solid rgba(33,34,38,0.06)`
- Logo left, nav links center, CTA buttons right
- Nav link font: 14px, weight 500, color #45474d, hover #041319

### Buttons
- Primary: background #041319, color white, 16px, weight 500, radius 12px, padding 12px 16px, shadow 0px 1px 3px rgba(0,0,0,0.12)
- Secondary: background white, color #041319, border 1px solid rgba(33,34,38,0.06), same shadow
- Large CTA: padding 16px 24px

### Cards
- Background white, radius 16px, padding 24px
- Shadow: 0 1px 3px rgba(0,0,0,0.12)
- Border: 1px solid rgba(33,34,38,0.06)
- Hover: translateY(-2px), shadow 0 2px 4px rgba(0,0,0,0.06)

### Badges / Pills (eyebrow labels)
- Display inline-flex, gap 6px, padding 6px 8px
- Border-radius 999px
- Background #f2f3f5, color #45474d
- Font 12px, weight 500, uppercase
- Blue variant: background #eefbfd, color #0177cc
- Success variant: background #cdffd3, color #006341

### Footer
- Background #041319, color white
- Padding 80px 30px
- Links: rgba(255,255,255,0.8), 14px, weight 400
- Top border: 1px solid rgba(255,255,255,0.1)

## Page Structure (build these sections in order)

1. **Nav** — glassmorphism sticky nav with logo, 4 links, Sign in + Book demo buttons
2. **Hero** — centered H1 "The [cloud platform] for modern teams", body text, 2 CTA buttons, "No credit card required · Cancel anytime" microcopy, large dashboard preview placeholder below
3. **Logo cloud** — "25,000+ companies..." text + row of placeholder logos
4. **Features** — eyebrow label "EVERYTHING YOUR TEAM NEEDS", H2, description, 4-column grid of feature cards with icon + title + description + "Learn more →" link
5. **Showcase** — split layout: image placeholder on one side, eyebrow + H3 + text + checklist with checkmark icons on the other. Background: gradient white→#f2fbfd
6. **Stats** — 4 large numbers in a row (56-60px font) with small labels below
7. **Pricing** — 3 cards: Starter (Free), Growth ($15/user/month, featured with badge), Enterprise (Custom). Each with feature checklist + button
8. **Final CTA** — dark section (#041319), centered H2 + button
9. **Footer** — dark, 4-column: brand+description, Product links, Company links, Legal links. Bottom bar with copyright + compliance badges

## Responsive Breakpoints
- Desktop: ≥1200px (4-column feature grid, 3-column pricing)
- Tablet: 810-1199px (2-column features, 1-column pricing, smaller headings)
- Mobile: ≤809px (1-column everything, nav links hidden, 50px section padding)

## Important Notes
- Use Inter from Google Fonts for ALL text
- Headings should feel light (weight 400), not bold — this is key to the Fuse aesthetic
- Cards have very subtle shadows + barely-visible borders — not heavy
- The overall feel is clean, airy, light-backgrounded with cyan-tinted section backgrounds
- Section padding is generous (80px vertical on desktop)
- The nav uses glassmorphism (translucent white + blur)
- Eyebrow labels are small pill-shaped badges above section headings