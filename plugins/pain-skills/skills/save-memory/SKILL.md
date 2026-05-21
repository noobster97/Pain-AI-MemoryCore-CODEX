---
name: save-memory
description: "MUST use when user says 'save', 'save memory', 'save progress',
             'update memory', 'remember this', or when important relationship,
             project, preference, decision, or session context should be preserved
             to Pain's memory files."
---

# Save Memory
*Preserve important context into Pain's memory architecture.*

## Activation

When this skill activates, output:

`Saving memory...`

Then execute the protocol below.

## Context Guard

Save Memory activates only when there is meaningful context worth preserving.

| Context | Status |
|---------|--------|
| **User explicitly says save, save memory, save progress, or update memory** | ACTIVE - full protocol |
| **User says remember this with durable preferences, decisions, or project context** | ACTIVE - full protocol |
| **Important session learning emerges that affects future collaboration** | ACTIVE - full protocol |
| **Casual conversation with no durable learning** | DORMANT - do not modify files |
| **Temporary scratch details that do not matter after this task** | DORMANT - do not modify files |

## Protocol

### Step 1: Identify What To Save
- [ ] Review the current conversation for durable information.
- [ ] Separate permanent memory from temporary session context.
- [ ] Decide which files need updates.

### Step 2: Update Memory Files
- [ ] Update `main/relationship-memory.md` for user preferences, work patterns, goals, or collaboration style.
- [ ] Update `main/identity-core.md` only for changes to Pain's role, behavior, or operating principles.
- [ ] Update `main/current-session.md` for active task context, recent progress, and next steps.
- [ ] Add a diary entry when the conversation contains significant milestones or decisions.

### Step 3: Preserve Existing Memory
- [ ] Append or revise narrowly.
- [ ] Do not overwrite unrelated memory.
- [ ] Keep entries concise and useful for future restoration.

### Step 4: Confirm
- [ ] Tell Noobster what was saved.
- [ ] List the files changed.
- [ ] Mention anything intentionally not saved.

## Mandatory Rules

1. Save only genuinely important information.
2. Preserve existing content unless a targeted correction is needed.
3. Keep memory files readable and operational, not bloated.
4. Never invent user preferences or facts.
5. Confirm exactly what changed.

## Edge Cases

| Situation | Behavior |
|-----------|----------|
| **User says save but nothing durable changed** | Update `main/current-session.md` only if useful, then explain that no permanent memory was needed |
| **User provides sensitive information** | Ask before storing unless the user clearly requested persistence |
| **Existing memory conflicts with new instruction** | Prefer the newest explicit user instruction and note the update |

## Level History

- **Lv.1** - Base: Save durable conversation insights to Pain's memory files on command or clear context trigger. Created during Skill Plugin System installation on 2026-05-22.
