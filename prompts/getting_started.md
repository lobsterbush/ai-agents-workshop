# Getting Started with Warp

A quick-start guide for first-time users of the Agentic Development Environment.

---

## 1. Download & Install

**Website:** [warp.dev](https://warp.dev)

| Platform | Installation |
|----------|--------------|
| macOS | Download `.dmg`, drag to Applications |
| Windows | Download `.exe`, run installer |
| Linux | Download `.deb` or use package manager |

**Time:** ~30 seconds

---

## 2. Create Your Account

1. Open Warp
2. Sign up with **email** or **GitHub**
3. No credit card required for free tier
4. Complete brief onboarding (optional)

---

## 3. Understand Credits

### Credits = Fuel for AI Operations

Every AI request uses credits. Think of them like fuel:

| Task Type | Credit Usage |
|-----------|--------------|
| Simple commands | Low (1-5 credits) |
| Code explanations | Medium (5-15 credits) |
| Multi-file edits | Higher (15-50 credits) |
| Complex planning | Highest (50+ credits) |

### Free Tier Limits
- **First 2 months:** 150 credits/month
- **After:** 75 credits/month
- Terminal features always free

### Need More?
- **Build Plan:** $20/mo → 1,500 credits + BYOK
- **Reload Credits:** Purchase extra, roll over 12 months

---

## 4. Choose Your Model

Click the model name in the input bar to switch. Available options:

### Anthropic Claude (Default Provider)
- **Claude Sonnet 4.5** — Best balance of speed and quality *(recommended)*
- **Claude Opus 4.5** — Most capable, best for complex reasoning
- **Claude Haiku** — Fastest, cheapest, good for simple tasks

### OpenAI
- **GPT-4o** — General purpose, multimodal

### Google
- **Gemini 2.5 Pro** — Alternative for certain tasks

### Auto Mode (Recommended)
Select **"auto"** to let Warp choose the best model for each task. Uses Sonnet for execution and Opus for planning.

---

## 5. Your First Prompts

### Prompt 1: Learn About Your Project
```
What files are in this directory? Give me a brief overview of the project structure.
```

### Prompt 2: Explain Code
```
Explain what the main function does in @main.py
```
*Tip: Use `@` to reference files directly*

### Prompt 3: Create a Simple File
```
Create a README.md for this project with:
- Project title
- Brief description
- Installation instructions
- How to run
```

### Prompt 4: Fix an Error
```
I'm getting this error when I run my code:
[paste error message]

Read the relevant files and fix the issue.
```

### Prompt 5: Refactor Code
```
Refactor @utils.py to be more readable. Add docstrings and type hints.
```

---

## 6. Key Features to Try

### Universal Input (`@` mentions)
Type `@` in the input to:
- Reference files: `@src/main.py`
- Attach images (drag and drop)
- Include URLs

### WARP.md / AGENTS.md
Create a `WARP.md` file in your project root to give the agent persistent context:
```markdown
# Project Context

This is a Python data analysis project using pandas and matplotlib.

## Conventions
- Use type hints
- Follow PEP 8
- All plots use theme_tufte()

## Key Files
- data/raw/ — raw data files
- src/analysis.py — main analysis script
```

### Autonomy Levels
Adjust how much the agent can do without asking:
- **Suggest** — Agent suggests, you approve everything
- **Auto-edit** — Agent can edit files, asks before commands
- **Full auto** — Agent works independently (use with caution)

Settings → AI → Agents → Profiles

---

## 7. Credit-Saving Tips

1. **Use Haiku for simple tasks** — explanations, quick questions
2. **Be specific** — vague prompts require more back-and-forth
3. **Use `@` mentions** — pointing to files is cheaper than asking agent to search
4. **Batch related tasks** — one detailed prompt > multiple small ones
5. **Set up WARP.md** — reduces context-building on each request

---

## 8. Comparison: Warp vs Alternatives

| Feature | Warp | Claude Code | OpenAI Codex |
|---------|------|-------------|--------------|
| **Models** | Claude, GPT, Gemini | Claude only | GPT only |
| **Interface** | Terminal-native | Terminal, IDE, web | Terminal, IDE, web |
| **Free tier** | Yes (75 credits) | No | ChatGPT Plus required |
| **BYOK** | Yes ($20/mo plan) | No | API key required |
| **Context files** | WARP.md | CLAUDE.md | AGENTS.md |

### When to Use Each

**Warp** — Model flexibility, terminal power users, cost-conscious
**Claude Code** — Deep Anthropic integration, Agent Teams, iOS access
**OpenAI Codex** — GPT-5 access, cloud sandbox tasks, existing ChatGPT users

---

## 9. Troubleshooting

### "I ran out of credits"
- Check Settings → Billing
- Purchase Reload Credits or upgrade to Build plan
- Or: Add your own API key (BYOK) on paid plans

### "The agent isn't understanding my project"
- Create a `WARP.md` file with project context
- Use `@` to point to relevant files
- Be more specific in your prompts

### "The agent made a mistake"
- Use `Cmd/Ctrl + Z` to undo file changes
- Or: Type "undo that" and explain what went wrong
- The agent can correct itself

### "How do I switch models?"
- Click the model name in the input bar
- Or: Go to Settings → AI → Default Model

---

## 10. Resources

- **Documentation:** [docs.warp.dev](https://docs.warp.dev)
- **Pricing:** [warp.dev/pricing](https://warp.dev/pricing)
- **Support:** [email protected]
- **Community:** [discord.gg/warp](https://discord.gg/warp)

---

## Quick Reference Card

```
┌─────────────────────────────────────────────────────────────┐
│  WARP QUICK REFERENCE                                       │
├─────────────────────────────────────────────────────────────┤
│  @ + filename    Reference a file                           │
│  Cmd/Ctrl + K    Open AI input                              │
│  Cmd/Ctrl + Z    Undo agent's changes                       │
│  /model          Switch model mid-conversation              │
│                                                             │
│  MODELS                                                     │
│  auto       →  Best for most tasks (recommended)            │
│  sonnet     →  Fast, balanced                               │
│  opus       →  Complex reasoning, planning                  │
│  haiku      →  Quick, cheap                                 │
│  gpt-4o     →  OpenAI alternative                           │
│                                                             │
│  CREDITS (Free tier: 75/month)                              │
│  Simple task    ~5 credits                                  │
│  Medium task    ~20 credits                                 │
│  Complex task   ~50+ credits                                │
└─────────────────────────────────────────────────────────────┘
```
