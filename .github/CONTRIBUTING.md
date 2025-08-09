# Contributing to Hallows Eve (Spellbound Scents’ Dawn Fork)

First off, thank you for your interest in contributing! 🎃  
**Hallows Eve** is a customized fork of Shopify’s [Dawn](https://github.com/Shopify/dawn) theme for **Spellbound Scents Wax Co.** with a kawaii/cute Halloween aesthetic. We welcome fixes, improvements, and documentation updates that keep the theme fast, accessible, and spooky-sweet year‑round.

> 💡 **Scope:** This repo is a Dawn fork primarily tailored to Spellbound Scents. External contributions are welcome if they:
> - Improve performance, accessibility, or code quality
> - Fix bugs and visual inconsistencies
> - Add general-purpose options that can be toggled in theme settings
> - Refine our Kawaii Halloween visual system without breaking brand consistency

---

## Code of Conduct

By participating, you agree to uphold our [Code of Conduct](./CODE_OF_CONDUCT.md). Be kind, be respectful, and bring good vibes.

---

## How to Contribute

### 1) Discuss first (issues)
- Open an issue describing the change (bug, enhancement, or documentation).
- Include reproduction steps or screenshots for UI issues.
- Tag it with an appropriate label (e.g., `bug`, `enhancement`, `docs`).

### 2) Fork & branch
- Fork the repo and create a branch:
  - `fix/header-icon-alignment`
  - `feat/theme-settings-candy-corn-button`
  - `docs/readme-license-badge`

### 3) Dev environment
- You’ll need:
  - Node 18+ (LTS recommended)
  - Shopify CLI
  - Theme Check
  - Prettier

```bash
# install dependencies if applicable
npm install

# run theme check (Liquid, JSON, etc.)
npx @shopify/theme-check

# format code
npx prettier --write .
```

Optional but recommended for previewing:
```bash
# login and serve to a dev store
shopify login --store <your-store>.myshopify.com
shopify theme dev
```

### 4) Style & conventions
# General

- Keep PRs focused and small. One feature or fix per PR.
- Include before/after screenshots or GIFs for UI changes.
- Update documentation (README, comments, or settings schema) if behavior changes.

# Liquid

- Prefer settings-driven changes over hard-coded values.
- Maintain accessibility (semantic HTML, ARIA where needed).
- Keep translation strings in /locales.

# CSS

- Prefer utility-like, minimal CSS. Avoid heavy overrides.
- Respect the candy corn palette and Kawaii Halloween aesthetic.
- Reuse existing variables/tokens if available.

# JavaScript

- Avoid large dependencies; stick to Dawn’s lightweight approach.
- Progressive enhancement: don’t break core functionality without JS.
  
# Commit messages

- Use conventional-style messages when possible:
  - fix: correct cart icon stroke width on mobile
  - feat: add setting to toggle candy-corn CTA style
  - docs: add MIT + Dawn attribution to README

### 5) Tests & checks
- Run Theme Check and Prettier before pushing.
- Manually test:
  - Header icons (cart/search/account)
  - Buttons/CTAs (hover/focus states)
  - Product cards, PDP, and Collections
  - Mobile responsiveness
  - Contrast and focus visibility
    
### Pull Request Checklist
 - Issue created/linked describing the change
 - Small, focused PR (screenshots for UI)
 - No breaking changes to existing settings unless documented and migrated
 - @shopify/theme-check passes
 - prettier --write . run
 - README / settings schema updated if needed

### Design Guidelines (Hallows Eve)
- Aesthetic: Kawaii/Cute Halloween; playful but readable; year‑round “Halloween anytime.”
- Palette: Candy corn (warm white #fffaf0, pumpkin/orange, golden yellow), plus neutral darks for contrast.
- Icons: Rounded, friendly shapes; avoid harsh edges.
- Accessibility: Maintain WCAG AA contrast and visible focus states.
- Performance: Keep it lean—prefer CSS over JS; remove unused assets.

### Security & Reporting
## If you discover a security issue, do not open a public issue. Email us at inbox@spellboundscentswax.com with details. We’ll respond as soon as possible.

### License & Attribution
Contributions are licensed under the repository’s MIT License.
This project is a modified version of Shopify’s Dawn theme (also MIT). Portions of the code are © Shopify Inc. and Dawn contributors.

Thank You
Your help keeps Hallows Eve fast, accessible, and adorable.
From our cauldron to yours: thanks for contributing! 🧪✨
