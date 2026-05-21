# Decisions
*Append-only decision log for Pain and Noobster.*

Use this file to preserve important technical, product, architecture, workflow, and MemoryCore decisions.

## Format

```markdown
### YYYY-MM-DD - [Decision Title]
- **Decision**: [What was chosen]
- **Context**: [Why the decision came up]
- **Options Considered**: [Short list]
- **Rationale**: [Why this choice wins]
- **Consequences**: [Tradeoffs, follow-ups, risks]
```

---

### 2026-05-22 - Codex-first MemoryCore adaptation
- **Decision**: Make this repository Codex-specific with Codex-native skills and `AGENTS.md`.
- **Context**: Noobster is using Codex, while the original MemoryCore template had non-Codex runtime assumptions.
- **Options Considered**: Keep upstream assumptions, dual-runtime setup, or Codex-specific runtime.
- **Rationale**: Codex-specific runtime avoids duplicate skill systems and keeps Pain's operating path unambiguous.
- **Consequences**: Future runtime skills should be bundled in `codex-skills/`; other runtimes should live in a separate fork only if needed.

### 2026-05-22 - Contextual command nudges
- **Decision**: Add `command-nudges` as a Codex-native skill.
- **Context**: Noobster wants reminders to run related MemoryCore commands after responses, but only when useful.
- **Options Considered**: No reminders, always remind, or contextual nudges.
- **Rationale**: Contextual nudges improve skill usage and memory hygiene without making Pain annoying or robotic.
- **Consequences**: Pain should suggest one relevant command only when it materially improves memory, planning, review, or prevention.
