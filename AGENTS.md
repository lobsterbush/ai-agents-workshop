# AGENTS.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

Workshop materials for a 105-minute hands-on session teaching social scientists how to use AI agents (specifically Warp) for research workflows. Target audience: School of Social Sciences staff at Monash University.

## Structure

- `slides.html` - Reveal.js presentation (1920×1080, CDN-hosted dependencies)
- `prompt-cards.html` - Printable 2×3 grid of prompt cards for participants
- `PRESENTER_GUIDE.md` - Detailed timing guide and backup plans

## Development

### Viewing slides locally
Open `slides.html` directly in a browser. Requires internet connection for CDN resources:
- Reveal.js 4.5.0
- Google Fonts (Inter, JetBrains Mono)
- Animate.css

### Slide navigation
- Arrow keys to navigate
- `F` for fullscreen
- `S` for speaker notes
- `ESC` for slide overview

## Design Conventions

### Color Palette
- Background: `#0a0a0a`
- Surface: `#141414`
- Accent: `#d63031` (red, used sparingly)
- Text: `#f0f0f0` (primary), `#888` (secondary), `#555` (muted)

### Typography
- Headings: Inter 600, h1 at 3em, h2 at 1.8em
- Body: Inter 400 at 1.1em
- Code: JetBrains Mono at 0.75em
- Quotes: Newsreader italic at 1.6em

### Layout
- Resolution: 1920×1080
- Padding: 100px all sides
- Left-aligned text throughout
- Width constraints: `.narrow` (650px), `.medium` (800px)

### CSS Classes
- `.section` - part divider slides (bottom-aligned)
- `.center` - centered content slides
- `.terminal` - command-line mockups
- `.card`, `.grid-2`, `.grid-3` - card layouts
- `.callout`, `.callout-muted` - highlighted boxes
- `.numbered` - ordered lists with circular numbers
- `.compare`, `.compare-divider` - side-by-side layouts
- `.workflow`, `.workflow-step`, `.workflow-step.on` - process flows
- `.big-num`, `.timer` - large display numbers
- `.accent` - red accent color
- `.label` - small caps section labels

## Workshop Content Notes

The workshop demonstrates three live demos in Warp:
1. **Analyze & Report** - Survey data → OLS with clustered SEs → LaTeX table + coefficient plot → results paragraph
2. **Interactive Experiment** - Building a Twitter/X clone interface for survey experiments, embeddable in Qualtrics
3. **Complete Paper Section** - Raw experimental data → pre-registered analyses → tables/figures → methods + results → compiled PDF

The cold open builds a Qualtrics-importable conjoint experiment in ~14 seconds.

Key themes: workflow automation (not just task completion), reproducibility through logging, verification of all outputs.
