# Skill File - Sample Format
*Reference template for creating SKILL.md files.*

```markdown
---
name: [skill-name]
description: "MUST use when [trigger condition 1], when user says '[phrase 1]',
             '[phrase 2]', '[phrase 3]', or when [contextual condition].
             Also triggers on '[alternative phrase]'."
---

# [Skill Name] - [Title]
*[One-line tagline describing the skill's purpose]*

## Activation

When this skill activates, output:

`[Activation message displayed to user]`

Then execute the protocol below.

## Context Guard

[Skill Name] activates only in appropriate contexts.

| Context | Status |
|---------|--------|
| **[Trigger context 1]** | ACTIVE - full protocol |
| **[Trigger context 2]** | ACTIVE - full protocol |
| **[Non-trigger context]** | DORMANT - do not activate |

## Protocol

### Step 1: [First Action]
- [ ] [Sub-task 1]
- [ ] [Sub-task 2]

### Step 2: [Second Action]
- [ ] [Sub-task 1]
- [ ] [Sub-task 2]

### Step 3: Confirm
- [ ] Display confirmation to user.
- [ ] Report what was done.

## Mandatory Rules

1. [Hard rule 1]
2. [Hard rule 2]
3. [Hard rule 3]

## Edge Cases

| Situation | Behavior |
|-----------|----------|
| **[Edge case 1]** | [How to handle it] |

## Level History

- **Lv.1** - Base: [Description of initial capability].
```

## Format Notes

- YAML frontmatter with `name` and `description` is required for auto-discovery.
- Start descriptions with `MUST use when...` for strong triggering.
- List specific trigger phrases and contextual conditions.
- Add a context guard when a skill could trigger too broadly.
- Keep protocols operational, concrete, and easy to execute.
