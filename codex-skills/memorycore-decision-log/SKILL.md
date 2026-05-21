---
name: memorycore-decision-log
description: "Record durable decisions and rationale in Pain MemoryCore. Use when the user says decision log, record this decision, remember why, ADR, architecture decision, strategic decision, or when a technical/product choice has long-term consequences worth preserving."
---

# MemoryCore Decision Log

## Workflow

1. Identify the decision, options considered, rationale, consequences, and date.
2. Prefer an existing decision-log location if installed. Check `master-memory.md` and `Feature/Decision-Log-System/`.
3. If no decision-log system is installed, record concise decision context in `main/current-session.md` and, when durable for the relationship/project, `main/relationship-memory.md`.
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
