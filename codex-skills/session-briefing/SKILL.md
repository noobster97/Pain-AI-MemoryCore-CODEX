---
name: session-briefing
description: "Create a concise session-start or on-demand briefing for Pain MemoryCore. Use when Noobster says brief, session brief, where did we leave off, what did we do last time, start session, or when beginning a new substantial work session in this repo."
---

# Session Briefing

## Workflow

1. Read `main/current-session.md`.
2. Check optional files if present:
   - `main/reminders.md`
   - `main/decisions.md`
   - `main/post-mortems.md`
3. Summarize only what matters now.
4. Keep output under 12 lines.

## Output Shape

```text
Session Brief
Last session: [one line]
Current focus: [one line]
Open flags: [max 3]
Suggested next move: [one line]
```

## Rules

- No long history dump.
- Prioritize next action and risk.
- Skip empty sections.
- If Noobster says `skip brief`, do not brief again in that session.
