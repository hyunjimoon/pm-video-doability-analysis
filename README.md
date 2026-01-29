# PM Video Doability Analysis

> **Research Question**: Can a novice MBA student complete a prototyping exercise by following video/written instructions?

This repository documents the evaluation and improvement of PM tutorial materials for Prof. Charlie Fine's Product Management course at MIT.

---

## 🎯 Charlie's Three Tasks

### Task 1: Evaluate if Novice Can Complete the Exercise
**Method**: Read the 30-minute video transcript as a novice. Identify every point where a student with no coding experience would get stuck.

**Finding**: Original video scores **3.3/10** on doability.

**Critical Blocker**: Node.js prerequisite never mentioned → 100% of novices fail at `npm install`

### Task 2: Edit Transcript to Clarify Instructions
**Method**: Create shortened versions that address confusion points.

| Version | Editor | Duration | Score | Key Change |
|:--------|:-------|:--------:|:-----:|:-----------|
| Original | Andres | 30 min | 3.3/10 | — |
| Charlie's edit | Charlie | 15 min | 5.2/10 | Removed motivation section, cleaner structure |
| Angie's edit | Angie (Descript) | 19 min | 4.8/10 | Removed fillers, but kept logo fumble |

### Task 3: Test Claude Code Version
**Method**: Walk through Claude Code instructions as a novice, flag all confusion points, implement top 10 fixes.

| Version | Score | Key Improvements |
|:--------|:-----:|:-----------------|
| Claude Code v1 | 7.7/10 | Prerequisites listed, single tool workflow |
| Claude Code v2 | **9.0/10** | +API key setup, +terminal explanation, +troubleshooting table |

---

## 🤜 Doability Scores Summary

| Version | Format | Duration | Score | Verdict |
|:--------|:-------|:--------:|:-----:|:--------|
| Original | Video | 30 min | 3.3/10 | ❌ Blocked at `npm` |
| Charlie | Video | 15 min | 5.2/10 | ⚠️ Still missing prerequisites |
| Angie | Video | 19 min | 4.8/10 | ⚠️ Needs more cuts |
| Claude Code v1 | Document | ~10 min | 7.7/10 | ✅ Workable |
| **Claude Code v2** | **Document** | **~12 min** | **9.0/10** | **✅ Recommended** |

---

## 📁 Repository Structure

```
├── 1_transcripts/           # Task 1 & 2: Video transcripts
│   ├── original_30min.md
│   ├── charlie_15min.md
│   └── angie_19min.md
│
├── 2_analysis/              # Task 1 & 3: Evaluation results
│   ├── doability_comparison.md
│   └── novice_walkthrough.md
│
└── 3_improved_instructions/ # Task 3: Fixed version
    └── claude_code_v2.md
```

---

## 💡 Key Insight

> **A 30-minute video with more information produces worse outcomes than a 10-minute document with less information.**

**Why?**
- Missing prerequisites block progress entirely
- Watching mistakes creates uncertainty
- For tutorials: **Actionability > Comprehensiveness**

---

## Evaluation Criteria

| Criterion | Weight | Description |
|:----------|:------:|:------------|
| Prerequisites Clear | 20% | Are Node.js, Git, accounts listed upfront? |
| Steps Numbered | 15% | Can novice follow 1-2-3 sequence? |
| Commands Explicit | 20% | Are terminal commands copy-pasteable? |
| Error Handling | 15% | What to do when something fails? |
| No Confusion | 15% | Are there fumbles or corrections? |
| Time Respect | 15% | Does it get to the point? |

---

*Analysis conducted for MIT Product Management course (Prof. Charlie Fine), January 2026*

*Generated with Claude Code*
