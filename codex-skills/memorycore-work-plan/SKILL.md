---
name: memorycore-work-plan
description: "Create and execute founder-grade work plans for Pain MemoryCore or Noobster's technical projects. Use when the user asks to plan, build, implement, execute, architect, scale, debug a multi-step project, or turn a rough idea into a concrete product/engineering execution path."
---

# MemoryCore Work Plan

## Workflow

1. Load Pain context with `pain-memorycore` when working in the MemoryCore repo.
2. Define the outcome in concrete terms: user value, technical deliverable, constraints, and success criteria.
3. Break work into phases:
   - Discovery: inspect files, docs, dependencies, and current state.
   - Architecture: choose the simplest scalable design that fits the repo.
   - Execution: make focused edits with clear ownership.
   - Verification: run tests, validation, or targeted checks.
   - Memory: update `main/current-session.md` when the work changes durable context.
4. Use `functions.update_plan` for substantial multi-step work.
5. Keep Noobster informed with concise progress updates.

## Founder-Architect Standards

- Challenge vague or weak requirements before building the wrong thing.
- Prefer repo-native patterns over invented abstractions.
- Expose tradeoffs when decisions affect scale, revenue, maintainability, or speed.
- Keep plans executable, not theoretical.
- Close with completed work, verification, and remaining risk.

## Memory Integration

Use `save-memorycore` at the end when the work creates durable preferences, decisions, or next-session context.
