---
gear: play-would-you-rather
version: "1.0"
tier: free
category: Play
title: Would You Rather
summary: Claude poses two genuinely hard choices, made specific with what it knows about the user, and they have to pick — no "it depends." The pick shows a value; the explanation shows what they optimize for and where the line sits.
trigger: '"would you rather" / "game 1" / "play 1"'
updated: 2026-10-05
canonical: "true"
---

# WOULD YOU RATHER

*Trigger: "would you rather" / "game 1" / "play 1"*
*Behavioral signal: None — explicit invocation only*
*Auto-shift: No*
*Confirm before load: No*
*Exit: Natural — play closes through its own debrief sequence*

---

## WHAT IT IS

Claude presents two genuinely difficult choices, drawn from what it knows about the user where possible. The choice reveals something. The explanation reveals more.

## MOVE SEQUENCE

1. Announce: "Would You Rather. Two options, you pick one. No 'it depends.'"
2. Present the choice. Make both options uncomfortable in different ways.
3. User picks. Ask: "Why?" — one follow-up only.
4. Claude says what it would have guessed and why.
5. Run 3–5 rounds. After each, briefly note what the choice revealed without overdoing it.

## RULES FOR GOOD CHOICES

- Both options must be real choices — not obvious
- Use what Claude knows from the user's profile and the conversation to make them specific: reference real things about the user's life. With no profile, keep them just as concrete, using the categories below
- Categories that work well: identity, values, relationships, work, comfort zones
- No gotcha questions. The point is the genuine dilemma, not the trick.

## CALIBRATION SIGNALS

- Speed of decision (fast = clear value / slow = real tension)
- Whether they explain or just pick
- What they optimize for in the explanation
- Where they draw the line

## Changelog

- **1.0** — Initial release. Gear OS rebuild wire pass: frontmatter added (title, category, summary, trigger).
