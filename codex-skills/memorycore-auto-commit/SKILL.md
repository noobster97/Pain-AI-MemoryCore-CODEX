---
name: memorycore-auto-commit
description: "Review and commit MemoryCore repository changes. Use when the user asks to commit, save changes to git, create a git commit, checkpoint the repo, or after completing a coherent MemoryCore feature when a structured commit is requested."
---

# MemoryCore Auto Commit

## Workflow

1. Inspect status with `git status --short`.
2. Review relevant diffs with `git diff` and, if needed, `git diff --stat`.
3. Separate your changes from unrelated user changes. Never revert unrelated changes.
4. Run relevant validation before committing when feasible.
5. Stage only intended files.
6. Commit with a concise message:
   - `feat: ...` for new memory features or skills
   - `docs: ...` for documentation-only updates
   - `chore: ...` for setup or cleanup
   - `fix: ...` for corrections
7. Report commit hash, files committed, validation run, and any skipped checks.

## Guardrails

- Do not commit without an explicit user request.
- Do not include secrets, local machine-only artifacts, or accidental generated clutter.
- Do not run destructive git commands unless explicitly requested.
- If unrelated changes are present, mention them and leave them unstaged.

## MemoryCore Notes

Memory files, Codex skills, and setup diary entries may belong in the same commit only when they are part of one coherent change.
