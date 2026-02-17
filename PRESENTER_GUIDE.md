# AI Agents for Social Science Research
## Presenter Guide — 105 Minutes

**Presenter:** Charles Crabtree  
**Audience:** School of Social Sciences staff, all levels  
**Date:** [Workshop Date]

---

## Pre-Workshop Checklist

- [ ] Test Warp.dev installation on presentation machine
- [ ] Pre-create demo project folder (so you have a backup if live demo fails)
- [ ] Have sample dataset ready (anonymized survey data)
- [ ] Test projector/screen resolution (slides are 1920×1080)
- [ ] Print prompt cards (6 per person)
- [ ] Set up shared Google Doc for discussion notes capture
- [ ] Test internet connection (slides use CDN-hosted fonts/libraries)

---

## Workshop Flow & Timings

### Part 0: Warp Setup (5 min)
**-0:05–0:00** (do this as people arrive)

| Slide | Time | Notes |
|-------|---------|-------|
| Download Warp | 1 min | "If you haven't already, go to warp.dev. It's free and takes 30 seconds." |
| Credits = Fuel | 1 min | Quick explanation. "75 credits/month on free tier. Plenty for today." |
| Pricing Plans | 30s | Show options briefly. "Build at $20/mo is great for power users." |
| Models Available | 1 min | "Warp works with Claude, GPT, and Gemini. We'll use 'auto' today." |
| Warp vs Competitors | 1.5 min | Quick landscape. "Claude Code, Codex are alternatives. Warp is model-agnostic." |

**Presenter note:** This section runs while people are still settling in. Keep it light and informational. The goal is to get everyone on the same page about what Warp is and how pricing works.

**Key talking points:**
- Credits are like fuel. Simple tasks = fewer credits. Complex tasks = more.
- Free tier (75 credits/month) is enough for occasional use
- Build plan ($20/mo) gives 1,500 credits and BYOK (Bring Your Own Key)
- BYOK lets you use your own OpenAI/Anthropic/Google API keys
- Warp supports multiple models: Claude Sonnet (default), Opus (planning), GPT-4o, Gemini
- We'll use "auto" mode today — it picks the best model for each task

---

### Part 1: Opening & Hook (10 min)
**0:00–0:10**

| Slide | Time | Notes |
|-------|------|-------|
| Title | 30s | Let people settle. Don't start talking immediately. |
| "Before we begin..." | 30s | Build anticipation. Pause for effect. |
| Cold open demo (terminal) | 2-3 min | **THIS IS THE HOOK.** Don't explain—just type the prompt and let them watch. Use fragments to reveal output step by step. |
| "45 minutes → 12 seconds" | 1 min | Let the number sink in. Dramatic pause before "12 seconds" reveal. |
| "What just happened?" | 2 min | Now explain. Chatbot vs Agent comparison. Key insight: agents *do*. |
| "Today's Journey" | 1 min | Quick roadmap. Don't dwell. |
| "Pulse Check" | 2 min | Get hands raised. Acknowledge skeptics—"You'll keep us honest." |

**Presenter note:** The cold open is everything. If you nail this, they're hooked. Practice this demo 10+ times so it's flawless.

---

### Part 2: The Mental Model (8 min)
**0:10–0:18**

| Slide | Time | Notes |
|-------|------|-------|
| Part 1 title | 15s | Brief transition |
| "The Evolution" | 2 min | Walk through chatbot → copilot → agent. Emphasize: "Agents ACT." |
| "Agents Have Tools" | 2 min | File system, terminal, web. "Anything you can do in a terminal..." |
| "The Agent Loop" | 2 min | Observe → Plan → Act → Reflect → Repeat. This is why they can handle complex tasks. |
| "Why This Matters for Research" | 1.5 min | Self-correcting, context-aware, end-to-end. These are the killer features. |

**Presenter note:** Don't over-explain here. The demos will make it concrete.

---

### Part 3: Live Demos (35 min)
**0:18–0:53**

#### Demo 1: Project Setup (10 min)
**0:18–0:28**

| Slide | Time | Notes |
|-------|------|-------|
| Demo 1 title | 30s | "Let's see this in action." |
| "What We'll Create" | 1 min | Show the tree structure. Set expectations. |
| 🎬 Live Demo | 7 min | **LIVE IN WARP.** Prompt: "Create a new survey experiment project called [topic] with folder structure, README, pre-registration template, ethics template, analysis scripts, and .gitignore." |
| Debrief | 1.5 min | "What used to take me 45 minutes... This is just the beginning." |

**Backup plan:** If demo fails, show pre-created project and narrate what happened.

#### Demo 2: Qualitative Analysis + Web App (15 min)
**0:28–0:43**

| Slide | Time | Notes |
|-------|------|-------|
| Demo 2 title | 30s | "Now for something different—real qualitative data." |
| Data source callout | 1 min | Explain QDR: "This is published, citable data. 25 interviews with South African politicians about representation." |
| The prompt | 1 min | Walk through the Braun & Clarke framework. "This is proper methodology, not just AI magic." |
| 🎬 Live Demo Part 1 | 5 min | **LIVE IN WARP.** Download transcripts, run thematic analysis, produce codebook. |
| Codebook output | 1 min | Show the themes. Discuss: "Would you code it the same way? That's reflexivity." |
| 🎬 Live Demo Part 2 | 4 min | **LIVE IN WARP.** Build the Thematic Explorer web app. |
| Web app output | 1.5 min | Demo the app: filter by theme, click participants, show co-occurrence. |

**Presenter note:** The web app is the wow moment. Building a custom research tool in minutes. If demo fails, open `examples/thematic_explorer.html` as backup.

**Key discussion point:** "AI can code data, but can it be reflexive about its own assumptions? That's where human judgment remains essential."

#### Demo 3: Interactive Experiment Interface (10 min)
**0:43–0:53**

| Slide | Time | Notes |
|-------|------|-------|
| Demo 3 title | 30s | "This is where it gets wild." |
| "One Prompt. Multiple Steps." | 1 min | Build anticipation with each fragment. |
| 🎬 Live Demo | 7 min | **LIVE IN WARP.** Build the Twitter/X interface for survey experiment. |
| "This is workflow, not task" | 1.5 min | Let the quote sink in. This is the paradigm shift. |

**Presenter note:** This is the jaw-dropper. Practice this one the most. Have a backup transcript ready.

---

### Part 4: Principles & Pitfalls (10 min)
**0:53–1:03**

| Slide | Time | Notes |
|-------|------|-------|
| Part 3 title | 15s | Transition |
| "Four Habits" | 4 min | Be specific, ask for explanations, verify, humans in loop. Give a quick example for each. |
| "Common Failure Modes" | 3 min | Hallucinated citations (!), plausible-but-wrong stats, overconfident code. "Trust but verify." |
| "Reproducibility Payoff" | 2.5 min | Everything is logged. This is your audit trail. Reviewers will love you. |

**Presenter note:** Be honest about limitations. Credibility comes from acknowledging what can go wrong.

---

### Part 5: Hands-On Sprint (20 min)
**1:03–1:23**

| Slide | Time | Notes |
|-------|------|-------|
| Part 4 title | 15s | "Your turn." |
| "Choose Your Level" | 2 min | Walk through all three options. Tell them: "Pick the one that slightly scares you." |
| Timer slide (14 min) | 14 min | Roam the room. Help people. Common issues: typos in prompts, not being specific enough. Celebrate early wins out loud. |
| "Quick Share-Out" | 3 min | 2-3 volunteers. "Show us what you got!" Applaud everything. Normalize when things go sideways. |

**Presenter note:** The sprint is where learning actually happens. Be generous with encouragement.

---

### Part 6: Group Discussion (20 min)
**1:23–1:43**

| Slide | Time | Notes |
|-------|------|-------|
| Part 5 title | 15s | "Let's zoom out." |
| "These tools are coming..." | 1 min | Frame the stakes. This is about shaping our field. |
| "Discussion Questions" | 2 min | Read each question. Give them 5 seconds to think before moving on. |
| Timer slide (12 min) | 12 min | Walk around. Listen to conversations. Take notes on good insights. |
| "Report Back" | 5 min | One insight per table. Capture key themes. "What I'm hearing is..." |

**Presenter note:** This discussion is gold for the post-workshop summary. Listen more than you talk.

---

### Part 7: Close (7 min)
**1:43–1:50**

| Slide | Time | Notes |
|-------|------|-------|
| "Three Things to Remember" | 2 min | 1. Agents act. 2. Verify always. 3. Document everything. |
| "Resources" | 1.5 min | Point to the download link. "Everything we talked about is there." |
| "What's Next?" | 1.5 min | Office hours, Slack, advanced workshop. Create pathways for continued engagement. |
| Thank You | 2 min | Contact info. Pause for final questions. End strong. |

---

## Demo Prompts (Copy-Paste Ready)

### Demo 1: Project Setup
```
Create a new survey experiment project called "immigration-attitudes" with:
- Folder structure for data (raw/processed), analysis, output (tables/figures), and ethics
- README with project overview, folder explanations, and how to reproduce
- Pre-registration template in AsPredicted format
- Ethics application template
- Starter R scripts for cleaning and analysis
- .gitignore configured for R projects
```

### Demo 2: Qualitative Analysis + Web App
```
Analyze these 25 interview transcripts about political representation in South Africa (QDR doi:10.5064/F6L9HHYL).

Using Braun & Clarke's reflexive thematic analysis:
1. Familiarize yourself with the data
2. Generate initial codes inductively
3. Search for themes—group codes into potential themes
4. Review themes against data extracts
5. Define and name themes

Produce a codebook, coded data CSV, and theme visualization using ggplot with theme_tufte().
```

Then immediately follow with:
```
Build a web app called "Thematic Explorer" to help researchers explore these coded transcripts.

Features:
- Dashboard showing theme frequency across all 25 interviews
- Filter by theme to see all supporting quotes
- Click a participant to see their full coded transcript
- Theme co-occurrence matrix (which themes appear together?)
- Export filtered data to CSV
- Dark/light mode toggle

Use vanilla HTML/CSS/JS. Make it professional and intuitive.
```

### Demo 3: Interactive Experiment Interface
```
Build a Twitter/X interface for a survey experiment.

- Feed of 8 posts about climate change (mix of accurate/misinformation)
- Users can like, retweet, reply, and scroll
- Track all engagement with timestamps
- Randomize post order and treatment conditions
- Make it embeddable in Qualtrics via iframe
- Log data to CSV on completion
```

---

## Troubleshooting Common Issues

| Issue | Solution |
|-------|----------|
| Warp not connecting | Check internet. Use mobile hotspot as backup. |
| Agent taking too long | Explain: "It's thinking through the steps." Use the time to narrate. |
| Agent makes error | Say: "Watch—it's going to notice and self-correct." |
| Participant can't install Warp | Have them pair with a neighbor who has it working. |
| Slides not loading fonts | Use backup local copy of slides. |
| No projector | Present from laptop with people gathered around (intimate workshop mode). |

---

## Post-Workshop

- [ ] Email participants within 48 hours with:
  - Link to resource packet
  - Summary of discussion insights
  - Office hours schedule
  - Feedback survey link
- [ ] Share anonymized discussion notes with SoSS leadership
- [ ] Update slides based on what worked/didn't
- [ ] Plan advanced workshop based on demand

---

## Resource Packet Contents (bit.ly/soss-ai-agents)

1. **Prompt Cards (PDF)** — 6 cards covering:
   - Project setup
   - Data cleaning
   - Statistical analysis
   - Visualization
   - Writing assistance
   - Literature review

2. **Workflow Templates** — Pre-built project structures for:
   - Survey experiments
   - Interview studies
   - Secondary data analysis
   - Mixed methods projects

3. **Example Datasets** — Anonymized CSVs for practice

4. **Troubleshooting Guide** — Common Warp issues and solutions

5. **Reading List** — Papers on AI in research workflows

---

*Remember: The goal isn't to make them experts today. It's to show them what's possible and give them a starting point. The wow moment comes from seeing it work. Everything else is context.*
