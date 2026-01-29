---
modified:
  - 2026-01-28T21:47:44-05:00
---
# 🤜 Doability Score Comparison

> **Evaluator Perspective**: Novice MBA student in MIT Product Management course (Prof. Charlie Fine)
> **Task**: Follow video instructions to build a working prototype using Lovable, GitHub, and Cursor
> **Success Criteria**: Complete the exercise from start to GitHub submission without external help

---

## 📊 Evaluation Criteria

| Criterion | Weight | What We're Measuring |
|:----------|:------:|:---------------------|
| **Prerequisites Clear** | 20% | Are required installations (Node.js, Git, accounts) listed upfront? |
| **Steps Numbered** | 15% | Can I follow a clear 1-2-3 sequence? |
| **Commands Explicit** | 20% | Are terminal commands shown exactly as I should type them? |
| **Error Handling** | 15% | Does it tell me what to do when something fails? |
| **No Confusion** | 15% | Are there fumbles, corrections, or confusing moments? |
| **Time Respect** | 15% | Does it get to the point without tangents? |

---

## 🎬 Version 1: Original (30 minutes)

**Source**: `30min_video.md`

### Scores

| Criterion | Score | Evidence |
|:----------|:-----:|:---------|
| Prerequisites Clear | 2/10 | Git mentioned at minute 23, Node.js **never** mentioned |
| Steps Numbered | 4/10 | Workflow explained verbally but buried in prose |
| Commands Explicit | 6/10 | Commands shown but with typo ("misspelled origin") |
| Error Handling | 1/10 | "Explain how to install Git?" left hanging, no troubleshooting |
| No Confusion | 3/10 | Logo fumble (~1 min), Lovable/Cursor mixup, "Sorry, it didn't work" |
| Time Respect | 4/10 | Extended MVP→MLP explanation, waiting in real-time, GitHub tour |

### 🤜 Original Score: **3.3/10**

### Novice Experience
> *"I got to `npm install` and it said 'command not found'. The video never told me I needed Node.js. I spent 30 minutes watching but I'm stuck at minute 11. The instructor fumbled with the logo URL and I don't know if I should copy his mistakes or not."*

### Blockers for Completion
1. ❌ `npm` command fails (Node.js not installed)
2. ❌ `git push` fails (Git not installed)
3. ❌ Confused by logo correction sequence
4. ❌ No guidance when things go wrong

---

## 🎬 Version 2: Charlie's Version (15 minutes)

**Source**: `🧑‍🏫15min_video_charlie.md`

### Scores

| Criterion | Score | Evidence |
|:----------|:-----:|:---------|
| Prerequisites Clear | 3/10 | Git mentioned at [08:35], Node.js still missing |
| Steps Numbered | 7/10 | Clear timestamps, section headers (Step 1, Step 2...) |
| Commands Explicit | 7/10 | Commands listed with explanations |
| Error Handling | 2/10 | Still no troubleshooting section |
| No Confusion | 5/10 | Logo correction kept: "it put it on the right, I wanted left" |
| Time Respect | 7/10 | Tighter pacing, but still shows wait time, keeps mistakes |

### 🤜 Charlie's Score: **5.2/10**

### Novice Experience
> *"Much better organized—I can see the sections. But I still hit 'npm not found' and had to Google it. The logo back-and-forth made me unsure if making mistakes is part of the process. I finished, but it took me 2 hours with troubleshooting."*

### Blockers for Completion
1. ⚠️ `npm` still fails initially (but Googleable)
2. ✅ Git mentioned (though late)
3. ⚠️ Confusion from watching mistakes play out
4. ❌ No guidance when things go wrong

---

## 🎬 Version 3: Angie's Descript Edit (19 minutes)

**Source**: `👩‍🏫15min_video_angie.md`

### Scores

| Criterion | Score | Evidence |
|:----------|:-----:|:---------|
| Prerequisites Clear | 3/10 | Git mentioned at [08:00], Node.js still missing |
| Steps Numbered | 6/10 | Timestamps present, workflow at [03:00] is numbered list |
| Commands Explicit | 8/10 | Commands formatted as code blocks with syntax highlighting |
| Error Handling | 2/10 | No troubleshooting, but cleaner flow |
| No Confusion | 4/10 | Logo fumble still present [13:00-15:00] |
| Time Respect | 6/10 | 19 min (saved 11 min), but still includes corrections |

### 🤜 Angie's Score: **4.8/10**

### Novice Experience
> *"The formatting is cleaner and I can see the commands clearly. But I still hit the npm error—wish there was a prerequisites checklist at the start. The logo section still shows the mistake happening. Better than the original, but still had to troubleshoot."*

### Blockers for Completion
1. ⚠️ `npm` still fails initially (not warned)
2. ✅ Git mentioned (still late)
3. ⚠️ Logo fumble still visible
4. ❌ No troubleshooting guidance

---

## 📈 Summary Comparison

| Aspect | Original (30m) | Charlie (15m) | Angie (19m) |
|:-------|:--------------:|:-------------:|:-----------:|
| **🤜 Doability Score** | **3.3/10** | **5.2/10** | **4.8/10** |
| Duration | 30 min | ~16 min | ~19 min |
| Time saved vs Original | — | 14 min (47%) | 11 min (37%) |
| Prerequisites | ❌ Missing | ⚠️ Partial | ⚠️ Partial |
| Commands formatted | ⚠️ Inline | ✅ Listed | ✅ Code blocks |
| Fumbles removed | ❌ Present | ⚠️ Kept | ⚠️ Kept |
| Troubleshooting | ❌ None | ❌ None | ❌ None |

---

## 🔍 Why Angie < Charlie?

Angie's Descript edit is **longer** (19 min) than Charlie's (15 min) and scores **lower** (4.8 vs 5.2) because:

| Issue | Impact |
|:------|:-------|
| Logo fumble [13:00-15:00] still included | Adds 2 min of confusion |
| No jump cuts on Lovable generation | Wait time preserved |
| Filler words removed but content preserved | Descript transcript ≠ manual edit |
| Missing title card with prerequisites | Same gap as Charlie |

**Key insight**: Descript's transcript-based editing preserved content that Charlie's manual edit removed.

---

## 🎯 Gap Analysis: What All Versions Miss

| Gap | Impact | Novice Blocker? |
|:----|:-------|:---------------:|
| **Node.js prerequisite** | `npm` fails immediately | ✅ Yes |
| **Git installation link** | Mentioned but not linked | ⚠️ Partial |
| **Cursor download** | Assumes already installed | ⚠️ Partial |
| **GitHub signup** | Assumes account exists | ⚠️ Partial |
| **Troubleshooting section** | Students stuck with no recourse | ✅ Yes |

---

## 🏆 What Would Make a 9/10 Version?

### Add: Prerequisites Title Card (15 sec)
```
Before starting, install:
✅ Node.js → nodejs.org
✅ Git → git-scm.com
✅ Cursor → cursor.com
✅ GitHub account → github.com
```

### Cut: Logo Fumble [13:00-15:00] (Saves 2 min)
Replace with clean, pre-prepared prompt showing success on first try.

### Add: Troubleshooting Card (15 sec)
```
Common Issues:
• "npm not found" → Install Node.js first
• "git not found" → Install Git first
• "permission denied" → Check folder permissions
```

### Add: On-Screen Command Overlays
Show commands as text while speaking:
- `npm install` / `npm run dev`
- `git status` / `git add .` / `git commit -m ""` / `git push origin main`

---

## 📊 Projected Scores with Improvements

| Version | Current | +Prerequisites | +Clean Demo | +Troubleshooting | **Projected** |
|:--------|:-------:|:--------------:|:-----------:|:----------------:|:-------------:|
| Original | 3.3 | +1.5 | +1.5 | +1.0 | **7.3** |
| Charlie | 5.2 | +1.5 | +1.0 | +1.0 | **8.7** |
| Angie | 4.8 | +1.5 | +1.5 | +1.0 | **8.8** |

---

## ✅ Recommended: Angie V2 (Target 10-12 min)

To create the optimal version from Angie's Descript edit:

### Descript Actions

| Action | Timestamp | Time Saved |
|:-------|:----------|:-----------|
| Add Prerequisites title card | 0:00 | +15 sec |
| Cut logo fumble | [13:00-15:00] | 2 min |
| Add text overlays for commands | [11:00], [17:00-18:00] | — |
| Add troubleshooting card | End | +15 sec |

### Estimated Result
- **Duration**: ~17 min → ~12 min
- **Doability Score**: 4.8 → **8.5+**

---

## 🎓 PM Lesson

> **The paradox**: A 30-minute video with more information produces worse outcomes than a 10-minute video with less information.

**Why?**
- Novices need **actionability**, not comprehensiveness
- Missing prerequisites blocks progress entirely
- Watching mistakes creates uncertainty
- Time spent ≠ learning achieved

**Applied to Product Management**: When building products, **remove friction** before adding features. The same principle applies to tutorials, onboarding, and user documentation.

---

## 📁 File References

| Version | File | Duration | Score |
|:--------|:-----|:--------:|:-----:|
| Original | `30min_video.md` | 30 min | 3.3 |
| Charlie | `🧑‍🏫15min_video_charlie.md` | 15 min | 5.2 |
| Angie | `👩‍🏫15min_video_angie.md` | 19 min | 4.8 |

---

# 🤖 Version 4: Claude Code Instructions (Written Document)

**Source**: `PM_Prototyping_with_Claude_Code_Assignment.docx`

## Overview

This version replaces **Lovable + Cursor** with **Claude Code** — a single AI tool that handles both creation and modification.

### Tool Comparison

| Aspect | Lovable + Cursor | Claude Code |
|:-------|:-----------------|:------------|
| Tools needed | 3 (Lovable, Cursor, GitHub) | 2 (Claude Code, GitHub) |
| Interface | Web UI + Desktop app | Terminal/CLI |
| Learning curve | Lower (visual) | Higher (command line) |
| Workflow | Create → Connect → Clone → Edit → Push | Create → Init → Edit → Push |
| Cost | Lovable free tier limited | Requires API key |

---

## 🤜 Doability Score: Claude Code Version

### Scores

| Criterion | Score | Evidence |
|:----------|:-----:|:---------|
| Prerequisites Clear | **9/10** | Node.js, Git, GitHub listed with install links |
| Steps Numbered | **9/10** | Clear Step 1-5 structure with substeps |
| Commands Explicit | **8/10** | Commands shown: `npm install -g @anthropic-ai/claude-code`, `claude`, git commands |
| Error Handling | **4/10** | Mentions "if something isn't right, describe what's wrong" but no troubleshooting |
| No Confusion | **8/10** | Clean document, no fumbles (it's written, not transcribed) |
| Time Respect | **8/10** | Concise, action-oriented prose |

### 🤜 Claude Code Score: **7.7/10**

### Novice Experience
> *"The instructions are clear and I knew exactly what to install first. The Step 1-5 structure helped me follow along. But I'm intimidated by the terminal—I've never used command line before. The document assumes I know what 'cd path/to/folder' means."*

---

## Gap Analysis: Claude Code Version

### Strengths vs Video Versions

| Strength | Why It Helps |
|:---------|:-------------|
| ✅ Prerequisites **at the start** | Won't hit `npm not found` |
| ✅ Written document | Can ctrl+F, re-read, no scrubbing video |
| ✅ Example prompts included | Can copy-paste directly |
| ✅ Single tool workflow | Less context switching |
| ✅ No fumbles/mistakes | Clean instructions |

### Remaining Gaps

| Gap | Impact | Severity |
|:----|:-------|:--------:|
| Terminal literacy assumed | "cd path/to/folder" confuses novices | ⚠️ Medium |
| API key setup not mentioned | Claude Code requires Anthropic API key | ❌ High |
| No screenshots | Text-only, harder to verify you're on track | ⚠️ Medium |
| Error handling minimal | "Just ask Claude" isn't actionable when stuck | ⚠️ Medium |

---

## 🔬 Live Test: Can I Complete This Exercise?

### Prerequisites Check

```bash
# Check Node.js
node --version
# Should return: v18.x.x or higher

# Check Git
git --version
# Should return: git version 2.x.x

# Check Claude Code
claude --version
# Should return version number
```

### Step-by-Step Walkthrough

**Step 1: Install Claude Code**
```bash
npm install -g @anthropic-ai/claude-code
```

**Step 2: Create project folder and start Claude**
```bash
mkdir my-pm-prototype
cd my-pm-prototype
claude
```

**Step 3: Give Claude Code a prompt** (from the document)
```
Create a web app for MBA students to find study partners. The app should have:
(1) A home screen showing available study groups with filters for course and time
(2) A group detail screen showing members, meeting times, and a join button
(3) A create group screen with fields for course name, meeting time, location, and maximum members
Use a professional blue color palette (#1a365d as primary). Make it mobile-responsive.
```

**Step 4: Run locally**
```
How do I run this app locally?
```

**Step 5: Push to GitHub**
```
Help me initialize a git repository and push this project to GitHub.
```

---

## 📊 Final Comparison: All Versions

| Version | Format | Duration | 🤜 Score | Best For |
|:--------|:-------|:--------:|:--------:|:---------|
| Original | Video | 30 min | 3.3/10 | ❌ Not recommended |
| Charlie | Video | 15 min | 5.2/10 | Visual learners who can troubleshoot |
| Angie | Video | 19 min | 4.8/10 | (Needs more editing) |
| **Claude Code** | **Document** | **~10 min read** | **7.7/10** | **Terminal-comfortable users** |

---

## 🎯 Recommendation by Student Type

| Student Profile | Recommended Version | Why |
|:----------------|:--------------------|:----|
| **Never used terminal** | Charlie's video + Prerequisites card | Visual guidance, can pause/rewatch |
| **Comfortable with terminal** | Claude Code document | Faster, single tool, copy-paste commands |
| **Want to understand deeply** | Claude Code + ask "explain" often | Claude Code explains as it builds |
| **Just want to finish fast** | Claude Code | Shortest path to working prototype |

---

---

## 🎬 Version 5: Claude Code v2 (Improved Document)

**Source**: `PM_Prototyping_with_Claude_Code_v2.md`

### Improvements Applied (Top 10 from Novice Walkthrough)

| # | Issue Fixed | How |
|:-:|:------------|:----|
| 1 | API key not mentioned | Added full setup section with console.anthropic.com |
| 2 | First-time setup | Explained API key prompt on first run |
| 3 | "What's a terminal?" | Added Mac/Windows instructions for finding Terminal |
| 4 | `cd path/to/folder` | Added concrete example: `cd ~/Desktop/my-mba-app` |
| 5 | Node.js version | Specified "Download LTS version" |
| 6 | localhost explanation | Added "type in browser address bar" |
| 7 | Cost information | Added $5 free credit, $0.50-$2 per prototype |
| 8 | Keep terminal open | Explicit warning with explanation |
| 9 | Troubleshooting | Full table of common errors and solutions |
| 10 | Public vs Private | Specified "select Public so TAs can access" |

### Scores

| Criterion | Score | Evidence |
|:----------|:-----:|:---------|
| Prerequisites Clear | **10/10** | Checklist with install links, verification commands, cost info |
| Steps Numbered | **9/10** | Step 1-5 with substeps (1.1, 1.2, etc.) |
| Commands Explicit | **9/10** | Code blocks with copy-paste examples |
| Error Handling | **8/10** | Full troubleshooting table with 8 common issues |
| No Confusion | **9/10** | Terminal explained, paths concrete, tips throughout |
| Time Respect | **9/10** | Concise but complete |

### 🤜 Claude Code v2 Score: **9.0/10**

### Novice Experience
> *"Finally! I knew exactly what to install before starting. The terminal explanation helped—I didn't know Mac had a 'Terminal' app. The troubleshooting table saved me when I got 'command not found'. Built my prototype in 20 minutes."*

---

## 📊 Final Comparison: All Versions

| Version | Format | Duration | 🤜 Score | Status |
|:--------|:-------|:--------:|:--------:|:-------|
| Original | Video | 30 min | 3.3/10 | ❌ Not recommended |
| Charlie | Video | 15 min | 5.2/10 | ⚠️ Needs prerequisites |
| Angie | Video | 19 min | 4.8/10 | ⚠️ Needs more cuts |
| Claude Code v1 | Document | ~10 min | 7.7/10 | ✅ Good for terminal users |
| **Claude Code v2** | **Document** | **~12 min** | **9.0/10** | **✅ Recommended** |

---

## 🚀 Try It Now: Quick Start for Claude Code

If you want to test Claude Code right now:

```bash
# 1. Install (if not already)
npm install -g @anthropic-ai/claude-code

# 2. Create project
mkdir test-prototype && cd test-prototype

# 3. Start Claude Code
claude

# 4. Paste this prompt:
# "Create a simple contact list app with: (1) home page showing contacts,
# (2) add contact form, (3) delete button. Use MIT red (#A31F34) as primary color."

# 5. When done, ask:
# "How do I run this locally?"

# 6. View at http://localhost:5173 (or whatever URL Claude provides)
```

**Estimated time to working prototype**: 5-10 minutes
