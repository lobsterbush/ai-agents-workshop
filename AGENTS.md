# AGENTS.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

Workshop materials for a 105-minute hands-on session teaching social scientists how to use AI agents (specifically Warp) for research workflows. Target audience: School of Social Sciences staff at Monash University.

## Structure

- `slides.html` - Reveal.js presentation (1920×1080, CDN-hosted dependencies)
- `prompt-cards.html` - Printable prompt cards (3 scenarios: project management, quantitative analysis, survey instrument)
- `PRESENTER_GUIDE.md` - Detailed timing guide and backup plans

## Development

### Viewing slides locally
Open `slides.html` directly in a browser. Requires internet connection for CDN resources:
- Reveal.js 4.5.0
- Google Fonts (Space Grotesk, IBM Plex Mono)

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
- Headings: Space Grotesk 600, h1 at 2.4em, h2 at 1.6em
- Body: Space Grotesk 400 at 1em
- Code: IBM Plex Mono at 0.7em

### Layout
- Resolution: 1920×1080
- Padding: 60px top/bottom, 80px sides
- Left-aligned text throughout
- Max paragraph width: 1100px
- Center slides: max 850px
- Graph paper background (blue grid pattern from charlescrabtree.org)
- Subtle radial gradient overlays (blue/green)

### CSS Classes
- `.section` - part divider slides (bottom-aligned)
- `.center` - centered content slides
- `pre` - dark code blocks
- `.cols` - two-column comparison layouts
- `.stat` - large display numbers
- `.accent` - blue accent color
- `.label` - small caps section labels (IBM Plex Mono)
- `.dark` - dark background slides (for code demos)
- `.callout` - blue accent callout boxes
- `.card` - white card with subtle border/shadow

## Workshop Content Notes

The workshop demonstrates three live demos in Warp:
1. **Data Analysis → Publication-Ready Output** - Conjoint analysis with AMCEs, coefficient plot, LaTeX table, results paragraph
2. **Interview Transcripts → Thematic Analysis** - Qualitative coding with inductive codebook, theme visualization
3. **Interactive Experiment** - Building a Twitter/X clone interface for survey experiments, embeddable in Qualtrics

The cold open re-analyzes a forgotten populism survey dataset (~60 seconds):
- Data exploration (500+ variables, Argentina sample)
- Populism index construction
- Predictor models with robust SEs
- Immigration conjoint AMCEs with clustered SEs
- Publication-ready figures and LaTeX output

Prompt cards (3 scenarios, also inlined in slides):
1. Project management — entering an old/unfamiliar project directory
2. Quantitative analysis — re-analyzing old/forgotten data
3. Survey instrument — creating a survey with validated scales and experimental treatments

Key themes: workflow automation (not just task completion), interacting with and directing agents, rapid prototyping/iteration, reproducibility through logging, verification of all outputs.
