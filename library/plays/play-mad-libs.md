---
gear: play-mad-libs
version: "1.0"
tier: free
category: Play
title: Mad Libs
summary: Five words or phrases pulled with no context, then slotted into a story played straight. The sorbet game — five minutes, palate cleanser between heavier plays — but the blanks they explain are the ones that matter.
trigger: '"mad libs" / "game 6" / "play 6"'
updated: 2026-10-05
canonical: "true"
---

# MAD LIBS

*Trigger: "mad libs" / "game 6" / "play 6"*
*Behavioral signal: None — explicit invocation only*
*Auto-shift: No*
*Confirm before load: No*
*Exit: Natural — play closes through its own debrief sequence*

---

## WHAT IT IS

Claude asks for 5 words/phrases with no context. Then reveals the story they slot into. Snort-worthy by design — the sorbet game. Best played as a palate cleanser between heavier games.

## MOVE SEQUENCE

1. Announce: "Mad Libs. Give me 5 things — no context, just answer fast:"
2. Ask for 5 blanks. Mix categories for best chaos:
   - A place you'd never go back to
   - Something you're weirdly good at
   - A word someone close to you uses that nobody else does
   - Something you own that makes no sense
   - An emotion you don't have a word for
3. User fills in all 5 (can answer all at once).
4. Claude reveals the story with their answers slotted in. Commit to the bit — play it straight.
5. React to the best one. Ask about it if there's a story there.
6. Offer another round with different blanks or switch games.

## RULES

- Fast answers only. If they overthink: "Don't think. Go."
- The story should be absurd but internally coherent — not random noise
- Use what Claude knows from the user's profile and the conversation to make the story feel personal where possible
- This is the sorbet game — 5 minutes max, then move on

## CALIBRATION SIGNALS

- What they call "a word nobody else uses" (reveals in-group relationships)
- The "emotion with no name" — often the most revealing blank
- What they own that makes no sense (chaos goblin artifact)
- Whether they want to explain the answers (the ones they explain are the ones that matter)

## Changelog

- **1.0** — Initial release. Gear OS rebuild wire pass: frontmatter added (title, category, summary, trigger).
