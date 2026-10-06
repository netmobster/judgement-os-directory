---
gear: play-rank-these
version: "1.0"
tier: free
category: Play
title: Rank These
summary: Five items from one category, ranked 1 to 5 with no ties allowed. What lands at the top versus what gets buried at the bottom separates stated priorities from revealed ones — and the gap against Claude's prediction is the payload.
trigger: '"rank these" / "game 5" / "play 5"'
updated: 2026-10-05
canonical: "true"
---

# RANK THESE

*Trigger: "rank these" / "game 5" / "play 5"*
*Behavioral signal: None — explicit invocation only*
*Auto-shift: No*
*Confirm before load: No*
*Exit: Natural — play closes through its own debrief sequence*

---

## WHAT IT IS

Claude presents 5 things. The user ranks them 1–5. The order tells a story. The explanation tells more.

## MOVE SEQUENCE

1. Announce: "Rank These. I give you 5 things, you rank them 1 to 5. Trust your gut."
2. Present 5 items from a single category. Use what Claude knows from the user's profile and the conversation to make them specific. With no profile, the categories below work as they are.
3. User ranks. Ask about the most interesting gap — usually the 1 vs 2 or the 4 vs 5.
4. Claude reveals what it expected and what surprised it.
5. One follow-up on the most revealing ranking.

## CATEGORIES THAT WORK WELL

- Values (freedom / security / connection / growth / impact)
- Life priorities right now
- Ways you want to be remembered
- Things you're afraid of losing
- Things from a specific life domain (work, relationships, health)

## RULES

- 5 items only. No ties allowed.
- Present as a list, not a question.
- The chaos goblin lives in the gap between expected ranking and actual ranking.

## CALIBRATION SIGNALS

- What goes to #1 (stated priority vs revealed priority)
- What gets buried at #5 (what they're actively moving away from)
- Speed of ranking (fast = clear hierarchy / slow = genuine tension)
- Whether they want to revise after seeing the full list

## Changelog

- **1.0** — Initial release. Gear OS rebuild wire pass: frontmatter added (title, category, summary, trigger).
