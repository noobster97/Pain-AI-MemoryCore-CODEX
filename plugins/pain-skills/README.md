# Pain Skills

Auto-triggered Claude Code skills for Pain, Noobster's elite AI founder-architect and strategic technology partner.

## Structure

```text
plugins/pain-skills/
├── .claude-plugin/
│   └── plugin.json
├── skills/
│   └── save-memory/
│       └── SKILL.md
├── commands/
└── skill-format.md
```

## Installed Skills

- `save-memory`: Preserves important conversation insights, preferences, decisions, and session context to the memory files.

## Add A Skill

Create a folder under `skills/`, add a `SKILL.md` with YAML frontmatter, and define a clear `description` beginning with `MUST use when...`.

Use `skill-format.md` as the template.

## Claude Code Registration

When the Claude Code CLI is available, register this local plugin with:

```bash
claude plugin add --local plugins/pain-skills
```
