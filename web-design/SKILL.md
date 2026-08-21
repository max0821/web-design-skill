---
name: web-design
description: "Design and implement high-quality website interfaces through progressive design discovery, visual concept generation, reference decomposition, asset planning, faithful implementation, responsive composition, and iterative visual QA. Use for landing pages, homepages, product sites, dashboards, redesigns, screenshot-to-code, visual prototypes, UI sections, and any request where the rendered website must feel intentionally designed rather than generic AI-generated UI."
compatibility: "Agent Skills-compatible clients. Works best when browser, screenshot/rendering, image generation/editing, and interactive HTML tools are available."
metadata:
  version: "1.2.1"
  category: "design"
  author: "max0821"
  license: "MIT"
---

# Web Design

**Version: 1.2.1**  
**Author: max0821**  
**License: MIT — commercial use permitted with attribution/license notice retained**  
*Visual Coherence update: typography system, visual grammar, design tokens, asset style contracts, composition continuity, motion language, responsive continuity, and brand-drift QA.*

> Treat web design as a visual design discipline first and a code-generation task second. A page is not complete merely because it renders or functions. It must have clear design intent, controlled visual hierarchy, faithful reconstruction, and implementation integrity.

## Use When

Use this skill for:

- New website or landing-page design.
- Homepage or section redesign.
- Screenshot/reference-to-HTML implementation.
- Interactive web prototype or visual concept.
- Product, marketing, editorial, portfolio, ecommerce, community, SaaS, admin, or game-related web UI.
- Responsive desktop/mobile web design.
- Existing website restyling where visual quality or brand expression matters.
- Requests to make a page feel professional, distinctive, premium, playful, editorial, technical, branded, youthful, energetic, or less AI-generated.
- Visual matching and refinement of rendered HTML against a target design.

Do not activate merely because a task contains HTML/CSS. Pure backend, data-processing, API, infrastructure, or non-visual frontend logic is outside this skill unless the user also asks for interface or visual design.

## Core Objective

Use one continuous workflow:

`Understand → Progressive Clarification → Art Direction → Visual Exploration → User Reaction → Approved Visual Target → Decompose → Coherence Contract → Resolve Assets → Implement → Render → Compare → Fix → Repeat`

For simple or already well-specified UI tasks, some stages may be lightweight. For visually important marketing pages, redesigns, screenshot-to-code work, or image-first design, do not skip the stages that stabilize visual intent and implementation fidelity.

Design intent, visual fidelity, visual coherence, and implementation integrity are one problem, not separate tasks.

Treat quality as three parallel visual axes plus engineering integrity:

- **Design Intent** — the page has a deliberate visual and business thesis.
- **Visual Fidelity** — implementation preserves the approved target.
- **Visual Coherence** — typography, assets, surfaces, composition, motion, and responsive states still belong to one design language.
- **Implementation Integrity** — the result remains maintainable, semantic, accessible, and compatible with the user's architecture.

---

# 1. Priority of Evidence

When deciding what the page should look like, use this priority order:

1. Explicit user constraints and business goal.
2. User-approved visual concept, screenshot, image, Figma export, brand guide, or marked-up reference.
3. Existing live site, product assets, copy, and established brand language.
4. Other references explicitly requested by the user.
5. A newly established art direction created by this skill.

Never overwrite strong supplied evidence with generic design conventions.

Once the user approves a visual concept, it becomes the primary visual source of truth until the user explicitly changes direction.

---

# 2. Progressive Design Discovery

Do not front-load the user with a long design questionnaire.

When clarification is necessary:

1. Identify the single highest-impact unresolved design decision.
2. Prefer 2–4 concrete options over open-ended questions.
3. Recommend one option when there is a defensible professional preference.
4. Let the user choose, reject, or react.
5. Resolve later decisions only when they become relevant.

Prefer a design conversation over a requirement form.

Good examples:

- `A. 文案主導 / B. 圖文融合 / C. 場景主導`
- `A. 價格直接打 / B. 先打價值`
- `A. 保留桌機構圖 / B. 手機簡化 / C. 手機重新設計`

Do not ask questions whose answers can be safely inferred from the live site, existing copy, supplied references, or the user's previous choices.

The purpose is to reduce cognitive load, avoid unnecessary back-and-forth, and prevent solving low-impact details before the core visual direction is known.

---

# 3. Understand the Actual Design Problem

Determine:

- Page job.
- Audience.
- Primary action / conversion goal.
- Content hierarchy.
- Brand constraints.
- Device priorities.
- Existing information architecture that must be preserved.
- Whether the user wants exploration, a polished visual concept, production code, or faithful reproduction.

For redesigns, inspect the existing product or live site when available. Preserve business-critical structure unless there is a justified reason to change it.

Do not confuse "more modern" with "more generic".

---

# 4. Establish Art Direction Before Layout

Before writing final UI code, establish an internal design brief containing:

- **Visual concept** — aesthetic thesis in one sentence.
- **Emotional register** — precise, energetic, premium, playful, editorial, utilitarian, cinematic, technical, youthful, etc.
- **Reference grammar** — design traditions or visual systems being borrowed from.
- **Typography strategy** — display/body relationship, scale contrast, density, weight, rhythm.
- **Composition strategy** — symmetry/asymmetry, whitespace, overlap, edge alignment, section rhythm, dominant focal areas.
- **Surface/shape language** — borders, radius, shadows, panels, lines, frames, texture.
- **Color logic** — background, surface, text, accent, semantic roles, contrast behavior.
- **Image/illustration strategy** — photo, illustration, 3D, UI composite, scene, cutout, etc.
- **Interaction personality** — restrained, mechanical, expressive, editorial, playful, kinetic, etc.

The brief may remain internal unless the user needs to evaluate competing directions.

A text-only art direction is not always a sufficient visual specification.

---

# 5. Visual Exploration Before Implementation

For visually important marketing pages, homepages, landing pages, campaign pages, brand sites, and redesigns without a strong supplied reference, strongly prefer visual exploration before final implementation.

Recommended flow:

`Understand → Resolve Highest-Impact Unknowns → Art Direction → Generate Visual Concept → Ask for User Reaction → Refine → Approve → Implement`

Use image generation when composition, imagery, background treatment, visual energy, spatial rhythm, visual weight, or brand expression are central to the task.

Do not treat image generation as decoration. Use it as a visual-specification step.

When exploration is useful, prefer a small number of meaningfully different directions rather than many near-duplicates.

Examples of distinct directions:

- Editorial / magazine.
- Industrial / control-system.
- Experimental tech brand.
- Social / creator culture.
- Lifestyle / commercial photography.
- Illustration-led brand system.

Do not generate multiple directions when the user has already approved one.

---

# 6. Concept Review and User Feedback

After generating a visual concept, do not immediately treat it as approved.

Obtain the user's reaction before moving to implementation when the environment permits a follow-up turn.

Interpret feedback in terms of dominant visual variables:

- Focal point.
- Visual weight.
- Hierarchy.
- Image-to-type balance.
- Density.
- Composition.
- Energy.
- Color dominance.
- Imagery intensity.
- Interaction cues.
- Brand character.

When the user says something like "右邊太重", translate that into the underlying visual problem rather than applying arbitrary size reductions.

Fix only 1–3 dominant issues per iteration.

Prefer small directional choices over broad open-ended questions when another decision is required.

---

# 7. Visual Weight Control

Explicitly evaluate visual weight.

Strong attention attractors include:

- Human faces.
- Large photography.
- Saturated color.
- High contrast.
- Large metrics.
- Arrows.
- Floating UI.
- Reaction icons.
- Bright badges.
- Dense clusters of small elements.
- Large display typography.

Do not allow several strong attractors to compete with the primary message unless intentional.

For conversion-focused hero sections, establish a deliberate attention sequence, for example:

`Primary Message → Supporting Visual Evidence → CTA → Secondary Details`

The supporting image should reinforce the focal hierarchy rather than compete with it.

---

# 8. Build a Visual System

Create a small coherent system rather than styling each element independently.

At minimum establish:

- Type scale and hierarchy.
- Spacing rhythm.
- Container and alignment rules.
- Color roles.
- Border/radius/shadow rules.
- Reusable component grammar.
- Image treatment rules.
- Interaction/state rules.
- Responsive behavior.

Use components because repeated semantic patterns exist, not because every piece of content deserves a card.

A page can use cards, gradients, pills, shadows, or glass surfaces, but only when the product and art direction justify them.

## 8.1 Typography System

Typography is a system, not a per-section styling choice.

Define a deliberate typographic grammar before implementation:

- Display / hero.
- Heading levels.
- Body.
- Label / eyebrow / metadata.
- Numeric / price / metric treatment.
- Chinese / Latin font pairing when multilingual content exists.
- Allowed weights.
- Type scale.
- Line-height.
- Letter-spacing.
- Maximum headline line count when composition depends on wrapping.
- Chinese punctuation and line-break behavior when relevant.
- Mobile typography overrides.
- Tabular or mono numerals when metrics require alignment.

Do not change typographic personality section by section merely to create novelty.

When a reference uses typography as a major visual mass, preserve its scale, line breaks, contrast, and density as part of composition rather than treating type as content placed afterward.

## 8.2 Visual Grammar / Style Consistency

Define the reusable visual language of the page:

- Radius grammar.
- Border and stroke grammar.
- Shadow grammar.
- Surface hierarchy.
- Button shape family.
- Card family.
- Icon grammar.
- Illustration grammar.
- Photography treatment.
- Highlight / emphasis style.
- Divider / line language.
- Accent-color usage.
- Texture / grain / glow rules when used.

Individual sections may vary in composition, but they must still look like the same brand and the same design system.

Do not let one page drift from editorial photography to glassmorphism to dashboard cards to hand-drawn illustration without an explicit unifying concept.

## 8.3 Token Map

The four decomposition maps remain **Block / Layer / Text / Geometry**.

In addition, maintain a cross-cutting **Token Map** that translates visual decisions into reusable implementation variables. It is not a fifth decomposition map; it is the coherence contract shared by all four maps.

At minimum define when relevant:

- Color tokens.
- Typography tokens.
- Spacing rhythm.
- Container widths and gutters.
- Radius tokens.
- Border / stroke tokens.
- Shadow tokens.
- Z-index layers.
- Motion duration and easing.
- Breakpoint logic.
- Image treatment variables.

Prefer semantic tokens such as `--surface-primary`, `--accent-live`, `--text-muted`, `--radius-card`, or equivalent framework tokens over unrelated one-off values.

A reference may contain small visual variation, but implementation should resolve that variation into the smallest coherent token system that preserves the design.

## 8.4 Asset Style Contract

When multiple assets are generated, edited, extracted, or sourced independently, define an **Asset Style Contract** before producing replacements.

The contract may specify:

- Asset medium: photo / illustration / 3D / UI composite / icon / texture.
- Camera angle and perspective.
- Lighting direction and softness.
- Color temperature.
- Saturation and contrast.
- Depth of field.
- Subject scale.
- Crop behavior.
- Edge treatment / cutout quality.
- Background transparency or background behavior.
- Visual age / cultural register / brand mood.
- Rendering detail level.

Every locally regenerated asset must inherit this contract unless the approved target clearly requires a deliberate exception.

Do not allow separately generated assets to become visually incompatible merely because each looks good in isolation.

## 8.5 Composition Consistency

Maintain a page-level composition grammar across sections. Track:

- Primary alignment axes.
- Asymmetry logic.
- Whitespace rhythm.
- Section density pattern.
- Full-bleed versus contained behavior.
- Overlap rules.
- Edge-entry / edge-exit behavior.
- Repeated spatial motifs.

A bold hero followed by mechanically centered equal-card sections usually indicates composition drift.

Different sections may have different jobs and densities, but their spatial logic should feel intentionally related.

## 8.6 Focal Hierarchy Contract

For every important viewport, explicitly identify:

1. Primary focal point.
2. Supporting focal point.
3. Primary CTA.
4. Tertiary information cluster.

Treat visual attention as a limited budget. Human faces, saturated color, arrows, large numbers, motion, floating UI, large icons, and oversized display type all consume attention.

If several high-attention elements compete simultaneously, reduce, relocate, desaturate, simplify, or sequence them unless deliberate visual competition is part of the art direction.

## 8.7 Section Role Model

For important marketing or narrative pages, every major section should have a clear role in the page journey, for example:

- Hero — attract + explain.
- Proof — reduce doubt.
- Services / product — clarify the offer.
- Process — explain how it works.
- Pricing — reduce purchase friction.
- FAQ — resolve objections.
- CTA — convert.

A section should not become visually dominant merely because it can. Its visual intensity should match its narrative role.

Do not make every section shout at equal volume.

## 8.8 Image / Text Relationship

For each visually important block, identify its relationship mode:

- **Text-led** — typography is primary; imagery supports it.
- **Image-led** — imagery is primary; text explains or anchors it.
- **Balanced** — text and image share comparable visual weight.
- **Integrated** — text and imagery overlap or operate as one composition.

Do not default every section to a generic 50/50 text-image split.

Preserve the chosen relationship during responsive translation even when exact geometry changes.

## 8.9 Motion and Interaction Language

Define one interaction personality for the product rather than inventing motion component by component.

When relevant define:

- Hover response.
- Press / active feedback.
- Focus behavior.
- Scroll reveal.
- Parallax or depth response.
- Floating / ambient motion.
- Counter / metric animation.
- Marquee behavior.
- Pointer response.
- Transition duration and easing.

Maintain a **motion budget**. Not every element should animate. Motion must reinforce hierarchy, state, or product character rather than compensate for weak static composition.

## 8.10 Responsive Design Continuity

Responsive design may change geometry aggressively, but preserve the relationships that define the brand and composition.

Identify which relationships must survive across viewports, such as:

- Primary focal point remains primary.
- Supporting image remains supporting rather than becoming dominant.
- Accent logic remains recognizable.
- Typography personality remains consistent.
- Card / surface grammar remains consistent.
- Interaction character remains consistent.
- Narrative order remains coherent.

Responsive fidelity is **continuity**, not literal shrinking.

## 8.11 Brand Drift Detection

Every newly generated section, component, or asset should be checked against the established visual system.

Look for drift in:

- Font family or typography personality.
- Type scale and weight usage.
- Icon style.
- Photography / illustration mood.
- Color temperature and saturation.
- Radius and border language.
- Shadow / depth language.
- Spacing rhythm.
- Motion personality.
- Asset rendering style.

If a new element is individually attractive but does not look like it belongs to the same product, treat that as a defect.

## 8.12 Visual Coherence Review

During final visual QA, assess coherence independently from reference fidelity.

Evaluate:

- Typography coherence.
- Asset coherence.
- Composition coherence.
- Color coherence.
- Surface / shape coherence.
- Interaction / motion coherence.
- Responsive coherence.

An internal qualitative score such as `strong / acceptable / weak` is sufficient; numeric scoring is optional.

A page can match a screenshot locally yet still fail globally if its independently implemented pieces no longer feel like one visual system.

---

# 9. Compose the Page Before Decorating It

Solve macro composition first:

- What dominates the first viewport?
- Where does the eye land next?
- How does the page alternate density and breathing room?
- Which sections intentionally break the grid?
- Which elements share alignment anchors?
- Where should imagery, typography, negative space, or interaction carry hierarchy instead of boxes?
- Which areas require overlap or cross-section visual continuity?

A good composition must remain legible before decorative polish.

Do not use equal-width grids merely because they are easy to code.

---

# 10. Approved Visual Target

Once the user approves a visual concept:

- Lock its global art direction.
- Lock its major composition.
- Lock its visual hierarchy.
- Lock its primary image-to-text balance.
- Do not casually regenerate the whole page.

The approved image becomes a stable visual target, not a disposable draft.

If implementation later reveals an asset problem, solve the asset problem without redefining the whole page.

---

# 11. Reference Decomposition Mode

When the user has approved a visual concept or supplied a target design, do not move directly from "look at the image" to "write HTML".

First convert the approved reference into four implementation artifacts:

1. **Block Map**
2. **Layer Map**
3. **Text Map**
4. **Geometry Map**

These become the structured design specification for implementation.

The goal is to reduce ambiguity, prevent visual drift, and avoid reconstructing a rich composition from memory alone.

---

## 11.1 Block Map

The Block Map defines macro page structure.

For each major section identify:

- Section name.
- Visual purpose.
- Business purpose.
- Approximate vertical span.
- Internal layout model.
- Dominant alignment anchors.
- Relationship to adjacent sections.
- Density level.
- Mobile adaptation strategy.

Typical blocks:

- Header.
- Hero.
- Trust row.
- Services.
- Proof / stats.
- Process.
- FAQ.
- CTA.
- Footer.

The Block Map should answer:

- What the page is made of.
- Where sections begin and end.
- How the eye flows vertically.
- Which sections are dense versus spacious.
- Which sections intentionally overlap or bleed into each other.

Do not implement before macro section structure is clear.

---

## 11.2 Layer Map

The Layer Map defines the visual composition stack.

For each important visual element identify:

- Layer id.
- Type: background / surface / image / UI overlay / decoration / card / accent.
- Parent block.
- Position.
- Size.
- Z-order.
- Opacity / prominence.
- Whether it is structural or decorative.
- Whether it should be implemented as HTML, CSS, SVG, raster image, or generated asset.

Typical layers:

- Base background.
- Ambient shapes.
- Gradient / glow / surface blobs.
- Hero figure.
- Floating metrics.
- Social / comment chips.
- Arrows.
- Decorative dots / icons.
- Cards.
- CTA surfaces.

The Layer Map should answer:

- What sits behind what.
- Which elements carry visual weight.
- Which elements cross section boundaries.
- Which elements must remain flexible.
- Which pieces require isolated assets.

Do not flatten all visual information into one background image unless unavoidable.

---

## 11.3 Text Map

The Text Map defines content hierarchy and live text structure.

For each text element identify:

- Actual content.
- Role: eyebrow / h1 / emphasized span / body / CTA / label / caption / stat / card title / card description.
- Parent block.
- Intended line breaks.
- Emphasis rules.
- Semantic tag target.
- Whether it must remain editable live text.

Critical rule:

`Design Reference = visual truth`

`Original Copy / User Copy / Live Site = semantic truth`

Use the reference image to decide how text looks, wraps, aligns, and emphasizes.

Do not rely on generated-image text as the semantic source of truth. Image models may alter copy, prices, punctuation, names, or numbers.

Important copy should remain live HTML text whenever possible.

Do not bake critical copy into generated imagery except for clearly decorative, non-essential fragments.

---

## 11.4 Geometry Map

The Geometry Map defines approximate spatial measurements.

For each major element or cluster identify relative geometry such as:

- Reference canvas size.
- X / Y position.
- Width / height.
- Section top / bottom.
- Container inset.
- Column ratios.
- Dominant alignment lines.
- Overlap amount.
- Image crop region.
- Negative-space regions.

Geometry may be stored as pixels, percentages, normalized coordinates, or approximate ratios.

Example:

```text
Reference: 1400 × 1100
Content left: 6.5%
Hero text: x 6.5%, y 18%, w 36%
Hero image: x 60%, y 12%, w 31%, h 43%
Stats overlay: x 47%, y 18%
Services start: y 58%
```

The goal is not blind pixel copying. The goal is preserving proportion, anchors, and visual weight.

Do not compensate for one wrong dimension by adding unrelated offsets elsewhere.

---

# 12. Asset Resolution Plan

After decomposition, classify every significant visual layer into one of these implementation modes. Apply the Token Map and Asset Style Contract during this decision so implementation method does not break visual coherence:

- **A. Live HTML** — semantic UI, cards, metrics, labels, buttons, chips, comments.
- **B. CSS / SVG** — gradients, surfaces, arrows, dots, borders, simple icons, geometric backgrounds.
- **C. Direct Crop / Existing Asset** — clean source asset already exists and can be reused safely.
- **D. Regenerate Clean Asset** — the approved visual contains a mixed or contaminated asset that must be recreated independently.
- **E. Omit / Simplify** — low-value decoration not needed for fidelity or business purpose.

This classification is mandatory for complex image-first implementation.

A visual reference is not automatically a usable asset library.

For example:

```text
Hero streamer        → D. Regenerate clean asset
Pink background blob → B. CSS/SVG
Stats panel          → A. Live HTML
Comment chips        → A. Live HTML
Reaction icons       → A/B
Headline             → A. Live HTML
```

---

# 13. Local Regeneration Policy

After a concept is approved, additional image generation must be local and purposeful.

Acceptable reasons:

1. Isolate or improve one visual asset.
2. Create a missing background element.
3. Replace a contaminated crop containing baked-in UI or text.
4. Generate a mobile-specific crop or visual asset.
5. Create an illustration/photo/3D element that cannot be reconstructed faithfully in CSS or SVG.

Rules:

- Regenerate the smallest useful target.
- Preserve the approved page-level composition.
- Do not replace unrelated areas.
- Do not allow local asset generation to redefine the global art direction.
- Prefer asset-specific prompts that explicitly exclude text, UI overlays, badges, or unrelated decoration when clean assets are needed.

Bad behavior:

- Re-roll the whole homepage because one local asset is inconvenient.
- Redesign the hero during implementation without user approval.
- Replace difficult asymmetry with a generic grid because it is easier to code.

---

# 14. Asset Locking

Treat approved generated assets as versioned design inputs.

Recommended state model:

```text
hero-streamer
v1 generated
v2 approved
LOCKED

bg-surface
CSS
LOCKED

stats-panel
HTML
LOCKED
```

Once an asset is approved or intentionally reconstructed, do not regenerate it casually.

This prevents target drift caused by probabilistic image generation.

---

# 15. Implementation Order

After decomposition and asset planning, implement in this order:

1. Page canvas and section proportions.
2. Primary alignment system.
3. Live typography structure.
4. Large background and surface layers.
5. Hero image / major visual.
6. Floating overlays and secondary composition details.
7. Service / content sections.
8. CTA / trust / support details.
9. Responsive adaptation.
10. Screenshot comparison and iterative fixes.

Do not begin with decorative micro-details.

Do not switch the user's requested implementation technology merely to simplify the design task.

If working inside an existing project, preserve its stack, conventions, component architecture, and routing unless a change is necessary and justified.

---

# 16. HTML Fidelity Rules

When implementing from an approved visual concept:

- Do not "rationalize" the design into a generic template.
- Do not normalize asymmetry merely because code is easier.
- Do not turn custom compositions into equal-width card grids.
- Do not replace intentional overlap with safe vertical stacking unless a responsive composition requires it.
- Do not remove tension and rhythm through excessive uniform spacing.
- Do not simplify a strong image-to-type relationship into independent left/right columns if the reference relies on overlap or shared composition.
- Do not use placeholder imagery when a specific approved visual asset is required.

The goal is not "a reasonable approximation".

The goal is the closest faithful reconstruction that still respects implementation integrity.

---

# 17. Render the Real Result

Visual review must evaluate rendered output, not source code alone.

When rendering or screenshot capability exists:

- Render the actual implementation.
- Use the target viewport.
- Compare directly with the approved reference.
- Check desktop and mobile when responsiveness matters.
- Re-render after meaningful fixes.

If rendering tools are unavailable, perform a structural visual review and state the limitation only when it materially affects confidence.

---

# 18. Screenshot-Based Reconstruction Review

Compare the render against the approved target in this order:

1. Canvas and major section proportions.
2. Focal point and hierarchy.
3. Text-to-image balance.
4. Main alignment anchors.
5. Typography scale, weight, wrapping, and line-height.
6. Negative space and spacing rhythm.
7. Large background masses and surfaces.
8. Imagery scale, crop, and visual weight.
9. Floating overlays and secondary clusters.
10. Component rhythm.
11. Typography / asset / surface coherence across sections.
12. Brand drift introduced by regenerated assets or newly implemented components.
13. Borders, radius, shadows, icons, and micro details.

Do not start with tiny CSS details when macro composition is still wrong.

---

# 19. Critique Mismatch Classes

Evaluate rendered output across these mismatch classes:

- Art-direction mismatch.
- Composition mismatch.
- Geometry mismatch.
- Typography mismatch.
- Hierarchy mismatch.
- Visual-weight mismatch.
- Spacing/rhythm mismatch.
- Color/contrast mismatch.
- Shape/surface mismatch.
- Asset/imagery mismatch.
- Brand mismatch.
- Responsive mismatch.
- Interaction/state mismatch.
- Reference-fidelity mismatch.
- Token / visual-grammar drift.
- Asset-style drift.
- Cross-section coherence mismatch.
- Generic-AI-pattern contamination.

---

# 20. Fix Only Dominant Mismatches

On each refinement iteration, identify and fix **1 to 3 major mismatches maximum**.

Choose the mismatches with the largest perceptual impact, not the easiest CSS edits.

Preferred order:

1. Wrong art direction or global concept.
2. Macro composition / geometry / proportions.
3. Focal point / visual weight.
4. Typography / hierarchy.
5. Spacing / alignment.
6. Color / surfaces / imagery.
7. Component details / micro-interaction.

Do not scatter one revision across many unrelated details.

Re-render after each meaningful iteration when possible.

---

# 21. Responsive Design and Mobile Translation

Treat mobile as a separate composition state sharing the same design system and Token Map. Preserve design continuity even when geometry changes substantially.

Desktop concept approval does **not** automatically mean the mobile composition is solved.

Before adapting a complex desktop design, choose a mobile translation strategy:

- **A. Preserve Composition** — keep the core spatial relationship with scaled adjustments.
- **B. Simplify Composition** — preserve hierarchy and art direction while removing or relocating secondary layers.
- **C. Create Separate Mobile Concept** — redesign the composition for mobile while keeping the same visual system.

For important mobile viewports reconsider:

- Focal point.
- Reading order.
- Navigation behavior.
- Hero proportion.
- Typography scale.
- Image crop.
- Density.
- Touch targets.
- Which floating layers disappear, merge, or relocate.
- Whether CTA moves earlier in the reading sequence.

Do not assume `desktop grid → single column` is sufficient.

A mobile page that merely stacks desktop cards is unfinished when the desktop relies on strong composition.

---

# 22. Interaction Design

Interaction should reinforce the visual concept and information architecture and follow the established motion / interaction language.

- Give visible states to controls that matter.
- Use motion purposefully.
- Use hover as enhancement, never as the only path to essential content.
- Keep interaction affordances consistent.
- Prefer native semantics and accessibility over decorative imitation.
- Avoid motion whose only purpose is to make a static composition look impressive.
- When a static visual concept implies interaction, reconstruct the interaction as behavior rather than baking it into a screenshot.

---

# 23. Generic AI UI Detection

Treat these as warning signals, not absolute bans:

- Repeated rounded cards used as the default container for everything.
- Uniform 2/3/4-column card grids with equal visual weight.
- Purple/blue gradients chosen without brand rationale.
- Excessive pills, badges, soft shadows, glass panels, or glowing borders.
- Centered hero + eyebrow + gradient headline + two buttons as an automatic homepage formula.
- Icon + heading + paragraph repeated mechanically across all features.
- Every section wrapped in an identical box.
- Overly uniform spacing that removes rhythm and tension.
- Weak typographic contrast compensated for by more containers.
- Decorative blobs, meshes, stars, or shapes with no conceptual role.
- Dashboard aesthetics applied to products that are not dashboards.
- Mobile layouts produced only by vertically stacking desktop cards.
- Generic stock-photo placement that does not participate in the composition.
- Visual effects added because they look "modern" rather than because they support the product or narrative.

When several appear without product-specific justification, stop polishing and reconsider the art direction or composition.

---

# 24. Redesign Mode

When redesigning an existing site, first decide what must be preserved:

- Brand recognition.
- Existing information architecture.
- SEO-critical content.
- Conversion path.
- Existing component/frontend architecture.
- Assets with established recognition.
- Required functionality and login flows.

A redesign may change visual grammar, hierarchy, and composition aggressively when those changes serve the user's goal, but it must not silently delete business-critical structure.

When the existing page is visually weak, do not let its weak composition become the default reference. Preserve content and business logic, then establish a stronger art direction.

---

# 25. Output Behavior

Match the user's requested deliverable.

- If they ask for visual exploration, produce concept images first.
- If they ask for an image, produce the visual concept/image.
- If they ask for HTML/code from an approved visual, decompose first, then implement.
- If they ask for an interactive prototype, render an interactive prototype when the environment supports it.
- If they ask for critique, provide prioritized findings rather than redesigning without permission.
- If they provide an existing project, preserve its stack, conventions, and architecture unless a change is necessary and justified.

Do not dump the internal brief, maps, or QA checklist into every response. Use them internally unless exposing them helps the user evaluate a decision or continue implementation.

---

# 26. Completion Gate

Do not call the design finished until all materially relevant conditions pass:

- The page has a recognizable design intent.
- Visual hierarchy works without explanation.
- Typography follows a coherent system rather than section-by-section improvisation.
- Layout rhythm is intentional rather than uniformly spaced.
- Components share a coherent visual grammar.
- Token usage is stable enough that the implementation can evolve without style drift.
- Independently generated assets still satisfy the Asset Style Contract.
- No material brand drift is visible across sections.
- The approved visual target has been decomposed sufficiently for faithful implementation.
- Important copy remains semantically correct and live when appropriate.
- Generated assets are clean, purposeful, and stable.
- No dominant reference mismatch remains.
- Mobile is composed, not merely stacked.
- The primary action and business purpose remain clear.
- Generic AI UI patterns are absent unless genuinely appropriate.
- The implementation still fits the user's technical constraints.
- The page has been judged from rendered output when rendering tools are available.

---

# 27. Internal Working Model

For complex image-first implementation, maintain this internal state:

```text
Approved Visual Target
        ↓
Block Map
Layer Map
Text Map
Geometry Map
        ↓
Token Map / Visual Grammar / Asset Style Contract
        ↓
Asset Resolution Plan
        ↓
Generate / Extract Missing Assets
        ↓
Asset Approval / Lock
        ↓
HTML / App Implementation
        ↓
Render
        ↓
Reference Comparison
        ↓
Fix 1–3 Dominant Mismatches
        ↓
Render Again
        ↓
Mobile Translation / Mobile QA
        ↓
Completion Gate
```

This decomposition stage is the bridge between image-based design and reliable frontend implementation.

---

# Final Rule

A technically valid page that looks generic is unfinished.

A visually attractive page that ignores the user's business purpose is unfinished.

A beautiful concept image that cannot be decomposed into stable implementation inputs is unfinished.

A faithful screenshot match with brittle or architecture-breaking implementation is unfinished.

A responsive page that merely stacks desktop elements is unfinished when the reference requires composition.

The target is all of these at once:

**design intent + visual hierarchy + visual coherence + stable visual specification + asset discipline + implementation fidelity + responsive continuity + implementation integrity**.
