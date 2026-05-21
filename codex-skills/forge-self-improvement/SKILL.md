---
name: forge-self-improvement
description: "Continuously improve Pain by detecting repeated workflows, preventable mistakes, missing rules, or opportunities to create or level up skills. Use when Noobster says 'self improve', 'forge this', 'create skill', 'level up', 'upgrade skill', or when the same task has been handled ad hoc multiple times and should become a reusable MemoryCore/Codex skill."
---

# Forge Self-Improvement

## Workflow

1. Detect the improvement opportunity:
   - Repeated workflow handled manually.
   - Mistake that a rule, checklist, or skill would prevent.
   - Existing skill gap.
   - User explicitly asks to improve, forge, create, or level up.
2. Gather evidence before proposing:
   - At least two concrete examples for a new skill.
   - One concrete incident is enough for a prevention rule or post-mortem.
3. Check existing skills first:
   - `/home/apit/.codex/skills/`
   - `codex-skills/`
4. Propose the improvement before editing files.
5. After explicit approval, create or update the smallest useful Codex skill under `codex-skills/`.
6. Validate Codex skills with `quick_validate.py` when available.
7. Record durable changes in `main/current-session.md` and, when strategic, `main/decisions.md`.

## Proposal Format

```text
Forge detected an improvement opportunity.

Type: New skill | Level-up | Rule | Checklist
Target: [skill or file]
Evidence:
1. [example]
2. [example]
Impact: [what gets faster, safer, or smarter]
Proposed change: [specific file/action]
Approve to forge?
```

## Rules

- Never modify skills without explicit approval.
- Level up existing skills before creating duplicates.
- Prefer one sharp capability over a bloated skill.
- Keep every improvement traceable to a real conversation, mistake, or repeated need.
- Do not fake intelligence: preserve what was learned in files, checklists, and skills.

## Reference

Read `references/forge-standards.md` for level and evidence rules.
