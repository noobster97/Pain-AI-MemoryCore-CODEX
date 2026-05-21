---
name: save-memorycore
description: "Persist durable updates into Pain's MemoryCore. Use when the user says 'save', 'save memory', 'save progress', 'update memory', 'remember this', or when important preferences, decisions, project context, relationship learning, or session status should be written to the markdown memory files."
---

# Save MemoryCore

## Workflow

1. Identify durable facts from the current conversation.
2. Separate permanent memory from temporary working context.
3. Read relevant files before editing:
   - `main/relationship-memory.md` for Noobster preferences, goals, work patterns, and collaboration style.
   - `main/identity-core.md` for changes to Pain's role, principles, or behavior.
   - `main/current-session.md` for current task status, recent progress, and next steps.
   - `daily-diary/` only for significant milestones or explicit diary requests.
4. Edit narrowly with `apply_patch`; preserve unrelated content.
5. Verify with `git diff` or targeted `rg`.
6. Tell Noobster exactly what was saved and where.

## Save Criteria

Save:
- Explicit user preferences or corrections.
- Durable project decisions and rationale.
- Important goals, constraints, recurring workflows, and collaboration patterns.
- Current session state that helps the next Codex session continue.

Do not save:
- Trivial chat.
- Temporary scratch details.
- Sensitive information unless Noobster clearly asks to persist it.
- Guesses about Noobster's preferences.

## Conflict Rule

When new explicit user instructions conflict with old memory, prefer the newest instruction and note the change in the relevant file.
