# PRD Skill for Claude

A Claude skill for writing tight, stakeholder-ready Product Requirements Documents. Built for consumer web apps and internal tools. Opinionated by design.

---

## What It Does

Install this skill and Claude will produce structured PRDs in your style — without you having to re-explain your format every time.

**Bring a full brief** → Claude drafts immediately.  
**Bring a rough idea** → Claude asks 5 targeted questions, then drafts.  
**Bring an existing PRD** → Claude identifies the weakest sections and rewrites them.

---

## Document Structure

Every PRD follows this order:

| # | Section | Format |
|---|---------|--------|
| 1 | Executive Summary | 3–5 sentences, standalone |
| 2 | Why Now | Timing rationale, never skipped |
| 3 | Problem Statement + Hypothesis | Narrative + one-sentence hypothesis |
| 4 | User Segments | Persona + behavioral layer |
| 5 | Jobs to Be Done | Classic JTBD format |
| 6 | Success Metrics | OKR: 1 objective + 2–3 KRs |
| 7 | Scope | In scope / out of scope lists |
| 8 | Edge Cases | Top 3 blockers only |
| 9 | Open Questions | Categorized by UX / Technical / Business / Legal |

Target length: **1–2 pages**. Complexity scales length, but brevity is always the goal.

---

## Opinionated Defaults

**Hypothesis format**
```
We believe [doing X] for [user] will result in [outcome], measured by [metric].
```

**User Segments**
```
[Persona Name] — [Who they are]. Behaviorally: [what they do that's relevant].
```

**Jobs to Be Done**
```
When I ___, I want to ___, so I can ___.
```

**OKR format**
```
O:   [Qualitative goal]
KR1: [Metric + target]
KR2: [Metric + target]
KR3: [Metric + target]
```

**Edge Cases**
```
[Label]: [Situation]. [Handling or flag.]
```

**Open Questions**
```
[Category]
- [Question]? (Owner: [name or team if known])
```

---

## Tone & Style

- Short sentences. Active voice.
- No throat-clearing openers.
- Numbers over approximations.
- No weasel words: "potentially", "might", "could possibly".
- Bold only for labels and critical terms.

---

## Installation

1. Download `prd.skill`
2. Open Claude → Settings → Skills
3. Click **Install Skill** and select the file

Once installed, trigger it with phrases like:
- *"Write a PRD for…"*
- *"Help me spec this out"*
- *"Draft product requirements for…"*
- *"I need to write up a feature"*

---

## File Structure

```
prd/
└── SKILL.md    # Full skill instructions
```

---

## Customization

The skill is built around a specific PM style — leadership audience, OKR metrics, minimal edge cases, JTBD framing. If your defaults differ, edit `SKILL.md` directly. The section instructions and tone rules are clearly labeled.

---

## Quality Checklist

Before every PRD is finalized, Claude runs this internally:

- [ ] Executive summary stands alone
- [ ] Why Now is specific, not generic
- [ ] Hypothesis follows the exact format
- [ ] Each JTBD avoids solution language
- [ ] OKRs have measurable KRs
- [ ] Out of Scope list exists and is specific
- [ ] Edge cases are minimal (≤3) and actionable
- [ ] Open questions are categorized
- [ ] Total length is tight — nothing that doesn't earn its place
