# Qualitative Analysis Prompt Templates

Ready-to-use prompts for AI-assisted qualitative research. Adapt these to your own data and research questions.

---

## 🎯 Starter: Basic Thematic Analysis

**Use when:** You have interview transcripts and want to identify themes.

```
Analyze these interview transcripts about [YOUR TOPIC].

Using Braun & Clarke's reflexive thematic analysis:
1. Familiarize yourself with the data
2. Generate initial codes inductively  
3. Search for themes—group codes into potential themes
4. Review themes against data extracts
5. Define and name themes

Produce:
- A codebook with theme names, definitions, and example quotes
- A CSV of coded quotes (participant, theme, quote, line number)
- A bar chart of theme frequencies
```

---

## 🔬 Standard: Full Analysis Pipeline

**Use when:** You want publication-ready outputs.

```
Analyze the [NUMBER] interview transcripts in [FOLDER PATH] about [TOPIC].

Phase 1 - Analysis:
1. Read all transcripts carefully
2. Develop an inductive codebook using reflexive thematic analysis
3. Code each transcript, noting participant ID and line numbers
4. Calculate theme frequencies and co-occurrence patterns

Phase 2 - Outputs:
1. codebook.md - Themes with definitions, examples, and prevalence
2. coded_data.csv - All coded quotes with metadata
3. theme_frequencies.png - Bar chart using ggplot2 + theme_tufte()
4. methods_paragraph.tex - Describe the analytical approach

Be explicit about your interpretive decisions. Flag any ambiguous codes.
```

---

## 🚀 Advanced: Thematic Explorer Web App

**Use when:** You want an interactive tool to explore your coded data.

```
Build a web app called "Thematic Explorer" to explore these coded transcripts.

Features:
- Dashboard showing theme frequency across all interviews
- Filter by theme to see all supporting quotes
- Click a participant to see their full coded transcript
- Theme co-occurrence matrix (which themes appear together?)
- Export filtered data to CSV
- Dark/light mode toggle

Use vanilla HTML/CSS/JS in a single file. Make it professional and intuitive.
Include the coded data from our analysis.
```

---

## 📊 Visualization-Focused

**Use when:** You need publication-ready figures.

```
Create visualizations for my thematic analysis of [TOPIC]:

1. Theme frequency bar chart
   - Horizontal bars, sorted by frequency
   - Clean labels, no gridlines
   - Color-coded by theme category

2. Theme co-occurrence heatmap
   - Show how often themes appear together
   - Use sequential color scale
   - Include counts in cells

3. Participant × Theme matrix
   - Show which themes each participant discussed
   - Use dots or checkmarks for presence

Use ggplot2 with theme_tufte(). Export as PNG at 300 DPI.
Save source data as CSV for reproducibility.
```

---

## 📝 Writing-Focused

**Use when:** You need to draft results sections.

```
Based on the coded transcripts and codebook, draft a results section for a qualitative paper on [TOPIC].

Structure:
1. Overview paragraph describing the analytical approach
2. One subsection per major theme, including:
   - Theme definition and prevalence (N participants, N quotes)
   - 2-3 illustrative quotes with participant pseudonyms
   - Interpretation connecting to research question
3. Brief discussion of theme relationships

Style: Academic social science, past tense, third person.
Length: Approximately [X] words.

Include inline LaTeX macros for all statistics (e.g., \nparticipants{}).
```

---

## 🔍 Verification Prompt

**Use when:** You want to check AI coding against your own interpretation.

```
I've coded these transcripts myself. Compare my coding to your analysis:

My themes:
1. [THEME 1] - [Your definition]
2. [THEME 2] - [Your definition]
3. [THEME 3] - [Your definition]

For each quote I coded, tell me:
- Whether you agree with my theme assignment
- Alternative themes you might consider
- Any quotes I may have missed

Be critical. Disagreement is valuable for reflexivity.
```

---

## 💡 Tips for Effective Prompts

### Be Specific About Methodology
❌ "Analyze these interviews"  
✅ "Using Braun & Clarke's reflexive thematic analysis, analyze these interviews"

### Specify Output Formats
❌ "Create a codebook"  
✅ "Create a codebook in markdown with theme name, definition, example quotes, and prevalence"

### Request Transparency
Include phrases like:
- "Be explicit about your interpretive decisions"
- "Flag any ambiguous codes"
- "Note where multiple themes could apply"

### Maintain Reflexivity
Always follow up with:
- "Would I code this the same way?"
- "What assumptions is the AI making?"
- "Are there quotes the AI missed that I would include?"

---

## 🎓 Methodological Reference

### Braun & Clarke's Six Phases of Reflexive TA

1. **Familiarization** — Read and re-read data, note initial ideas
2. **Generating codes** — Systematically code interesting features
3. **Searching for themes** — Collate codes into potential themes
4. **Reviewing themes** — Check themes against data extracts and full dataset
5. **Defining themes** — Refine specifics, generate clear names and definitions
6. **Writing up** — Final analysis with vivid, compelling extract examples

### Key Principles

- **Themes are constructed, not discovered** — You are an active participant in meaning-making
- **Reflexivity is essential** — Document your assumptions and interpretive choices
- **Quality over quantity** — A theme doesn't need to appear in X% of data to be valid
- **Thick description** — Rich, contextualized quotes are more valuable than frequency counts

### Recommended Reading

- Braun, V. & Clarke, V. (2006). Using thematic analysis in psychology. *Qualitative Research in Psychology*, 3(2), 77-101.
- Braun, V. & Clarke, V. (2022). *Thematic Analysis: A Practical Guide*. SAGE.
- https://www.thematicanalysis.net/

---

## 📁 Example Data Source

**Perspectives on Political Representation**  
QDR DOI: [10.5064/F6L9HHYL](https://doi.org/10.5064/F6L9HHYL)

25 semi-structured interviews with South African elected representatives exploring:
- Pressure to represent associated identity groups
- Tensions between descriptive and substantive representation
- Trust-building strategies across constituencies

This is published, citable data — ideal for practicing qualitative analysis workflows.
