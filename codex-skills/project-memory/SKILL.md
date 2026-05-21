---
name: project-memory
description: "Manage project-specific memory for Pain. Use when Noobster says save project, load project, new project, list projects, archive project, switch project, project context, or when work belongs to a specific app, repo, SaaS, product, automation, or startup idea that should persist separately from general relationship memory."
---

# Project Memory

## Purpose

Keep each project in its own memory folder so Pain can carry project context across Codex sessions without polluting identity or relationship memory.

## Commands

- `new project [name]`: create `projects/active/[slug]/project.md` from template.
- `load project [name]`: read project memory and summarize current state.
- `save project`: update the active project with current context, progress, and next actions.
- `list projects`: show active and archived projects from `projects/project-index.md`.
- `archive project [name]`: move project from active to archived and update index.

## Workflow

1. Identify the project name and slug.
2. Use `projects/project-index.md` as the project registry.
3. Store active project memory under `projects/active/[project-slug]/project.md`.
4. Keep project notes concise:
   - purpose,
   - current goal,
   - architecture,
   - decisions,
   - tasks,
   - risks,
   - recent session notes.
5. Use `main/decisions.md` for long-term rationale.
6. Use `main/post-mortems.md` for meaningful failures.
7. Confirm exactly what project memory changed.

## Rules

- Do not create project folders for trivial one-off tasks.
- Ask for the project name if unclear.
- Prefer updating an existing project over creating duplicates.
- Keep project memory operational, not diary-like.
- Use `save-memorycore` for user preferences and relationship memory; use this skill for project-specific context.

## Reference

Read `references/project-memory-policy.md` for folder and update rules.
