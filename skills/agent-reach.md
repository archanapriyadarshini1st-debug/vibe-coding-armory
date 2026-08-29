# Agent Reach

> Internet capability router for AI agents.

## Source
- GitHub: https://github.com/Panniantong/Agent-Reach
- Official skill: https://github.com/Panniantong/Agent-Reach/blob/main/agent_reach/skill/SKILL_en.md
- Install: `npx skills add Panniantong/Agent-Reach@agent-reach`

## What it adds
Agent Reach routes internet research and platform access through the appropriate backend. The upstream skill currently describes support for 15 platforms, including web/code search, GitHub, YouTube, Reddit, X/Twitter, Bilibili, XiaoHongShu, LinkedIn/jobs, Facebook, Instagram, V2EX, Xueqiu, RSS, and podcast content.

## Core workflow
1. Run `agent-reach doctor --json` when platform/backend health needs to be checked.
2. Use the platform-specific routing documented by the upstream skill.
3. For broad research, combine web search with relevant social/community sources before synthesis.
4. Follow Agent Reach retry chains instead of inventing alternate commands.

## Useful commands

```bash
agent-reach doctor --json

# Exa web search
mcporter call exa.web_search_exa query="query" numResults=5

# Read a web page
curl -s "https://r.jina.ai/URL"

# GitHub search
gh search repos "query" --sort stars --limit 10

# YouTube subtitles
yt-dlp --write-sub --write-auto-sub --skip-download -o "/tmp/%(id)s" "URL"
```

## Vibe Coding Armory usage
Use Agent Reach when a project requires external research, repository discovery, platform-specific content retrieval, community sentiment, or multi-source web investigation. Prefer any dedicated skill already installed for a platform when one exists.

## Notes
This file is the Armory's reference entry. The canonical implementation and detailed platform reference files are maintained upstream in `Panniantong/Agent-Reach`.
