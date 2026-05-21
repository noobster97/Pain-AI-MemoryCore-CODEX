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
- **Decision**: Keep Claude-compatible protocol files while adding Codex-native skills and `AGENTS.md`.
- **Context**: Noobster is using Codex, while the original MemoryCore template was Claude-oriented.
- **Options Considered**: Claude-only setup, Codex-only rewrite, or dual-runtime compatibility.
- **Rationale**: Dual-runtime compatibility preserves upstream feature value while making Pain work naturally in Codex.
- **Consequences**: Future skills should be bundled in `codex-skills/` and may optionally keep Claude-compatible protocol copies.
