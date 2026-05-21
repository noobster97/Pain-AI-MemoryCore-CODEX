---
name: command-nudges
description: "Suggest one relevant MemoryCore/Codex command after a response only when it would materially improve the outcome. Use when a conversation creates durable memory, decisions, risks, failures, project planning needs, code review needs, or self-improvement opportunities; do not use for casual or obvious exchanges."
---

# Command Nudges

## Purpose

Help Noobster remember useful MemoryCore commands at the exact moment they matter, without turning Pain into a notification bot.

## Workflow

1. Decide if a nudge is useful.
2. If useful, add one short final line after the main answer.
3. Suggest only one command or skill.
4. Keep it optional and low-friction.

## Nudge Format

```text
Useful next command: `save memory` if you want this preserved.
```

or:

```text
Relevant skill: `survey` before we design the architecture.
```

## Command Map

- `save memory`: durable preference, decision, project context, or personal insight should persist.
- `brief`: user returns after a gap or asks where we left off.
- `survey`: before architecture, planning, refactor, or unfamiliar repo work.
- `investigate`: bug, unclear behavior, suspicious area, or root-cause work.
- `refine`: after code changes, before commit, or when quality pass is needed.
- `audit`: broad system review or high-stakes architecture check.
- `decision log`: non-obvious technical/product choice with future consequences.
- `post-mortem`: failure, wasted time, broken deploy/test, incident, or painful reversal.
- `self improve`: repeated workflow, repeated mistake, or skill gap appears.

## Suppression Rules

Do not nudge when:

- The response is casual small talk.
- The command is already being executed.
- More than one nudge would be needed.
- The user seems rushed and the nudge would distract.
- The suggestion is obvious noise.

## Tone

Keep nudges short, practical, and calm. Never guilt Noobster into using a command.

## Reference

Read `references/nudge-policy.md` for examples.
