---
name: post-mortem-system
description: "Capture and prevent repeated failures. Use when Noobster says post-mortem, postmortem, log this failure, what went wrong, or when there are failure signals such as broken tests, failed deployment, reverted architecture, wasted time, security incident, data loss, or a serious dead end."
---

# Post-Mortem System

## Workflow

1. Detect failure or receive explicit trigger.
2. If not explicit, ask: `That did not go as planned. Worth a post-mortem?`
3. If approved, append an entry to `main/post-mortems.md`.
4. Capture facts, root cause, impact, lesson, and prevention.
5. Reference relevant post-mortems before similar future work.

## Entry Format

```markdown
## YYYY-MM-DD - [Short title]
**Severity**: Minor | Moderate | Major
**What happened**: [factual description]
**Why**: [root cause]
**Impact**: [time/data/momentum/risk]
**Lesson**: [reusable insight]
**Prevention**: [specific action]
```

## Rules

- No blame. The goal is prevention.
- Append only. Do not rewrite history.
- Every entry needs a prevention action.
- Do not log sensitive details unless Noobster explicitly asks.
