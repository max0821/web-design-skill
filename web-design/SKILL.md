---
name: web-design
description: "Design, redesign, reconstruct, and implement visually polished websites with a visual-first workflow. Use for landing pages, homepages, marketing or product sites, dashboards, screenshot-to-code, image-to-HTML, mockup-to-code, pixel-accurate frontend reconstruction, responsive web design, design-system creation, visual prototypes, frontend visual fidelity, render-based visual QA, and requests to avoid generic AI-generated UI. Establish art direction, approve a visual target, decompose it into Block/Layer/Text/Geometry maps, resolve and lock assets, implement semantically, then render and iteratively fix the 1–3 dominant mismatches."
license: "MIT"
compatibility: "Agent Skills-compatible clients. Works best when browser, screenshot/rendering, image generation/editing, and interactive HTML tools are available."
metadata:
  version: "1.3.0"
  category: "design"
  author: "max0821"
  source: "https://github.com/max0821/web-design-skill"
---

# Web Design

**Version: 1.3.0**  
**Author: [max0821](https://github.com/max0821)**  
**Official source: https://github.com/max0821/web-design-skill**  
**License: MIT — commercial use permitted; copyright and license notice must be retained**

> Treat web design as a visual design discipline first and a code-generation task second. A page is unfinished if it merely renders; it must preserve design intent, visual hierarchy, coherence, fidelity, responsive continuity, and implementation integrity.

**Conversation language:** respond in the user's current conversation language unless the user explicitly requests another language. Do not inherit language from examples, metadata, or the default prompt.

## Use when

Use this skill for website/landing-page design, redesigns, screenshot/reference-to-code, image/mockup-to-HTML, visual prototypes, responsive UI, design-system work, rendered visual QA, or any request where the interface must feel intentionally designed rather than generic AI UI.

Do not activate merely because a task contains HTML/CSS. Pure backend, API, infrastructure, data-processing, or non-visual frontend logic is outside this skill unless interface or visual design is also requested.

## Core workflow

`Understand → Progressive Clarification → Art Direction → Visual Exploration → User Reaction → Approved Visual Target → Decompose → Coherence Contract → Resolve Assets → Implement → Render → Compare → Fix → Repeat`

For simple or already well-specified UI tasks, stages may be lightweight. For visually important marketing pages, redesigns, screenshot-to-code work, or image-first design, do not skip the stages that stabilize visual intent and implementation fidelity.

## Non-negotiable rules

1. **Evidence priority:** explicit user constraints and approved references outrank generic conventions. Once a visual concept is approved, it becomes the primary visual source of truth until the user changes direction.
2. **Progressive clarification:** ask only the highest-impact unresolved design question. Prefer 2–4 concrete options and recommend one when defensible. Never front-load a long questionnaire.
3. **Visual-first when appropriate:** for visually important pages without a strong supplied reference, strongly prefer visual exploration before final HTML. The first concept is not automatically approved.
4. **Attention control:** manage faces, saturated color, arrows, large numbers, floating UI, and oversized type as a limited attention budget. Establish a deliberate focal sequence.
5. **Coherence:** typography, surfaces, assets, composition, motion, and responsive states must belong to one visual language. Maintain a cross-cutting Token Map and Asset Style Contract.
6. **Approved target lock:** do not casually regenerate the whole page after approval. Local problems require local fixes.
7. **Semantic truth vs visual truth:** approved visual target controls appearance; real copy/user/live-site content controls semantic text. Exact text, buttons, metrics, labels, and structural UI should remain live HTML/CSS/SVG when possible.
8. **Render, don't infer:** judge implementation from the real rendered result, not source code alone.
9. **Dominant mismatch loop:** each refinement pass fixes only 1–3 highest-impact mismatches, then re-renders.
10. **Mobile is composition:** responsive design preserves focal hierarchy, image/text relationships, typography personality, and brand grammar; it is not desktop stacked vertically.
11. **Preserve architecture:** in an existing project, keep the user's stack, routing, component architecture, conventions, and business-critical structure unless a change is necessary and justified.

## Approved Visual Target → four maps

After approval, decompose the target into exactly four implementation maps:

- **Block Map** — sections, role, span, layout model, anchors, adjacency, mobile adaptation.
- **Layer Map** — visual layers, parent, position, size, z-order, prominence, structural/decorative role, implementation medium.
- **Text Map** — semantic copy, role, parent, wrapping, emphasis, semantic tag, live-text requirement.
- **Geometry Map** — canvas, section bounds, normalized ratios, insets, column ratios, alignment lines, overlap, crop, negative space.

The **Token Map** is a cross-cutting coherence contract shared by all four maps; it is not a fifth decomposition map.

## Asset Resolution Plan

Classify each significant visual layer as one of:

- live HTML / UI
- CSS / SVG
- existing / cropped asset
- clean local regeneration
- omit / simplify

For generated/replaced assets, define crop/aspect, alpha/background behavior, safe margins, pose, lighting, color, focal point, anchor box, expected placement, and forbidden changes when relevant.

If one approved asset is dirty or unusable, regenerate only the smallest useful local asset. After QA, mark it **LOCKED** and prevent later generations from changing its accepted role, crop, style, or placement without explicit approval.

## Implementation order

1. Page canvas and section proportions.
2. Primary alignment system.
3. Live typography structure.
4. Background/surface layers.
5. Hero or major visual assets.
6. Overlays and secondary composition details.
7. Service/content sections.
8. CTA/trust/support details.
9. Responsive translation.
10. Render comparison and iterative fixes.

Do not begin with decorative micro-details. Do not switch the user's implementation technology merely to simplify the design task.

## Render QA

After implementation:

1. Render the actual page at the target viewport.
2. Compare hierarchy, geometry, typography, crop, visual weight, color, surfaces, negative space, and responsive behavior against the approved target/reference.
3. Identify the 1–3 mismatches with the largest perceptual impact.
4. Fix only those mismatches.
5. Re-render and repeat until the remaining differences are low-impact or intentionally accepted.

Actively reject generic AI patterns when they contradict the art direction: repetitive equal cards, arbitrary gradients, excessive pills, decorative glass surfaces, default centered sections, weak hierarchy, or visually unrelated component styles.

## Reference loading

Load detailed references only when the task requires them:

- Art direction, clarification, visual exploration, feedback, attention: [references/art-direction-and-exploration.md](references/art-direction-and-exploration.md)
- Typography, visual grammar, tokens, asset style, composition, motion, brand drift: [references/visual-coherence-contract.md](references/visual-coherence-contract.md)
- Macro composition and Approved Visual Target locking: [references/approved-target-and-composition.md](references/approved-target-and-composition.md)
- Four maps, Asset Resolution Plan, local regeneration, asset lock: [references/decomposition-and-assets.md](references/decomposition-and-assets.md)
- HTML fidelity, screenshot comparison, mismatch repair, completion gate: [references/render-fidelity-contract.md](references/render-fidelity-contract.md)
- Mobile translation and interaction: [references/responsive-and-interaction.md](references/responsive-and-interaction.md)
- Compact reusable design-system guidance: [references/design-system.md](references/design-system.md)
- Compact visual-QA checklist: [references/visual-qa.md](references/visual-qa.md)
- Workflow examples: [references/workflow-examples.md](references/workflow-examples.md)

## Output behavior

Match the requested deliverable. If the user asks for visual exploration, produce concepts first. If they ask for an image, produce the visual. If they ask for code from an approved visual, decompose then implement. If they ask for critique, provide prioritized findings instead of silently redesigning.

Do not dump internal maps/checklists into every response. Use them internally unless exposing them helps the user evaluate a decision or continue implementation.

## Completion gate

Before declaring completion, verify:

- Design intent is clear and appropriate to the page job.
- Approved target/reference still controls the visual direction.
- Typography, assets, surfaces, composition, and motion are coherent.
- Important copy remains semantic/live.
- Generated assets have not drifted from locked contracts.
- Rendered hierarchy, geometry, crop, visual weight, and negative space are faithful.
- Mobile preserves the intended focal sequence and relationships.
- No dominant mismatch remains unreviewed.
- Existing project architecture and required functionality remain intact.

A technically valid page that looks generic is unfinished. A beautiful page that ignores business purpose is unfinished. A faithful screenshot match with brittle implementation is unfinished. The target is all of these at once: **design intent + visual hierarchy + visual coherence + stable visual specification + asset discipline + implementation fidelity + responsive continuity + implementation integrity**.
