---
gear: handoff
version: "3.1-general"
category: Session
title: HANDOFF
summary: Writes the cold-start brief for the next session into HANDOFF.md. Forward-facing, written for a session that has never seen this one — build state, next steps, open loops, nuance, boot sequence. Overwrites each time; a snapshot, not an archive.
trigger: '"handoff" / "good night + handoff" / "write the next-session brief"'
auto: "false"
---

# HANDOFF

*Trigger: "handoff" / "good night + handoff" / "write the next-session brief"*
*Behavioral signal: Explicit invocation only — the operator is closing and wants continuity delivered to the next session*
*Auto-shift: No*
*Exit: HANDOFF.md written — the next session can boot from it → return to DEFAULT*

---

## What it is

The gap between sessions. One session ends mid-stream, another arrives to continue — and instead
of reconstructing what happened, it already knows. Handoff writes the cold-start brief that makes
that possible: forward-facing, written for someone who has never seen this session.

Good for: multi-session projects, handing off mid-stream work, explicit "good night + handoff"
closes.

---

## What it looks like working

- Writes for the next session, not the operator — the audience is a fresh session with no context
- Specific over vague: names the actual files, decisions, open questions, and boot sequence
- Captures nuance: what doesn't show up in a file list but would matter on arrival
- Writes what it wishes it had known at the start
- Overwrites the previous handoff — snapshot, not archive
- Returns to DEFAULT on completion

---

## How to run

1. **Orient** — who's arriving, what kind of project, what the work state is
2. **Session summary** — one paragraph: what this session was actually about
3. **Build state** — what exists, where it lives, what's complete vs. in-flight
4. **Next steps** — the specific immediate next action first, then the one after it
5. **Open loops** — blockers, unanswered questions, anything waiting on someone
6. **Nuance** — what doesn't appear in a file list but would matter on arrival
7. **Boot sequence** — in order: what to read, what to check, what to ask first
8. **Write `HANDOFF.md`** in the project's root, replacing the last one → return to DEFAULT

---

## Output format

```markdown
# Handoff · [date]

**For:** the next session, cold.
**This session:** [what it was about, one paragraph]

## Build state
[what exists, where it lives, what's complete vs. in-flight]

## Next steps
1. [the immediate next action, specific]
2. [the one after it]

## Open loops
- [blockers, unanswered questions, anything waiting on someone]

## Nuance
[the stuff that doesn't show up in a file list]

## Parked
[what's intentionally deferred, and why]

## Boot sequence
1. [what to read first]
2. [what to check]
3. [what to ask]
```

`/judgement-os:boot` reads **Next steps** and **Open loops** from this file for its handoff phase, so keep
those two headings as they are.

---

## When to use

- "Handoff" / "good night + handoff"
- Any session that ends mid-stream with intent to continue
- Before a planned break of more than a day
- When passing a project to someone else

## When not to use

- A finished piece of work: if nothing continues, there's nothing to hand off.
- A short break: a few hours doesn't need a handoff.

**Failure mode:** a handoff that summarizes the past instead of briefing the future. The question
is "what does the next session need?", not "what happened?"

---

## Negative parameters

NOT a session summary for the operator. Written for the incoming session.
NOT an archive. Overwrites each time — the git history holds the record.
NOT vague. "We were working on something" is a failed handoff. Name it specifically.
