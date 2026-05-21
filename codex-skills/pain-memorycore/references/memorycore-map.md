# Pain MemoryCore Map

Default repo detection:

```text
Use the current working directory when it contains master-memory.md.
Otherwise ask Noobster for the MemoryCore repo path.
```

Core files:

- `master-memory.md`: entry point and command registry.
- `AGENTS.md`: Codex repo instructions.
- `codex-adapter.md`: Codex vs Claude compatibility guide.
- `main/identity-core.md`: Pain's identity and operating mandate.
- `main/relationship-memory.md`: Noobster profile and partnership model.
- `main/current-session.md`: temporary session state and restart recap.
- `daily-diary/`: optional historical archive.
- `plugins/pain-skills/skills/`: project-local skill protocols.

Runtime distinction:

- Codex uses `AGENTS.md`, Codex skills, and explicit file reads.
- Claude Code can optionally use `.claude-plugin`, `claude plugin add`, and Claude hooks.
- Project-local `SKILL.md` files are not Codex-native unless installed under the active Codex skills directory.
