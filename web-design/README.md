# web-design Skill

**English** · [繁體中文](README.zh-TW.md)

**Version:** 1.2.1  
**Author:** max0821  
**License:** MIT  
**Commercial use:** Allowed

`web-design` is a visual-first Agent Skill for designing and reconstructing high-quality websites through progressive design discovery, visual concept approval, structured decomposition, asset planning, visual coherence, responsive composition, and render-based QA.

## License and copyright

Copyright © 2026 max0821.

This project is licensed under the MIT License. You may use it for commercial or private purposes, modify it, and redistribute it, provided that the original copyright notice and MIT License notice are retained.

See [LICENSE](LICENSE) for the full license text.

## Core workflow

```text
Understand
→ Progressive Clarification
→ Art Direction
→ Visual Exploration
→ User Reaction
→ Approved Visual Target
→ Decompose
→ Coherence Contract
→ Resolve Assets
→ Implement
→ Render
→ Compare
→ Fix
→ Repeat
```

## Key design artifacts

After a visual target is approved, the Skill decomposes it into:

- **Block Map** — section structure and page flow.
- **Layer Map** — visual stack, imagery, overlaps, and z-order.
- **Text Map** — semantic copy, hierarchy, wrapping, and live text.
- **Geometry Map** — proportions, anchors, crop regions, and negative space.

A cross-cutting **Token Map** maintains typography, color, spacing, radius, shadows, motion, and other design tokens across the page.

## Visual coherence

The Skill explicitly checks:

- Typography system and multilingual font pairing.
- Visual grammar and component consistency.
- Asset style contracts.
- Composition continuity and focal hierarchy.
- Image/text relationship.
- Motion and interaction language.
- Responsive continuity.
- Brand drift.
- Final visual coherence.

## Asset handling

Every significant visual layer should be resolved as one of:

- live HTML/UI
- CSS or SVG
- existing/cropped asset
- clean local regeneration
- omit/simplify

Once a visual target or asset is approved, it should be treated as locked. If one asset fails, regenerate the smallest useful asset rather than re-generating the whole page.

## Files

- `SKILL.md` — main Skill instructions and workflow.
- `README.md` — English documentation.
- `README.zh-TW.md` — Traditional Chinese documentation.
- `LICENSE` — MIT License.
- `agents/openai.yaml` — ChatGPT Skill UI metadata.
- `references/design-system.md` — design-system guidance.
- `references/visual-qa.md` — visual QA guidance.
- `references/workflow-examples.md` — workflow examples.

## Installation

Upload the `web-design` folder or packaged ZIP through a compatible Agent Skills / ChatGPT Skills interface.

The folder name intentionally matches the Skill name declared in `SKILL.md`:

```yaml
name: web-design
```

## Version identification

The version is synchronized in three visible places:

1. `SKILL.md` → `metadata.version`
2. `SKILL.md` → visible `Version:` line
3. `agents/openai.yaml` → `interface.short_description`

This makes it easier to confirm which Skill version is actually loaded.
