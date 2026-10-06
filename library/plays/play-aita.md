---
gear: play-aita
version: "1.0"
tier: free
category: Play
title: Am I The Asshole?
summary: Claude invents a morally ambiguous scenario and the user delivers a verdict. The judgment looks like it's about a stranger, but what gets weighted — intent versus impact, context versus rule — is the user's own value map.
trigger: '"am i the asshole" / "AITA" / "game 3" / "play 3"'
updated: 2026-10-05
canonical: "true"
---

# AM I THE ASSHOLE?

*Trigger: "am i the asshole" / "AITA" / "game 3" / "play 3"*
*Behavioral signal: None — explicit invocation only*
*Auto-shift: No*
*Confirm before load: No*
*Exit: Natural — play closes through its own debrief sequence*

---

## WHAT IT IS

Claude presents an ambiguous real-life scenario. The user judges it. The joke is that you think you're judging a stranger. You're not.

## MOVE SEQUENCE

1. Announce: "Am I The Asshole? I'll describe a situation. You tell me if the person is the asshole or not."
2. Generate a scenario. Rules for good scenarios:
   - Morally ambiguous — both sides have a point
   - Specific enough to feel real (names, settings, details)
   - Calibrated to the user when possible — use contexts they know, from their profile and the conversation. With no profile, pick settings anyone knows
   - The setting does work (a Starbucks changes everything)
   - No obvious villains. No obvious heroes.
3. Ask: "Asshole or not? Or somewhere in between?"
4. User gives verdict. Claude reveals what it predicted and why, using what it knows from the user's profile and the conversation.
5. Dig into the gap between verdict and prediction. That's where the real thing is.

## RULES

- Generate scenarios — no web search, no database
- No Reddit jargon (no YTA/NTA/ESH/NAH). Natural language only: "kind of an asshole," "not the asshole," "both have a point"
- Claude maps natural language to a verdict internally — never asks the user to learn jargon
- The point isn't the verdict. It's what the verdict reveals about the user's values.

## CALIBRATION SIGNALS

- How fast they judge (quick = clear values / slow = genuine conflict)
- Whether they see nuance or pick a side hard
- What factors they weight (intent vs impact, context vs rule)
- What makes them defend the "asshole" — that's always interesting

## Changelog

- **1.0** — Initial release. Gear OS rebuild wire pass: frontmatter added (title, category, summary, trigger).
