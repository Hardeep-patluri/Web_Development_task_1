# Web_Development_task_1
# Ember & Oak — Responsive Landing Page

A clean, responsive landing page built for a fictional small-batch coffee
roastery, created as a practice project for learning HTML5, CSS Flexbox/Grid,
and media queries.

## Objective

Build a responsive landing page with a header, hero section, and footer using
only HTML and CSS — no frameworks, no JavaScript.

## Tools Used

- **VS Code** — code editor
- **Live Server extension** — local development server with auto-reload
- **Chrome DevTools** — used to test responsiveness at different screen sizes

## Project Structure

```
├── index.html   # Page markup
├── style.css    # All styling, layout, and responsiveness
└── README.md
```

HTML and CSS are kept in separate files, linked via a `<link>` tag in the
`<head>` of `index.html`.

## Features

- **Header** — logo and nav links laid out with Flexbox (`justify-content:
  space-between`); nav wraps and re-centers below the logo on small screens.
- **Hero section** — heading, supporting paragraph, and a call-to-action
  button, laid out as a two-column CSS Grid that collapses to a single column
  on tablet-sized screens.
- **Signature visual** — a hand-drawn-style coffee cup built with inline SVG,
  with a subtle animated steam effect (disabled automatically for users with
  `prefers-reduced-motion` set).
- **Menu and About sections** — additional content blocks demonstrating a
  3-column CSS Grid that reflows to 2 columns, then 1, as the screen narrows.
- **Footer** — centered layout with social links, built with Flexbox.
- **Responsive breakpoints**:
  - `860px` — hero switches from 2 columns to 1; menu grid drops to 2 columns.
  - `600px` — header nav collapses to a centered, wrapped row; menu grid
    drops to 1 column.

## Design Notes

- **Color palette**: warm espresso-brown background with copper and sage
  accents, chosen to fit the coffee-roastery theme rather than a generic
  template palette.
- **Typography**: `Fraunces` (serif) for headings paired with `Work Sans`
  (sans-serif) for body text and navigation, loaded via Google Fonts.
- All colors, fonts, and spacing values are defined once as CSS custom
  properties (`:root` variables) at the top of `style.css` for easy tweaking.

## How to Run

1. Open the project folder in VS Code.
2. Right-click `index.html` and select **Open with Live Server**.
3. The page opens in Chrome at `http://127.0.0.1:5500` (or similar).
4. Resize the browser window (or use Chrome DevTools' device toolbar) to test
   responsiveness at desktop, tablet, and mobile widths.

## Possible Next Steps

- Add a hamburger menu with JavaScript for an even more compact mobile nav.
- Replace the SVG illustration with real product photography.
- Add scroll-triggered animations for the Menu and About sections.
