# PM Video Doability Analysis

> **Research Question**: Can a novice MBA student complete a prototyping exercise by following video/written instructions?

This repository documents the evaluation and improvement of PM tutorial materials for Prof. Charlie Fine's Product Management course at MIT Sloan.

---

## Quick Start for Charlie

| Asset | Link |
|:------|:-----|
| **Claude Code video** | [Google Drive](https://docs.google.com/videos/d/1K_QM0viGAfKkscE1kLrkFyJLUD_OqcprlZUuDcX5vds/edit?usp=sharing) |
| **Claude Code slides** | [Google Slides](https://docs.google.com/presentation/d/1mh7uzy2-RCQKt3H0W_l_ZSr7dRlhF2HcGB73N4IPafU/edit?usp=sharing) |
| **Claude Code instructions** | [`claude_code_v2.md`](3_improved_instructions/claude_code_v2.md) |
| **Lovable/Cursor video** | [Descript](https://share.descript.com/view/h6rLcdP97IR) |
| **Full analysis** | [`doability_comparison.md`](2_analysis/doability_comparison.md) |

---

## Project Background

### Charlie's Original Request

1. **Watch the video** and read the transcript — assess if a novice can complete the exercise using Lovable, GitHub, and Cursor
2. **Edit the transcript** to make instructions clearer if there's confusion
3. **Test the Claude Code version** of the exercise

### Initial Evaluation (ChatGPT Agent)

ChatGPT role-playing a novice evaluated three transcript versions:

| Version | Score | Notes |
|:--------|:-----:|:------|
| Original (30 min) | 7.5/10 | Full video, some confusion points |
| Charlie's revision | 9/10 | Cleaner structure |
| Angie's revision | 8/10 | Closer to original for easier editing |

**Report**: [ChatGPT Simulation](https://chatgpt.com/share/697acd1a-ac00-8002-929c-26cc22557cbd)

### Deliverables Created

1. **20-minute Lovable/Cursor video** with title pages: [Descript Link](https://share.descript.com/view/h6rLcdP97IR)
2. **Claude Code alternative** with improved instructions (this repository)

---

## Two Approaches Compared

| Aspect | Lovable + Cursor | Claude Code |
|:-------|:-----------------|:------------|
| **Tools needed** | 3 (Lovable, Cursor, GitHub) | 2 (Claude Code, GitHub) |
| **Interface** | Web UI + Desktop app | Terminal/CLI |
| **Learning curve** | Lower (visual) | Medium (command line) |
| **Video** | [Descript 20 min](https://share.descript.com/view/h6rLcdP97IR) | [Google Drive 10 min](https://docs.google.com/videos/d/1K_QM0viGAfKkscE1kLrkFyJLUD_OqcprlZUuDcX5vds/edit) |
| **Instructions** | Video transcript | Written document |

### Recommendation

**For visual learners**: Use Lovable/Cursor video (20 min)

**For terminal-comfortable users**: Use Claude Code instructions + video (10 min)

---

## Doability Evaluation (Claude Analysis)

Re-evaluated all versions with stricter novice criteria:

| Version | Format | Duration | Claude Score | ChatGPT Score |
|:--------|:-------|:--------:|:------------:|:-------------:|
| Original | Video | 30 min | 3.3/10 | 7.5/10 |
| Charlie's edit | Video | 15 min | 5.2/10 | 9/10 |
| Angie's edit | Video | 19 min | 4.8/10 | 8/10 |
| Claude Code v1 | Document | ~10 min | 7.7/10 | — |
| **Claude Code v2** | **Document** | **~12 min** | **9.0/10** | — |

### Why Score Difference?

Claude evaluation used stricter criteria:
- **Prerequisites**: Node.js never mentioned in video → blocks 100% of novices at `npm install`
- **Error handling**: No troubleshooting guidance
- ChatGPT may have assumed novices would Google solutions

---

## Key Insight

> **A 30-minute video with more information can produce worse outcomes than a 10-minute document with less information.**

**Why?**
- Missing prerequisites block progress entirely
- Watching mistakes creates uncertainty
- For tutorials: **Actionability > Comprehensiveness**

---

## Repository Structure

```
pm-video-doability-analysis/
│
├── README.md                          # This file
│
├── 1_transcripts/                     # Video transcripts
│   ├── original_30min.md              # Original (3.3/10)
│   ├── charlie_15min.md               # Charlie's edit (5.2/10)
│   └── angie_19min.md                 # Angie's edit (4.8/10)
│
├── 2_analysis/                        # Evaluation results
│   ├── doability_comparison.md        # Full scoring comparison
│   └── novice_walkthrough.md          # 30 flagged improvements
│
├── 3_improved_instructions/           # Claude Code approach
│   └── claude_code_v2.md              # Production-ready (9.0/10)
│
└── 4_slides/                          # Tutorial materials
    └── README.md                      # Slides, video, replication guide
```

---

## Evaluation Criteria

| Criterion | Weight | What It Measures |
|:----------|:------:|:-----------------|
| Prerequisites Clear | 20% | Are Node.js, Git, accounts listed upfront? |
| Steps Numbered | 15% | Can novice follow 1-2-3 sequence? |
| Commands Explicit | 20% | Are terminal commands copy-pasteable? |
| Error Handling | 15% | What to do when something fails? |
| No Confusion | 15% | Are there fumbles or corrections? |
| Time Respect | 15% | Does it get to the point? |

---

## Next Steps

1. **Choose approach** for Spring 2026 (Lovable/Cursor vs Claude Code)
2. **Test with 2-3 students** before launch
3. **Gather feedback** on clarity and completeness
4. **Iterate** based on real student errors

---

## Contributors

- **Hyunji Moon** — Analysis, video editing, Claude Code testing
- **Claude Code (Opus 4.5)** — Co-authored improvements and evaluation
- **ChatGPT** — Initial novice simulation

---

*Analysis conducted January 2026 for MIT Sloan Product Management course (Prof. Charlie Fine)*
