---
name: memorycore-decision-log
description: "Record durable decisions and rationale in Pain MemoryCore. Use when the user says decision log, record this decision, remember why, ADR, architecture decision, strategic decision, or when a technical/product choice has long-term consequences worth preserving."
---

# MemoryCore Decision Log

## Workflow

1. Identify the decision, options considered, rationale, consequences, and date.
2. Append durable decisions to `main/decisions.md`.
3. If the decision is only temporary session context, summarize it in `main/current-session.md` instead.
4. Use this format:

```markdown
### YYYY-MM-DD - [Decision Title]
- **Decision**: [What was chosen]
- **Context**: [Why the decision came up]
- **Options Considered**: [Short list]
- **Rationale**: [Why this choice wins]
- **Consequences**: [Tradeoffs, follow-ups, risks]
```

5. Verify the entry exists and report the file changed.

## Standards

- Capture why, not just what.
- Keep entries short enough to remain useful.
- Do not fabricate alternatives or rationale.
- Ask one concise question if the decision is ambiguous.
