# OpenAI Plugin Directory Submission Pack — web-design v1.3.0

**Status:** prepared; not yet submitted.  
**Type:** skill-only plugin / Agent Skill  
**Publisher:** max0821  
**Official source:** https://github.com/max0821/web-design-skill  
**License:** MIT

## Submission note

OpenAI currently documents that plugins may contain only Skills and that the Plugin Directory is the primary discovery surface across ChatGPT and Codex. Public documentation does not currently publish a separate stable manifest schema or public submission API specifically for third-party skill-only plugins. This repository therefore does not invent a proprietary manifest; use the current Plugin/Skills submission or import UI and copy the listing material below into the fields actually presented.

## Copy-ready listing

- **Name:** Web Design
- **Skill:** `web-design`
- **Version:** `1.3.0`
- **Publisher:** `max0821`
- **Category:** Design / Front-end / Developer workflow
- **Short description:** Visual-first web design with approved targets, design-to-code fidelity, asset locking, and render-based QA.
- **Official source:** https://github.com/max0821/web-design-skill
- **License:** MIT

### Long description

Web Design is a visual-first Agent Skill for designing, redesigning, and reconstructing polished websites without generic AI UI. It establishes art direction and a user-approved visual target, decomposes the target into Block, Layer, Text, and Geometry maps, resolves exact UI versus generated assets, locks accepted assets to prevent target drift, implements semantic frontend code, and iterates against the rendered result by fixing only the 1–3 highest-impact mismatches per pass.

### Discovery terms

`website redesign`, `landing page`, `homepage`, `marketing site`, `product site`, `dashboard UI`, `screenshot-to-code`, `image-to-HTML`, `mockup-to-code`, `pixel-accurate frontend`, `responsive web design`, `design system`, `visual prototype`, `visual fidelity`, `render-based QA`, `avoid generic AI UI`

### Starter prompts

- Redesign this homepage, but establish the visual direction before writing final HTML.
- Reconstruct this screenshot into responsive HTML/CSS and keep the rendered result visually faithful.
- Turn this approved visual mockup into production frontend without letting generated assets drift.
- Review this rendered page against the reference and fix only the three largest visual mismatches.

## Review / privacy notes

- No OAuth, MCP server, external account dependency, custom backend, or executable scripts.
- No custom telemetry or data collection.
- May use host-provided browser, screenshot/rendering, image-generation/editing, or interactive HTML capabilities when available and relevant.
- Does not grant access to data the user or host cannot already access.
- Canonical source, history, author, and MIT license are visible in the repository and package.

## Verification prompt

```text
Do not perform design work.
Based only on the loaded web-design Skill, answer:
1. metadata.version?
2. Four Maps after Approved Visual Target?
3. Asset Resolution Plan types?
4. Whole-page or local regeneration for one dirty asset?
5. How is target drift prevented?
6. Long questionnaire or progressive options?
7. Official source URL?
```

Expected fingerprints: `1.3.0`, Block/Layer/Text/Geometry, five Asset Resolution types, local regeneration, asset locking, progressive clarification, canonical GitHub source, and 1–3 dominant mismatch render QA.

## Checklist

- [x] Required Agent Skills `name` and `description`.
- [x] Folder name matches `name: web-design`.
- [x] Description under 1024 characters with concrete routing terms.
- [x] Standard top-level `license: MIT`.
- [x] Version, author, source in metadata.
- [x] Main `SKILL.md` under 500 lines.
- [x] Progressive-disclosure references.
- [x] No OAuth/MCP/custom backend/scripts.
- [x] English and Traditional Chinese docs.
- [x] Installable ZIP prepared.
- [ ] Open the current Plugin Directory / Skills submission UI and paste the listing fields.
- [ ] Review live terms/fields and press Submit.
