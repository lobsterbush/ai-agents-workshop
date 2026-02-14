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
- Background: `#fafafa` (light)
- Text: `#1a1a1a` (primary), `#4a4a4a` (secondary), `#6a6a6a` (muted)
- Accent: `#0066cc` (blue)
- Green: `#4A9B67`
- Code blocks: `#1a1a1a` background, `#e8e8e8` text

### Typography
- Headings: Space Grotesk 600, h1 at 2.6em, h2 at 1.7em
- Body: Space Grotesk 400 at 1.1em
- Code: IBM Plex Mono at 0.7em

### Layout
- Resolution: 1920×1080
- Padding: 60px top/bottom, 80px sides
- Left-aligned text throughout
- Max paragraph width: 750px

### CSS Classes
- `.section` - part divider slides (bottom-aligned)
- `.center` - centered content slides
- `pre` - dark code blocks
- `.cols` - two-column comparison layouts
- `.stat` - large display numbers
- `.accent` - blue accent color
- `.label` - small caps section labels (IBM Plex Mono)
- `.dark` - dark background slides (for code demos)

## Workshop Content Notes

The workshop demonstrates three live demos in Warp:
1. **Experimental Design → Qualtrics** - Design a 2x2 vignette experiment on media trust, export as .qsf
2. **Data → Analysis → Results** - OLS with clustered SEs → coefficient plot → LaTeX table → results paragraph
3. **Interactive Experiment** - Building a Twitter/X clone interface for survey experiments, embeddable in Qualtrics

The cold open builds a complete "Partisan Bias in Scandal Evaluation" experiment in ~47 seconds:
- Title and abstract (LaTeX)
- Vignette text with randomization
- AsPredicted pre-registration
- R analysis script with estimatr/modelsummary

Key themes: workflow automation (not just task completion), reproducibility through logging, verification of all outputs.
