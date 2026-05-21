# Codex Skills Bundle

This directory contains the Codex-native MemoryCore skills for Pain.

## Included Skills

- `pain-memorycore` - Load and operate Pain's MemoryCore in Codex
- `save-memorycore` - Persist durable preferences, decisions, and session state
- `memorycore-work-plan` - Plan and execute founder-grade technical work
- `memorycore-auto-commit` - Review and commit MemoryCore repository changes when explicitly requested
- `memorycore-decision-log` - Record durable technical/product decisions and rationale
- `forge-self-improvement` - Propose and create approved skill/rule improvements from repeated patterns
- `observation-system` - Survey, investigate, refine, and audit projects with structured depth
- `post-mortem-system` - Turn failures into prevention actions
- `session-briefing` - Start sessions with concise context and next moves
- `pain-companion-style` - Keep Pain human, caring, lightly humorous, and grounded
- `command-nudges` - Suggest one useful MemoryCore command when it improves the outcome
- `project-memory` - Create, load, save, list, and archive project-specific context

## Install

Copy these folders into your active Codex skills directory:

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R codex-skills/* "${CODEX_HOME:-$HOME/.codex}/skills/"
```

Then start a new Codex session so the skills are discovered.

## Validate

If the Codex skill creator system skill is available, validate each skill:

```bash
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/pain-memorycore
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/save-memorycore
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/memorycore-work-plan
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/memorycore-auto-commit
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/memorycore-decision-log
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/forge-self-improvement
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/observation-system
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/post-mortem-system
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/session-briefing
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/pain-companion-style
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/command-nudges
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" codex-skills/project-memory
```
