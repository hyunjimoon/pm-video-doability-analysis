# PM Video Doability Analysis

> **Research Question**: Can a novice MBA student complete a prototyping exercise by following video/written instructions?

Analysis and improvement of PM tutorial materials for Prof. Charlie Fine's Product Management course at MIT Sloan.

---

## Quick Start for Charlie

| What You Need | Link |
|:--------------|:-----|
| **Claude Code video** | [Google Drive (10 min)](https://docs.google.com/videos/d/1K_QM0viGAfKkscE1kLrkFyJLUD_OqcprlZUuDcX5vds/edit) |
| **Claude Code slides** | [Google Slides](https://docs.google.com/presentation/d/1mh7uzy2-RCQKt3H0W_l_ZSr7dRlhF2HcGB73N4IPafU/edit) |
| **Claude Code instructions** | [`claude_code_v2.md`](3_improved_instructions/claude_code_v2.md) |
| **Lovable/Cursor video** | [Descript (20 min)](https://share.descript.com/view/h6rLcdP97IR) |
| **Full narrative** | [`CHANGELOG.md`](CHANGELOG.md) |

---

## The Story in 30 Seconds

**Charlie asked**: Can novices complete the prototyping exercise?

**ChatGPT said**: Yes, scores 7.5-9/10

**Claude found**: No — video says `npm install` but never mentions Node.js must be installed first → 100% of novices get "command not found" error and are stuck

**Solution**: Created Claude Code v2 instructions scoring **9.0/10**

> **Key Insight**: A 30-minute video with more information produces worse outcomes than a 10-minute document with less information. For tutorials: **Actionability > Comprehensiveness**

---

## Evaluation Summary

### Two Evaluators, Different Standards

| Version | ChatGPT | Claude | Gap |
|:--------|:-------:|:------:|:---:|
| Original (30 min) | 7.5 | 3.3 | -4.2 |
| Charlie's revision | 9.0 | 5.2 | -3.8 |
| Angie's revision | 8.0 | 4.8 | -3.2 |
| Claude Code v2 | — | **9.0** | — |

**Why the gap?** ChatGPT assumed novices would Google solutions. Claude assumed they would give up at the first blocker.

### The Critical Blocker

The video assumes students have Node.js installed, but never says so:

```
Step 1: Video says "type npm install"
Step 2: Novice types "npm install"
Step 3: Terminal shows "npm: command not found"
Step 4: Novice is stuck — what is npm? what went wrong?

Root cause: npm comes bundled with Node.js
            Video never told students to install Node.js first
            → 100% of true novices blocked at this step
```

---

## Two Tutorial Approaches

| Aspect | Lovable + Cursor | Claude Code |
|:-------|:-----------------|:------------|
| Tools needed | 3 | 2 |
| Interface | Visual (web + app) | Terminal |
| Video duration | 20 min | 10 min |
| Written instructions | No | Yes ([v2.md](3_improved_instructions/claude_code_v2.md)) |
| Doability score | 4.8-5.2 | **9.0** |
| **Recommendation** | Visual learners | Everyone else |

---

## Repository Structure

```
pm-video-doability-analysis/
├── README.md                    ← You are here
├── CHANGELOG.md                 ← Full narrative arc
│
├── 1_transcripts/               ← Video transcripts
│   ├── original_30min.md        (3.3/10)
│   ├── charlie_15min.md         (5.2/10)
│   └── angie_19min.md           (4.8/10)
│
├── 2_analysis/                  ← Evaluation details
│   ├── doability_comparison.md
│   └── novice_walkthrough.md    (30 improvements flagged)
│
├── 3_improved_instructions/     ← The solution
│   └── claude_code_v2.md        (9.0/10) ✅
│
└── 4_slides/                    ← Tutorial materials
    └── README.md                (slides, video, replication guide)
```

---

## Evaluation Criteria

| Criterion | Weight | Question |
|:----------|:------:|:---------|
| Prerequisites Clear | 20% | Are Node.js, Git, accounts listed upfront? |
| Steps Numbered | 15% | Can novice follow 1-2-3 sequence? |
| Commands Explicit | 20% | Are commands copy-pasteable? |
| Error Handling | 15% | What to do when something fails? |
| No Confusion | 15% | Are there fumbles or corrections? |
| Time Respect | 15% | Does it get to the point? |

---

## Next Steps for Spring 2026

1. **Choose approach**: Lovable/Cursor (visual) or Claude Code (terminal)
2. **Test with 2-3 students** before launch
3. **Iterate** based on real student errors

---

## Contributors

| Who | Role |
|:----|:-----|
| **Prof. Charlie Fine** | Course instructor, requested evaluation |
| **Andres** | Created original 30-min video |
| **Hyunji Moon** | Analysis, editing, Claude Code testing |
| **Claude Code (Opus 4.5)** | Co-authored improvements |
| **ChatGPT** | Initial novice simulation |

---

*Analysis conducted January 2026 for MIT Sloan Product Management*

*For full project history, see [`CHANGELOG.md`](CHANGELOG.md)*
