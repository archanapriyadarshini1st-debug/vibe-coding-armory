# Humanize Writing

A focused upstream skill for making generated prose less formulaic while keeping it accurate, natural, and recognizably in the writer's voice.

## Upstream

- Repository: https://github.com/shir-danishyar/humanize
- Skill: `humanize-writing`
- License: MIT
- Install: `npx skills add shir-danishyar/humanize`

This Armory entry is a curated reference, not a copied implementation. Install the upstream skill using its own instructions and review its repository/license before adapting it.

## What it is useful for

- **Generation mode:** shape prose as it is being drafted, rather than relying only on a cleanup pass.
- **Rewrite mode:** revise an existing draft to remove repetitive or generic patterns.
- Reduce predictable vocabulary, stock transitions, repetitive sentence structures, generic openings/endings, excessive em-dash use, and overly uniform cadence.
- Calibrate register and voice from writing samples when appropriate.
- Use its documented pattern checks and deterministic Python linter as an editing aid.

## Recommended workflow

1. Draft for the actual audience, purpose, and facts.
2. Use the skill's generation mode when voice and natural variation matter from the start.
3. Run rewrite mode on a finished draft when it needs a cleanup pass.
4. Review every change for meaning, accuracy, tone, and whether it still sounds like the intended writer.
5. Keep useful technical terms, deliberate repetition, slang, fragments, and stylistic choices when they serve a purpose.

## Armory guardrails

- Improve authentic writing; do not treat this as an AI-detector evasion tool.
- Do not invent personal anecdotes, evidence, sources, quotations, or details to make prose seem human.
- Do not replace precise words with random synonyms just to increase vocabulary variation.
- Preserve the writer's intended voice and the text's factual meaning.
- AI detectors are unreliable indicators of authorship; no writing skill can guarantee a particular detector result.

## When to choose it

Choose **Humanize Writing** when you want a stronger generation-time approach to voice, rhythm, and predictable phrasing. Use the existing [Humanizer](humanizer.md) reference for a compact general editing checklist, or [Writing Craft](writing-craft.md) for broader drafting and editing guidance.
