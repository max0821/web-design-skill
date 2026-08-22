# Decomposition and Asset Resolution

Detailed rules for the four maps, Asset Resolution Plan, local regeneration, and asset locking.

## 11. Reference Decomposition Mode

When the user has approved a visual concept or supplied a target design, do not move directly from "look at the image" to "write HTML".

First convert the approved reference into four implementation artifacts:

1. **Block Map**
2. **Layer Map**
3. **Text Map**
4. **Geometry Map**

These become the structured design specification for implementation.

The goal is to reduce ambiguity, prevent visual drift, and avoid reconstructing a rich composition from memory alone.

---

### 11.1 Block Map

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

### 11.2 Layer Map

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

### 11.3 Text Map

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

### 11.4 Geometry Map

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

## 12. Asset Resolution Plan

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

## 13. Local Regeneration Policy

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

## 14. Asset Locking

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
