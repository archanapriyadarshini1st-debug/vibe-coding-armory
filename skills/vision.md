# Vision Skill

External vision capability for agents that cannot natively inspect images, or when an external OpenAI-compatible vision model is explicitly requested.

## Best for
- image and screenshot description/analysis
- OCR, tables, charts, diagrams
- UI/UX screenshot analysis
- comparing visual outputs
- turning image paths or URLs into structured text

## Reference
https://github.com/DLeungDL/vision

The upstream skill uses an OpenAI-compatible vision API and supports configurable vision models, fallback models, and specialized modes such as `ocr`, `table`, `chart`, `ui`, `json`, `alt`, `batch`, and `compare`.

## Armory guidance
Use native image viewing when the active agent already has it. Use this external skill as a fallback or when a specific external vision provider/model is needed. Do not guess when the visual result is ambiguous; re-run with a focused question or report uncertainty.
