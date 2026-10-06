# Judgement OS

A second opinion for your Claude Code skills, only when they need one. (*Not an operating system. The name is a joke; the plugin isn't.*)

Version 0.2.5. Made by Jay Wright. [The Judgement OS page](https://unstuck-games.com/judgement-os/) has the whole story.

## What it does

Skills make most decisions with a plain rule. At the few marked decisions where the right answer depends on you, and the rule can't tell, two judges (a small model and a big one) each answer one bounded question after reading a short profile you write about how you work. A recorder checks every answer in code and combines the two. You only hear about it when both judges disagree with the rule, with real confidence. Every call goes into an append-only log on your machine. The judges recommend; they never authorise.

Around that core, one plugin carries the rest of the system:

| Part | Commands | What it does |
|---|---|---|
| The judges | `/judgement-os:profile`, `/judgement-os:try` | Write the one file the judges read, then put both judges on a morning, blind, to see which one you trust |
| The day | `/judgement-os:boot`, `/judgement-os:checkin`, `/judgement-os:habits`, `/judgement-os:daily`, `/judgement-os:flag`, `/judgement-os:guide` | A short boot from your TASKS.md, check-ins, habits with no scores out of anything, a daily reading and a language phrase, and a field guide |
| Pages | `/judgement-os:sexyhtml`, `/judgement-os:jay`, `/judgement-os:seren`, `/judgement-os:judgement-os` | Finished HTML pages in a house style, with the style and the shape picked for you |
| Making things | `/judgement-os:make`, `/judgement-os:diff-review`, `/judgement-os:plan-review`, `/judgement-os:project-recap`, `/judgement-os:fact-check`, `/judgement-os:make-guide` | One front door: a page, a card in the chat, a deck, a doc or a file, and four explainer pages that cite every claim |
| Thinking tools | `/judgement-os:gear`, or plain words ("what am I missing", "grumpy on this") | 28 gears, loops and modes through one router |
| Messages | `/judgement-os:humanify`, `/judgement-os:poll` | A send gate that waits for your yes, a de-tic pass for drafts, and Slack polling |
| Hard rules | `/judgement-os:guard` | Hooks: deploys are printed, never run; destructive commands and secrets ask first |
| Dice | `/judgement-os:roll`, `/judgement-os:play` | Dice rolled by a script, never invented, and nine party games |

## Install

```
/plugin marketplace add netmobster/judgement-os-directory
/plugin install judgement-os@judgement-os
```

Then start with `/judgement-os:profile`. Until the profile exists, no judge is asked and every rule decides alone; nothing breaks.

## What it needs

Nothing to start. The day loop reads a TASKS.md in your project. Poll needs Claude's Slack connector. Everything Judgement OS keeps lives in `~/.claude/judgement-os/` on your machine; it never needs an account and sends nothing anywhere.

## The same plugins, separately

This is the plugin-directory build: everything in one plugin. The eight plugins also install one at a time from [netmobster/judgement-os-general](https://github.com/netmobster/judgement-os-general), where the commands keep their own names (`/labs:profile`, `/day:boot`).

## Licence

MIT.
