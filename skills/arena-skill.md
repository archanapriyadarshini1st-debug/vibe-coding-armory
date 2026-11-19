# Arena Skill

A multi-agent tournament skill for improving a solution when a first attempt is not good enough.

## What it does
- Gives the same task to multiple sub-agents, each with a different reasoning/workflow strategy.
- Runs a single-elimination bracket where agents critique, defend, and revise competing solutions.
- Uses a written rubric to select a surviving solution.
- Keeps run state and agent outputs in a dedicated `.arena/` workspace; it does not directly apply the winning code changes.

## Best for
- comparing alternative implementations or architectures
- difficult debugging and problem-solving tasks
- evaluating competing product, UX, or technical approaches
- getting a stronger second pass when a normal retry is insufficient

## Important trade-offs
- The default 100-agent tournament can involve hundreds of sub-agent calls and substantial model usage.
- Use the smaller `--quick` mode (16 agents) or a lower `--agents N` value for routine tasks.
- The tournament's winner is the strongest candidate under its rubric, not a guarantee of correctness; review and test the result.

## Compatibility and requirements
Designed for Claude Code and its sub-agent workflow. Requires Python 3.8+; the bracket utility uses the Python standard library.

## Reference
- Repository: https://github.com/Jakeschincariol/arena-skill
- License: MIT
- Claude Code plugin marketplace: `/plugin marketplace add Jakeschincariol/arena-skill`
- Install: `/plugin install arena-skill@arena-skill`
- Skill source: https://github.com/Jakeschincariol/arena-skill/tree/main/skills/arena
