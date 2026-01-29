# Changelog

> **Project**: PM Video Doability Analysis
> **For**: Prof. Charlie Fine, MIT Sloan Product Management
> **By**: Hyunji Moon + Claude Code (Opus 4.5)

---

## Narrative Arc

### Phase 1: Charlie's Request

Charlie asked three questions about the PM prototyping tutorial:

1. Can a novice complete the exercise using Lovable, GitHub, and Cursor?
2. How can we edit the transcript to clarify instructions?
3. How does the Claude Code version compare?

### Phase 2: Initial Evaluation (ChatGPT)

ChatGPT role-played a novice and scored three transcript versions:

| Version | ChatGPT Score |
|:--------|:-------------:|
| Original (30 min) | 7.5/10 |
| Charlie's revision | 9/10 |
| Angie's revision | 8/10 |

**Report**: [ChatGPT Simulation](https://chatgpt.com/share/697acd1a-ac00-8002-929c-26cc22557cbd)

### Phase 3: Stricter Re-evaluation (Claude)

Claude applied stricter novice criteria and found a critical blocker:

> **Node.js prerequisite is NEVER mentioned → 100% of novices fail at `npm install`**

| Version | Claude Score | Why Lower? |
|:--------|:------------:|:-----------|
| Original (30 min) | 3.3/10 | Missing prerequisites, fumbles |
| Charlie's revision | 5.2/10 | Better structure, still missing Node.js |
| Angie's revision | 4.8/10 | Descript preserved too much content |

**Key Insight**: ChatGPT assumed novices would Google solutions. Claude assumed they would give up.

### Phase 4: Claude Code Alternative

Tested the Claude Code approach (single tool vs Lovable+Cursor):

| Version | Score | Improvement |
|:--------|:-----:|:------------|
| Claude Code v1 | 7.7/10 | Prerequisites listed, simpler workflow |
| Claude Code v2 | 9.0/10 | +Auth options, +Terminal basics, +Troubleshooting |

### Phase 5: Final Deliverables

Created two complete tutorial paths:

| Approach | Video | Instructions | Score |
|:---------|:------|:-------------|:-----:|
| Lovable/Cursor | [Descript 20min](https://share.descript.com/view/h6rLcdP97IR) | Video transcript | 4.8-5.2 |
| Claude Code | [Google 10min](https://docs.google.com/videos/d/1K_QM0viGAfKkscE1kLrkFyJLUD_OqcprlZUuDcX5vds/edit) | [claude_code_v2.md](3_improved_instructions/claude_code_v2.md) | 9.0 |

---

## Commit History (Chronological)

| # | Commit | Phase | What Changed |
|:-:|:-------|:------|:-------------|
| 1 | `📋 Task 1` | Evaluate | Read original transcript, scored 3.3/10 |
| 2 | `✏️ Task 2` | Edit | Added Charlie's and Angie's transcript versions |
| 3 | `🔧 Task 3` | Improve | Created Claude Code v2 (9.0/10) |
| 4 | `🔐 Fix auth` | Polish | Added Claude Max vs API key options |
| 5 | `🧹 Clean up` | Polish | English-only for sharing |
| 6 | `📚 Improve` | Package | Quick Start section for Charlie |
| 7 | `🎬 Add video` | Deliver | Slides + video + replication guide |
| 8 | `📋 History` | Document | All links, ChatGPT comparison |
| 9 | `📖 Narrative` | Finalize | This changelog, consistent story |

---

## Terminology Clarification

| Term | Meaning |
|:-----|:--------|
| **Charlie** | Prof. Charlie Fine (requester, not editor) |
| **Andres** | TA who created original 30-min video |
| **Angie/Hyunji** | Student who edited transcripts and tested |
| **Charlie's revision** | Transcript edited per Charlie's feedback |
| **Angie's revision** | Transcript edited via Descript |

---

## All Links (Single Source of Truth)

### Claude Code Approach (Recommended)
- **Video**: https://docs.google.com/videos/d/1K_QM0viGAfKkscE1kLrkFyJLUD_OqcprlZUuDcX5vds/edit
- **Slides**: https://docs.google.com/presentation/d/1mh7uzy2-RCQKt3H0W_l_ZSr7dRlhF2HcGB73N4IPafU/edit
- **Instructions**: [`claude_code_v2.md`](3_improved_instructions/claude_code_v2.md)

### Lovable/Cursor Approach (Original)
- **Video**: https://share.descript.com/view/h6rLcdP97IR
- **ChatGPT Report**: https://chatgpt.com/share/697acd1a-ac00-8002-929c-26cc22557cbd

### Repository
- **GitHub**: https://github.com/hyunjimoon/pm-video-doability-analysis

---

## Key Learnings

1. **Actionability > Comprehensiveness**: A 10-min document beats a 30-min video
2. **Prerequisites are critical**: One missing item blocks 100% of novices
3. **Evaluation method matters**: Strict criteria catch real blockers
4. **Single tool > Multiple tools**: Claude Code simpler than Lovable+Cursor+GitHub

---

*Last updated: January 2026*
