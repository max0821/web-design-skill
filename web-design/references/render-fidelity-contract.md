# Implementation Fidelity and Render QA

Detailed rules for HTML fidelity, rendering, screenshot reconstruction, mismatch classes, dominant-mismatch repair, generic-AI detection, and completion gates.

## 16. HTML Fidelity Rules

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

## 17. Render the Real Result

Visual review must evaluate rendered output, not source code alone.

When rendering or screenshot capability exists:

- Render the actual implementation.
- Use the target viewport.
- Compare directly with the approved reference.
- Check desktop and mobile when responsiveness matters.
- Re-render after meaningful fixes.

If rendering tools are unavailable, perform a structural visual review and state the limitation only when it materially affects confidence.

---

## 18. Screenshot-Based Reconstruction Review

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

## 19. Critique Mismatch Classes

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

## 20. Fix Only Dominant Mismatches

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

## 23. Generic AI UI Detection

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

## 26. Completion Gate

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
