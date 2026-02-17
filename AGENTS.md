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

### Additional CSS Classes (v4)
- `.era-slide` - full-screen background image slides (computing history, IT screenshots)
- `.era-label` - overlay label with backdrop blur for era slides
- `.section-bg` - section dividers with background images
- `.section-fail` - dark section divider with red accent (Part 3: Where They Fail)
- `.cost-grid` / `.cost-item` / `.cost-arrow` - equilibrium cost visualization
- `.value-arrow` - blue up-arrow for "what gains value" items
- `.timer` - clickable countdown timer (click to start, click again to reset)

## Workshop Content Notes

### Slide Flow
Title → About Me → AI Credentials → "I was a skeptic" → Today (roadmap) → Computing History (5 era slides) → "New OS is language" → Installation section → IT conversation screenshots (6 slides) → Download Warp → Credits → Pricing → Models → Competitors → "You direct the agent" → Cold open (populism) → Output slides → ~60 seconds → "This isn't the ChatGPT you know" → Part 1 (How Agents Work) → Part 2 (Three Demos) → Part 3 (Where They Fail) → Verification → Prototyping → Part 4 (Hands-On) → Prompt Cards 1–3 → Challenges → Timer → Share → Part 5 (Implications) → Equilibrium → Discussion → Timer → Summary → Resources → Thank You

### Three Live Demos
1. **Forgotten Survey Data → Full Paper** - TKFD Asia comparative survey project (China, Korea, Taiwan). Explores `~/Dropbox/tkfd/surveys/asia` — immigration, masculinity, COVID-19, security, refugees data. Models with robust SEs, ggplot figures, LaTeX tables, paper draft with guardrails.
2. **Interview Transcripts → Thematic Explorer** - QDR South Africa political representation interviews. Braun & Clarke reflexive thematic analysis producing 7-theme codebook (2 slides), coded data CSV, and an expansive web app with dashboard (frequency charts, co-occurrence matrix, quote density heatmap) and explorer (quote browser, participant comparison, keyword search, CSV export).
3. **Interactive Experiment** - Building a Twitter/X clone interface for survey experiments, embeddable in Qualtrics

### Cold Open
Re-analyzes a forgotten populism survey dataset (~60 seconds):
- Data exploration (500+ variables, Argentina sample)
- Populism index construction
- Predictor models with robust SEs
- Immigration conjoint AMCEs with clustered SEs
- Publication-ready figures and LaTeX output

### Installation Sequence
Before the Warp setup slides, there are 6 screenshots (`images/it-1.png` through `it-6.png`) showing a conversation with IT about installing Warp, preceded by a dark "Installation" section divider.

### Prompt Cards
3 scenarios, inlined in slides (unchanged):
1. Project management — entering an old/unfamiliar project directory
2. Quantitative analysis — re-analyzing old/forgotten data
3. Survey instrument — creating a survey with validated scales and experimental treatments

### Timers
Two countdown timers (14 min work session, 12 min discussion). Click to start, click again to reset. JS uses `stopPropagation()` to avoid Reveal.js click interference. Colors: green → amber (≤2 min) → red (expired, pulsing).

Key themes: workflow automation (not just task completion), interacting with and directing agents, rapid prototyping/iteration, reproducibility through logging, verification of all outputs.
