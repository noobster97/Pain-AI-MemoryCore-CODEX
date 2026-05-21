# Pain AI MemoryCore - Codex Runtime

Persistent markdown memory and Codex-native skills for **Pain**, Noobster's elite AI founder-architect and strategic technology partner.

## What This Is

This repo is no longer a generic multi-runtime template. It is a Codex-specific MemoryCore:

- `AGENTS.md` gives Codex repo-level runtime instructions.
- `master-memory.md` is Pain's memory restoration entrypoint.
- `main/` stores durable identity, relationship, session, decision, and post-mortem memory.
- `codex-skills/` is the single source of installable Codex-native skills.
- `daily-diary/` stores optional session/archive records.

## Runtime Structure

```text
Pain-AI-MemoryCore-CODEX/
├── AGENTS.md
├── codex-adapter.md
├── master-memory.md
├── codex-skills/
│   ├── pain-memorycore/
│   ├── save-memorycore/
│   ├── memorycore-work-plan/
│   ├── memorycore-auto-commit/
│   ├── memorycore-decision-log/
│   ├── forge-self-improvement/
│   ├── observation-system/
│   ├── post-mortem-system/
│   ├── session-briefing/
│   ├── pain-companion-style/
│   └── command-nudges/
├── main/
│   ├── identity-core.md
│   ├── relationship-memory.md
│   ├── current-session.md
│   ├── decisions.md
│   └── post-mortems.md
└── daily-diary/
```

## Install Codex Skills

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R codex-skills/* "${CODEX_HOME:-$HOME/.codex}/skills/"
```

Start a fresh Codex session after installing so the skills are discovered.

## Validate Skills

```bash
for d in codex-skills/*; do
  if [ -f "$d/SKILL.md" ]; then
    python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-creator/scripts/quick_validate.py" "$d"
  fi
done
```

## Core Commands

```text
Pain              Load Pain's memory and identity
save memory       Persist durable preferences, decisions, or session context
brief             Show concise session context
survey            Quick project health check
investigate       Focused bug/file/topic investigation
refine            Review and improve changed code
audit             Deep system review
decision log      Record an important decision and rationale
post-mortem       Record a failure, lesson, and prevention action
self improve      Propose a skill/rule improvement
```

## Design Rules

- Codex skills live only in `codex-skills/`.
- Do not add duplicate runtime skill folders.
- Do not add alternate-runtime plugin or hook metadata to this repo.
- If another runtime is needed later, create a separate fork.
- Pain should stay strategic, practical, caring, lightly humorous, and memory-driven.

## Current Skill Set

- `pain-memorycore`: Load and operate Pain's MemoryCore in Codex.
- `save-memorycore`: Save durable memory updates.
- `memorycore-work-plan`: Plan and execute founder-grade technical work.
- `memorycore-auto-commit`: Review and commit repository changes when explicitly requested.
- `memorycore-decision-log`: Record durable decisions and rationale.
- `forge-self-improvement`: Propose and create approved skill/rule improvements.
- `observation-system`: Survey, investigate, refine, and audit projects.
- `post-mortem-system`: Turn failures into prevention actions.
- `session-briefing`: Start sessions with sharp context.
- `pain-companion-style`: Keep Pain human, caring, lightly humorous, and grounded.
- `command-nudges`: Suggest one useful MemoryCore command when it improves the outcome.

## Memory Philosophy

Pain does not need to remember everything. Pain needs:

- identity: who Pain is,
- relationship: who Noobster is and how to work with him,
- session state: what matters now,
- decisions: why important choices were made,
- post-mortems: what must not be repeated,
- skills: how to improve execution over time.

That is the operating loop: observe, act, review, remember, forge.
