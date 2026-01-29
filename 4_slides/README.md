# Tutorial Slides & Video

## Final Assets

| Asset | Link |
|:------|:-----|
| **Google Slides** | [PM Claude Code Tutorial](https://docs.google.com/presentation/d/1mh7uzy2-RCQKt3H0W_l_ZSr7dRlhF2HcGB73N4IPafU/edit?usp=sharing) |
| **Video** | [Tutorial Video](https://docs.google.com/videos/d/1K_QM0viGAfKkscE1kLrkFyJLUD_OqcprlZUuDcX5vds/edit?usp=sharing) |

---

## How to Replicate This Process

### Step 1: Generate Slides with Claude Cowork

1. Go to [claude.ai](https://claude.ai)
2. Start new conversation
3. Paste this prompt:

```
Create a 16-slide PPTX presentation for MIT Sloan MBA students titled
"PM Prototyping with Claude Code & GitHub" for Spring 2026 Product Management class.

AUDIENCE: Code novices who have never used terminal or GitHub.

SLIDES:
1. Title - "PM Prototyping with Claude Code & GitHub", subtitle "No coding required"
2. Project Goal - Create working prototype, deliverable = public GitHub repo
3. Why This Matters - Writing-first → Building-first PM shift
4. Do I Need Coding Skills? - Giant "NO", Claude Code writes code from English
5. Your Two Tools - Claude Code (AI engineer) + GitHub (code storage)
6. Prerequisites - Node.js, Git, GitHub account, Claude Code install
7. Account Options - Claude Max ($20/mo) vs API Credits ($5 free)
8. 5-Step Workflow - Setup → Create → Push → Iterate → Update
9. Step 1: Setup - Terminal basics, mkdir/cd/claude commands
10. Step 2A: Describe - Good prompt structure with example
11. Step 2B: Run Locally - npm install, npm run dev, localhost:5173
12. Step 3: Push - git init, create GitHub repo, push
13. Step 4: Iterate - Plain English change requests
14. Step 5: Commit - git add/commit/push workflow
15. Final Checklist - Public repo, code pushed, app runs
16. Troubleshooting - Common errors table + TA contact

Include terminal mockup screenshots. Use navy blue (#1a365d) as primary color.
```

4. Claude Cowork generates PPTX with screenshots
5. Download the PPTX file

### Step 2: Upload to Google Slides

1. Go to [Google Slides](https://slides.google.com)
2. File → Import slides → Upload PPTX
3. Select all slides → Import
4. Review and adjust formatting if needed

### Step 3: Export as Video

1. In Google Slides: File → Download → Microsoft PowerPoint
2. Or use: File → Share → Publish to web → Link
3. For video with narration: Use Loom or screen recording while presenting

---

## Slide Content Summary

| # | Title | Key Content |
|:-:|:------|:------------|
| 1 | Title | "No coding experience required" |
| 2 | Project Goal | Working prototype → GitHub repo |
| 3 | Why This Matters | "PMs can now SHOW, not just tell" |
| 4 | Coding Skills? | **NO** - Claude writes code from English |
| 5 | Two Tools | Claude Code + GitHub |
| 6 | Prerequisites | Node.js (LTS), Git, GitHub, Claude Code |
| 7 | Account Options | Max $20/mo OR API $5 free credit |
| 8 | Workflow | 5 circular steps |
| 9 | Step 1 | `mkdir my-app && cd my-app && claude` |
| 10 | Step 2A | Detailed prompt → better results |
| 11 | Step 2B | `npm run dev` → localhost:5173 |
| 12 | Step 3 | Ask Claude to init git + push |
| 13 | Step 4 | "Add delete button to each card" |
| 14 | Step 5 | "Commit and push with message..." |
| 15 | Checklist | Public ✓ Pushed ✓ Runs ✓ |
| 16 | Troubleshooting | npm/git/claude not found → solutions |

---

## Tools Used

| Tool | Purpose | Time |
|:-----|:--------|:----:|
| Claude Cowork | Generate PPTX + screenshots | 5 min |
| Google Slides | Host + minor edits | 5 min |
| Google Slides Video | Export to video | 2 min |

**Total production time**: ~12 minutes

---

## Design Specifications

- **Primary**: Navy blue (#1a365d)
- **Accent**: MIT Red (#A31F34) optional
- **Background**: White
- **Code blocks**: Dark theme with syntax highlighting
- **Font**: Sans-serif, readable at distance

---

*Created January 2026 for MIT Sloan Product Management course*
*Process: Claude Cowork → PPTX → Google Slides → Video*
