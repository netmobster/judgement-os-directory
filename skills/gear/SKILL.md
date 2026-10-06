---
name: gear
description: Load a gear, loop or mode by name. Bare lists the menu.
argument-hint: "[name, fuzzy: scout, \"root cause\", goofy]"
disable-model-invocation: true
---

The typed shortcut into the library. Requested: **$ARGUMENTS**

Follow the router's skill (`${CLAUDE_PLUGIN_ROOT}/skills/router/SKILL.md`) for the menu (the user's
own gears included), the hidden part and the rules. This only adds the two things a typed command
needs.

- **Bare:** print the menu from the router's skill, grouped as gears, loops and modes, one
  line each, with each item's summary (its frontmatter's `summary:`, or the manifest's). Don't
  list the hidden parts.
- **With a name:** resolve it as the router's Names section says. The affix probe here is
  `loop-<x>` and `<x>-mode`.
  `→ resolved "<input>" → <slug>`.
