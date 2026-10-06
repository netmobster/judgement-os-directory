---
name: play
description: Party games to play with Claude. Use when the user says let's play, play a game, I'm bored, or names one (would you rather, two truths, AITA, desert island, rank these, mad libs, story chain, young me, guess what Claude thinks).
argument-hint: "[game name, fuzzy, or a number 1–9]"
---

# /play: party games

Requested: **$ARGUMENTS**

Each play is a file: `${CLAUDE_PLUGIN_ROOT}/library/plays/play-<slug>.md`. **Read the one you
picked and play it from the spec.** Never improvise a game from its name.

| # | Play | Slug |
|---|---|---|
| 1 | Would You Rather | `would-you-rather` |
| 2 | Two Truths & a Lie | `two-truths` |
| 3 | Am I The Asshole? | `aita` |
| 4 | Desert Island | `desert-island` |
| 5 | Rank These | `rank-these` |
| 6 | Mad Libs | `mad-libs` |
| 7 | Story Chain | `story-chain` |
| 8 | Young [Name] | `young-name` |
| 9 | Guess What Claude Thinks | `guess-what-claude-thinks` |

- **No game named:** pitch **one**, picked to fit the moment (a short one if they're low, Mad
  Libs as a palate cleanser), in two lines. If they say no, offer the table.
- **Fuzzy and numbers work:** "game 3" → `aita`, "two truths" → `two-truths`.
- **Don't narrate the read mid-game.** It kills the game. The read lands in the debrief.
- **Plays that use what Claude knows about the user get sharper with the user's profile.** That
  is the settings' `profile` file, set up by `/judgement-os:profile` (`~/.claude/judgement-os/profile.md`
  by default). `node "${CLAUDE_PLUGIN_ROOT}/scripts/jos-settings.js"` prints it, and
  `profileFound` says whether it's filled in. With none, play the cold version the spec
  describes. Never make a profile just to play.
