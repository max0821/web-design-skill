# Changelog

## 1.3.0 — 2026-08-22

### Added
- Canonical source metadata and standards-aligned top-level MIT license field.
- Discovery-oriented routing terms for redesign, screenshot-to-code, image-to-HTML, mockup-to-code, pixel-accurate frontend, responsive design, and visual QA.
- Conversation-language rule.
- Progressive-disclosure references for detailed design, decomposition, responsive, and render-fidelity contracts.
- Plugin Directory submission pack and reviewer notes.

### Changed
- Main `SKILL.md` reduced below the recommended 500-line target while preserving detailed v1.2.1 rules in references.
- Visible version and OpenAI interface description updated to `v1.3.0`.
- MIT wording clarified to require retention of copyright and license notice.


All notable changes to `web-design` are documented here.

## [1.2.1] - 2026-08-22

### Added

- Author and license metadata in `SKILL.md`.
- MIT License inside the Skill package.
- English `web-design/README.md`.
- Traditional Chinese `web-design/README.zh-TW.md`.
- Explicit commercial-use permission and copyright notice.

### Changed

- UI short description now shows `v1.2.1`.
- Skill package now carries its own documentation and license so attribution survives when the Skill folder is redistributed independently of the GitHub repository.

## [1.2.0] - 2026-08-22

### Added

- Visible version marker near the top of `SKILL.md`.
- Typography System.
- Visual Grammar / Style Consistency.
- Cross-cutting Token Map.
- Asset Style Contract for multi-pass image generation.
- Composition consistency rules.
- Focal Hierarchy Contract and attention budget.
- Section Role Model.
- Explicit Image / Text Relationship modes.
- Motion and Interaction Language with motion budget.
- Responsive Design Continuity.
- Brand Drift Detection.
- Visual Coherence Review.
- `agents/openai.yaml` UI metadata with version in `short_description`.

### Changed

- Core workflow now includes a `Coherence Contract` between decomposition and asset resolution.
- Quality target now treats Design Intent, Visual Fidelity, Visual Coherence, and Implementation Integrity as connected concerns.

## [1.1.0] - 2026-08-22

### Added

- Progressive, option-based design clarification.
- Visual exploration before implementation for high-visual pages.
- User reaction and explicit Approved Visual Target.
- Four decomposition artifacts: Block Map, Layer Map, Text Map, Geometry Map.
- Asset Resolution Plan.
- Local regeneration policy.
- Asset approval / lock to prevent target drift.
- Visual-weight control and focal hierarchy.
- Separate mobile translation strategies: preserve, simplify, or create a separate mobile concept.
- Screenshot-based reconstruction review.

### Changed

- Workflow shifted from direct `Art Direction → HTML` toward a visual-design-to-code decomposition pipeline.
- Generated-image text is not semantic truth; original/user copy remains the semantic source of truth.

## [1.0.0] - 2026-08-22

### Added

- Initial `web-design` Skill.
- Art direction and visual system workflow.
- Composition-first implementation.
- Render-based visual QA.
- 1–3 dominant mismatch refinement rule.
- Generic AI UI detection.
- Reference matching mode.
- Responsive composition guidance.
