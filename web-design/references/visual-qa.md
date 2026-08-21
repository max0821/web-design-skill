# Visual QA Rubric

Use this reference after rendering a design or when comparing implementation to a supplied target.

## Core principle

Review perceptually, from largest impact to smallest. Do not spend an iteration correcting icon offsets while the hero proportions, typography, or page rhythm are wrong.

Each iteration should fix at most **1–3 dominant mismatches**.

## Mismatch taxonomy

### Art-direction mismatch

Symptoms:
- The interface is competent but belongs to the wrong visual world.
- Brand personality is missing.
- The design relies on generic SaaS/UI conventions instead of a product-specific thesis.

Typical action:
- Revisit the art direction, not local CSS.

### Composition mismatch

Check:
- First-viewport balance.
- Section heights.
- Column proportions.
- Alignment anchors.
- Focal points.
- Negative-space distribution.
- Image/text relationship.

Composition errors usually outrank all decorative errors.

### Typography mismatch

Check:
- Font category/personality.
- Display/body relationship.
- Size ratios.
- Weight.
- Width.
- Tracking.
- Line-height.
- Line wrapping.
- Measure.
- Optical alignment.

A different line break in the hero can shift the entire composition.

### Hierarchy mismatch

Ask:
- Can the intended reading order be understood in 2–3 seconds?
- Are secondary elements visually quieter?
- Is the primary CTA actually dominant where it should be?
- Are boxes compensating for weak hierarchy?

### Spacing/rhythm mismatch

Check:
- Local grouping.
- Section separation.
- Alignment consistency.
- Uneven accidental gaps.
- Excessively uniform spacing.
- Optical spacing around large type and images.

### Color/contrast mismatch

Check:
- Canvas and surface relationships.
- Text contrast.
- Accent saturation and usage frequency.
- Dark/light balance.
- Semantic state consistency.

### Surface/shape mismatch

Check:
- Radius consistency by semantic role.
- Border weight.
- Shadow logic.
- Panel treatment.
- Divider style.

### Asset/imagery mismatch

Check:
- Crop.
- Scale.
- Subject placement.
- Image tone.
- Illustration style.
- Icon family.
- Whether assets actually reinforce the art direction.

### Brand mismatch

Check:
- Recognizable brand cues.
- Existing identity elements.
- Tone of typography and imagery.
- Color usage.
- Product-specific conventions.

### Responsive mismatch

Check each target viewport independently:
- Reading order.
- Hero height.
- Navigation.
- Type scale.
- Overflow.
- Tap targets.
- Image crop.
- Density.
- Content that becomes too long when stacked.

### Interaction/state mismatch

Check:
- Hover/focus/active/selected/disabled states.
- Motion behavior.
- Expansion/collapse.
- Loading/empty/error states when relevant.
- Whether interaction matches the visual grammar.

### Reference fidelity mismatch

When a target exists, compare:
- Large geometry first.
- Typography second.
- Spacing third.
- Surface/color fourth.
- Detail last.

Do not chase pixel-level detail while macro ratios remain incorrect.

### Generic-AI-pattern contamination

Look for clusters of these signals:
- Cardification.
- Excessive rounded corners.
- Purple/blue gradients without rationale.
- Uniform feature grids.
- Generic icon-heading-copy modules.
- Decorative glow/mesh/blob effects.
- Identical section rhythm.
- Centered-everything marketing layout.
- Weak typography.
- Mobile = stacked desktop cards.

One pattern may be correct. Several together without a strong product reason indicate design drift.

## Iteration protocol

1. View the whole page before zooming into details.
2. Name the single biggest perceptual problem.
3. Name at most two additional high-impact problems.
4. Change only what is necessary to address those problems.
5. Re-render.
6. Re-rank from scratch rather than blindly continuing the old checklist.

Do not maintain a long accumulating list of micro-fixes across iterations; priorities change after major corrections.

## Completion questions

- Does the page have a specific visual point of view?
- Does the page composition serve the content rather than merely contain it?
- Does typography carry hierarchy before cards, borders, or color are added?
- Does mobile preserve the design idea?
- If a reference exists, are the remaining differences minor rather than structural?
- Is the implementation maintainable enough that fidelity will survive future changes?
