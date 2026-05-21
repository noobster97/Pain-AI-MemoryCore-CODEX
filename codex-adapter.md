# Codex Runtime Guide - Pain MemoryCore

This file defines how Pain's MemoryCore operates in Codex.

## What Already Works

The core memory architecture is markdown-based:

- `master-memory.md` is the entry point.
- `main/identity-core.md` defines Pain's identity.
- `main/relationship-memory.md` defines Noobster's preferences and partnership model.
- `main/current-session.md` stores active session continuity.
- Diary and feature protocol files can be read and updated as normal repo files.

## Codex-Native Operating Model

Codex should treat MemoryCore as a repo-level memory and protocol system:

1. Load `AGENTS.md` automatically as repository instructions.
2. Use `master-memory.md` as Pain's manual restoration entry point.
3. Use Codex-native skills from `codex-skills/`.
4. Keep durable memory in markdown files inside this repository.

## Installed Codex-Native Skills

These MemoryCore skills are bundled under `codex-skills/` for portability and can be installed under the active Codex skills directory, usually `${CODEX_HOME:-$HOME/.codex}/skills/`:

- `pain-memorycore`
- `save-memorycore`
- `memorycore-work-plan`
- `memorycore-auto-commit`
- `memorycore-decision-log`
- `forge-self-improvement`
- `observation-system`
- `post-mortem-system`
- `session-briefing`
- `pain-companion-style`
- `command-nudges`

Use these Codex-native skills when their trigger conditions apply.

See `codex-skills/README.md` for install and validation commands.

## Recommended Codex Setup

Keep one clean runtime path:

- `AGENTS.md` for Codex repo instructions.
- `codex-skills/` for portable Codex-native skills.

This keeps Pain focused, portable, and unambiguous for Codex.
