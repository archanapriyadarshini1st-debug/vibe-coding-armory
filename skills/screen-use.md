# screen-use Skill

Desktop computer-use capability for Windows agents: see the screen, locate UI elements, click, type, scroll, and perform autonomous visual workflows through MCP or the Python SDK.

## Best for
- screenshot-based desktop perception
- Windows GUI automation
- UI element discovery through accessibility + vision
- mouse and keyboard actions
- cross-application workflows
- observe → think → act → verify loops
- local VLM workflows through Ollama

## Reference
https://github.com/tongriyaotxt/screen-use

## Armory guidance
Prefer semantic element targeting and accessibility-tree inspection before raw coordinates. Re-observe after major UI changes. Use screenshots to verify important actions. Treat computer-use as control of the user's real desktop and keep destructive or externally visible actions gated by confirmation.
