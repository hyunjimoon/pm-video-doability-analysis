# PM Video Doability Analysis

> **Research Question**: Can a novice MBA student complete a prototyping exercise by following video/written instructions?

This repository documents the evaluation and improvement of PM tutorial materials for Prof. Charlie Fine's Product Management course at MIT Sloan.

---

## Quick Start for Charlie

| What You Need | Where to Find It |
|:--------------|:-----------------|
| **Tutorial video** | [Google Drive Video](https://docs.google.com/videos/d/1K_QM0viGAfKkscE1kLrkFyJLUD_OqcprlZUuDcX5vds/edit?usp=sharing) |
| **Tutorial slides** | [Google Slides](https://docs.google.com/presentation/d/1mh7uzy2-RCQKt3H0W_l_ZSr7dRlhF2HcGB73N4IPafU/edit?usp=sharing) |
| **Recommended instructions** | [`3_improved_instructions/claude_code_v2.md`](3_improved_instructions/claude_code_v2.md) |
| **Full analysis** | [`2_analysis/doability_comparison.md`](2_analysis/doability_comparison.md) |
| **All transcripts** | [`1_transcripts/`](1_transcripts/) |

---

## Executive Summary

### The Problem
The original 30-minute video tutorial has a **3.3/10 doability score**. 100% of novices fail at `npm install` because Node.js is never mentioned as a prerequisite.

### The Solution
Created improved Claude Code instructions scoring **9.0/10**, addressing:
- Missing prerequisites (Node.js, Git, accounts)
- Terminal basics for non-technical users
- Two authentication paths (Claude Max vs API credits)
- Troubleshooting table for common errors

### Key Insight
> **A 30-minute video with more information produces worse outcomes than a 10-minute document with less information.**
>
> For tutorials: **Actionability > Comprehensiveness**

---

## Recommendation

For Spring 2026, we recommend using **Claude Code v2 instructions** + **tutorial slides**:

| Approach | Doability | Rationale |
|:---------|:---------:|:----------|
| Original video (Lovable+Cursor) | 3.3/10 | Missing prerequisites, confusing workflow |
| **Claude Code v2 + Slides** | **9.0/10** | Single tool, clear steps, troubleshooting included |

**Why Claude Code over Lovable+Cursor?**
- Single tool (Claude Code) vs three tools (Lovable + Cursor + GitHub)
- Terminal workflow is more transferable to industry
- Better error messages and AI assistance built-in

---

## Charlie's Three Tasks: Results

### Task 1: Evaluate if Novice Can Complete
**Finding**: Original video = **3.3/10**

| Criterion | Score | Issue |
|:----------|:-----:|:------|
| Prerequisites Clear | 2/10 | Node.js NEVER mentioned |
| Error Handling | 1/10 | No troubleshooting guidance |
| No Confusion | 3/10 | Logo fumble, tool mixups |

### Task 2: Edit Transcript to Clarify
| Version | Duration | Score | Change |
|:--------|:--------:|:-----:|:-------|
| Original | 30 min | 3.3/10 | — |
| Charlie's edit | 15 min | 5.2/10 | Added structure, kept mistakes |
| Angie's edit | 19 min | 4.8/10 | Descript cleanup, still too long |

### Task 3: Test Claude Code Version
| Version | Score | Key Improvements |
|:--------|:-----:|:-----------------|
| Claude Code v1 | 7.7/10 | Prerequisites listed |
| **Claude Code v2** | **9.0/10** | +Auth options, +Terminal basics, +Troubleshooting |

---

## Doability Scores: All Versions

| Version | Format | Duration | Score | Status |
|:--------|:-------|:--------:|:-----:|:-------|
| Original | Video | 30 min | 3.3/10 | Not recommended |
| Charlie | Video | 15 min | 5.2/10 | Missing prerequisites |
| Angie | Video | 19 min | 4.8/10 | Needs more cuts |
| Claude Code v1 | Document | ~10 min | 7.7/10 | Workable |
| **Claude Code v2** | **Document** | **~12 min** | **9.0/10** | **Recommended** |

---

## Repository Structure

```
pm-video-doability-analysis/
│
├── README.md                          # This file
│
├── 1_transcripts/                     # Task 1 & 2: Video transcripts
│   ├── original_30min.md              # Original video (3.3/10)
│   ├── charlie_15min.md               # Charlie's edit (5.2/10)
│   └── angie_19min.md                 # Angie's Descript edit (4.8/10)
│
├── 2_analysis/                        # Evaluation results
│   ├── doability_comparison.md        # Full scoring comparison
│   └── novice_walkthrough.md          # 30 flagged improvements
│
├── 3_improved_instructions/           # Task 3: Fixed version
│   └── claude_code_v2.md              # Production-ready (9.0/10)
│
└── 4_slides/                          # Tutorial slides
    └── README.md                      # Slide overview + specs
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

1. **Test with 2-3 students** before Spring 2026 launch
2. **Gather feedback** on video clarity and instruction completeness
3. **Iterate** on troubleshooting section based on real student errors

---

## Contributors

- **Hyunji Moon** — Analysis, Claude Code testing, documentation
- **Claude Code (Opus 4.5)** — Co-authored improvements and evaluation

---

*Analysis conducted January 2026 for MIT Sloan Product Management course*
