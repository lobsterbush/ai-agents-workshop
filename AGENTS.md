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
- Background: near-black (`#0c0c0c`)
- Surface: dark gray (`#161616`)
- Accent: vermillion red (`#e34234`) - used sparingly
- Text: white (`#fafafa`), secondary (`#a1a1a1`), muted (`#6b6b6b`)
- No gradients, no stock photos, no emojis

### Typography
- Headings: Inter (weight 600-700)
- Body: Inter (weight 400)
- Code: JetBrains Mono
- Accent serif: Playfair Display (for quotes)

### Layout
- Resolution: 1920×1080
- Padding: 80px top/bottom, 120px sides
- Left-aligned text (not centered)
- Content width constraints: `.content-narrow` (800px), `.content-medium` (1000px), `.content-wide` (1400px)

### CSS Classes
- `.section-title` - part divider slides (bottom-aligned)
- `.center-slide` - centered content slides
- `.terminal` - command-line mockups
- `.card`, `.card-grid`, `.card-grid-3` - information cards
- `.callout`, `.callout-subtle` - highlighted information
- `.numbered-list` - ordered lists with circular numbers
- `.vs-grid`, `.vs-divider` - comparison layouts
- `.workflow`, `.workflow-step` - process flows
- `.accent` - red accent color for emphasis
- `.serif` - italic Playfair for editorial emphasis

## Workshop Content Notes

The workshop demonstrates three live demos in Warp:
1. **Research Dashboard** - Building an interactive Shiny app from WVS data with filters and map visualization
2. **Full Analysis Pipeline** - Raw data → clustered SE regressions → LaTeX tables/figures → methods text → compiled PDF
3. **Interactive Experiment** - Building a Twitter/X clone interface for survey experiments, embeddable in Qualtrics

The cold open builds a Qualtrics-importable conjoint experiment in ~14 seconds.

Key themes: workflow automation (not just task completion), reproducibility through logging, verification of all outputs.
