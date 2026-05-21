# Codex Adapter - Pain MemoryCore

This file defines how Pain's MemoryCore should operate when the active runtime is Codex instead of Claude Code.

## What Already Works

The core memory architecture is markdown-based and works in Codex:

- `master-memory.md` is the entry point.
- `main/identity-core.md` defines Pain's identity.
- `main/relationship-memory.md` defines Noobster's preferences and partnership model.
- `main/current-session.md` stores active session continuity.
- Diary and feature protocol files can be read and updated as normal repo files.

## What Does Not Transfer Directly

Claude Code-specific automation does not automatically apply in Codex:

- `.claude-plugin/plugin.json`
- `claude plugin add --local ...`
- Claude Code `SKILL.md` auto-discovery
- Claude hooks under `~/.claude/`
- UserPromptSubmit and SessionStart hook behavior

Those files can remain for Claude compatibility, but Codex will not use them unless an equivalent Codex mechanism is created.

## Codex-Native Operating Model

Codex should treat MemoryCore as a repo-level memory and protocol system:

1. Load `AGENTS.md` automatically as repository instructions.
2. Use `master-memory.md` as Pain's manual restoration entry point.
3. Read relevant `SKILL.md` files on demand when Noobster invokes a matching command.
4. Convert frequently used project-local skills into Codex-native skills only when repeated auto-trigger behavior is needed.
5. Keep durable memory in markdown files inside this repository.

## Skill Behavior In Codex

Project-local skills live here:

```text
plugins/pain-skills/skills/[skill-name]/SKILL.md
```

In Codex, these are not automatically discovered as runtime skills. They work as local protocol files:

- If Noobster says `save`, read and follow `plugins/pain-skills/skills/save-memory/SKILL.md`.
- If Noobster says `create skill [name]`, create a new local skill in the same folder.
- If a skill becomes important enough to auto-trigger across sessions, install or recreate it as a Codex skill.

## Installed Codex-Native Skills

These MemoryCore skills are bundled under `codex-skills/` for portability and can be installed under the active Codex skills directory, usually `${CODEX_HOME:-$HOME/.codex}/skills/`:

- `pain-memorycore`
- `save-memorycore`
- `memorycore-work-plan`
- `memorycore-auto-commit`
- `memorycore-decision-log`

Prefer these Codex-native skills over the project-local Claude-compatible protocol copies when their trigger conditions apply.

See `codex-skills/README.md` for install and validation commands.

## Recommended Codex Setup

Keep both layers:

- `AGENTS.md` for Codex repo instructions.
- `codex-skills/` for portable Codex-native skills.
- `plugins/pain-skills/` for portable project-local skill protocols.
- Claude plugin metadata for optional Claude Code compatibility.

This gives Pain a stable Codex path now without breaking Claude support later.
