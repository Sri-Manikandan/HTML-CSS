# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

A collection of standalone HTML/CSS exercise tasks. No build tools, package manager, or JavaScript framework — each task is a self-contained `index.html` + CSS file that opens directly in a browser.

## Viewing tasks

Open any task directly in a browser:

```
open task1/index.html
open task2/index.html
# etc.
```

There is no build step, dev server, or test runner.

## Task summary

| Task | Description | Key technique |
|------|-------------|---------------|
| task1 | Full static webpage (header, hero, cards, footer) | Responsive layout with `@media` breakpoints (768px, 480px) |
| task2 | Single card component | CSS hover effects (`transform`, `box-shadow`, `filter`) |
| task3 | Responsive card grid | CSS Grid with `auto-fill`/`minmax` |
| task4 | Navigation with dropdowns | Pure CSS dropdowns; mobile hamburger via checkbox hack |
| task5 | Modal popups | Pure CSS modals via `:target` pseudo-class — no JavaScript |

## CSS conventions

- **BEM naming** (task2 onward): `.block__element--modifier` — e.g., `.card__image`, `.nav__item--dropdown`
- **Box-sizing reset** in every file: `*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }`
- **CSS file name**: task1 uses `styles.css`; tasks 2–5 use `style.css`
- Accent color in task1: `#e94560` (red); task2: `#4a6cf7` (blue) — each task has its own palette
- Transitions use `ease` or `ease-in-out` at 0.25–0.3s
