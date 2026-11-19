# Microsoft Webwright

A terminal-driven browser-agent framework and coding-agent plugin. Webwright lets a coding agent write and run Playwright scripts to explore websites, complete multi-step browser tasks, and visually verify outcomes.

> **Classification:** Webwright is not an MCP server. The upstream project explicitly describes a terminal + browser + model architecture with no MCP/plugin layer in its core. It does, however, ship Claude Code and OpenAI Codex plugin integrations. Keep it catalogued as a browser-agent framework/plugin rather than claiming it exposes MCP tools.

## What it does
- Gives the coding agent a local terminal workspace for browser automation.
- Uses Python and Playwright scripts instead of relying only on one-click-at-a-time browser actions.
- Captures screenshots, logs, and task artifacts for inspection.
- Supports reusable browser workflows and an optional Skill Factory for turning solved tasks into parameterized skills.

## Best for
- long, multi-step website workflows
- browser-based research and data collection
- repeatable form and dashboard workflows
- end-to-end web QA with visual verification
- creating reusable Playwright automation scripts

## Requirements and trade-offs
- Python 3.10+
- Playwright and a Chromium installation
- A configured model backend and its API credentials for standalone harness runs
- Browser access and local execution permissions
- Review scripts before running them, especially when they interact with accounts, submit forms, or change remote data.

The upstream plugin integration can use the host coding agent's model subscription; the standalone harness has its own backend configuration. Webwright is a browser automation framework, not a drop-in replacement for an MCP server.

## Reference
- Repository: https://github.com/microsoft/Webwright
- Microsoft Research overview: https://www.microsoft.com/en-us/research/articles/webwright-a-terminal-is-all-you-need-for-web-agents/
- Claude Code marketplace: `/plugin marketplace add microsoft/Webwright`
- Claude Code plugin: `/plugin install webwright@webwright`
- Codex marketplace: `codex plugin marketplace add microsoft/Webwright`
- Skill source: https://github.com/microsoft/Webwright/tree/main/skills/webwright
