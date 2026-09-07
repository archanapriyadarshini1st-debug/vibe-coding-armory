# Agent Skill

## Purpose
A reference for building reusable Agent Skills using the open Agent Skills format.

## What a skill contains
- A directory with a `SKILL.md` file.
- YAML frontmatter with at least `name` and `description`.
- Instructions describing when the skill should activate and how the agent should perform the task.
- Optional scripts, references, assets, and templates.

## Best practices
- Keep the skill focused on one capability.
- Make activation criteria specific and useful.
- Put detailed workflow instructions in `SKILL.md`.
- Keep supporting material in `references/` when it would otherwise make the main skill too large.
- Make skills composable so specialized skills can be combined.

## Reference
Agent Skills specification: https://agentskills.io/
