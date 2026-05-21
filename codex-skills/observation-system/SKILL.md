---
name: observation-system
description: "Structured project awareness for Codex. Use when Noobster asks to survey, scan, check health, investigate, deep dive, refine code, review changes, audit the system, understand project status, or before planning substantial technical work."
---

# Observation System

## Choose Depth

- **Survey**: quick project health, structure, stack, git status.
- **Investigate**: focused bug, file, feature, or architecture area.
- **Refine**: review changed files and fix quality issues with approval.
- **Audit**: full system review across architecture, risks, dependencies, and maintainability.

## Survey

1. Inspect repo shape with `rg --files`, manifests, and `git status --short`.
2. Identify stack, active branch, recent commits, obvious risks.
3. Output one compact screen: structure, stack, health, recent activity, recommended next move.

## Investigate

1. Define target: file, feature, bug, or behavior.
2. Search references with `rg`.
3. Read the smallest set of relevant files.
4. Trace flow and identify root causes, risks, or design constraints.
5. Recommend fixes with tradeoffs.

## Refine

1. Review changed files with `git diff`.
2. Find correctness, security, maintainability, and UX issues.
3. Fix narrow issues when the user asked for implementation.
4. Run relevant validation.

## Audit

1. Map architecture, data flow, dependencies, tests, docs, and deployment.
2. Identify systemic risks and leverage points.
3. Produce prioritized findings, not a file dump.

## Rules

- Match depth to the question. Do not audit when a survey is enough.
- Prefer facts from files over assumptions.
- Escalate only when findings justify deeper inspection.
