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

### Styling
- Primary color: Monash Blue (`#006DAE`)
- Accent colors: mint (`#4ECDC4`), coral (`#FF6B6B`), gold (`#FFE66D`)
- Progress bar enabled at bottom
- Resolution: 1920×1080

### Content patterns
Slides use these CSS classes:
- `.gradient-text` / `.gradient-text-warm` - gradient headings
- `.callout`, `.callout-warning`, `.callout-success`, `.callout-insight` - callout boxes
- `.terminal` - mock terminal displays
- `.fragment` - Reveal.js reveal animations

### Prompt cards
6 cards covering: Project Setup, Data Cleaning, Statistical Analysis, Visualization, Writing Assistance, Literature Review. Print double-sided, cut along grid.

## Workshop Content Notes

The workshop demonstrates three live demos in Warp:
1. **Project Setup** - Creating folder structures, READMEs, pre-registration templates
2. **Data Analysis** - Loading data, running regressions with clustered SEs, generating LaTeX tables
3. **Full Pipeline** - Qualitative coding of interview transcripts → codebook → visualization → methods paragraph

Key themes: reproducibility through logging, self-correcting agent behavior, verification of citations and statistics.
