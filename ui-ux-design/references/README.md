
# References catalog

Curated links, markdown digests, and tagged media URL refs for design and build work. Not executable recipes—for those, see [`../README.md`](../README.md#skills).

## How to add an entry

1. Copy [`_template/`](_template/) to a new kebab-case folder (e.g. `references/footer-pattern-notes/`).
2. Fill frontmatter and body in `README.md`.
3. For `kind: media-set`, add or update sibling `media.md` (URLs only—no image or video binaries in git).
4. Set `status: inbox` until reviewed; move to `curated` when ready for agent use.
5. Add a row to the catalog table below.

## Frontmatter contract

```yaml
---
title: ...
kind: reference | media-set | link-digest
status: inbox | curated | deprecated
tags: [seo, aeo, ui, ...]
sources:
  - url: https://...
    label: ...
---
```

| Field | Values | Notes |
| --- | --- | --- |
| `title` | string | Human-readable entry name |
| `kind` | `reference`, `media-set`, `link-digest` | `media-set` requires sibling `media.md` |
| `status` | `inbox`, `curated`, `deprecated` | Only `curated` entries belong in agent context by default |
| `tags` | string array | Discovery filters (e.g. `seo`, `aeo`, `ui`, `footer`, `intake`) |
| `sources` | url + label pairs | Canonical links this entry summarizes or cites |

## Media-set pattern

For `kind: media-set`, keep `README.md` as the index and put URL rows in `media.md`:

```markdown
| url | type | alt | when-to-use |
| --- | --- | --- | --- |
| https://example.com/photo.jpg | image | ... | ... |
| https://example.com/demo.mp4 | video | ... | ... |
```

Each row: `url`, `type` (`image` | `video`), `alt`, `when-to-use`. URLs only—no binaries in git.

## Catalog

| Folder | Title | Kind | Status | Tags |
| --- | --- | --- | --- | --- |
| [`astra-skills-standard/`](astra-skills-standard/README.md) | Astra skills audit standard | reference | curated | skills, astra, standards |
| [`design-book-of-shapes/`](design-book-of-shapes/README.md) | Book of Shapes — generative SVG patterns | reference | curated | design, shapes, svg, patterns, generative, backgrounds, free, commercial |
| [`design-playgrnd/`](design-playgrnd/README.md) | Playgrnd — browser-based generative design tools | reference | curated | design, generative, patterns, posters, backgrounds, textures, browser, privacy, free |
| [`design-specialized-galleries/`](design-specialized-galleries/README.md) | Specialized web and brand design inspiration galleries | link-digest | curated | ui, design, inspiration, gallery, sections, bento, hero, navigation, footer, 404, saas, social |
| [`design-kage/`](design-kage/README.md) | Kage — real-product interface inspiration and agent prompts | reference | curated | ui, design, inspiration, components, prompts, agents, gallery, free |
| [`design-quiver-ai/`](design-quiver-ai/README.md) | QuiverAI — structured AI-generated SVGs | reference | curated | design, ai, svg, vector, logos, icons, illustrations, animation, mcp, api, paid |
| [`design-typeface-fyi/`](design-typeface-fyi/README.md) | Typeface.fyi — visual typeface discovery | reference | curated | design, typography, fonts, inspiration, discovery, licensing |
| [`design-uisfx/`](design-uisfx/README.md) | UI SFX — semantic interface sound library | reference | curated | design, audio, sound, ui, accessibility, typescript, mit, cc0, free |
| [`tools-screenshot-to-code/`](tools-screenshot-to-code/README.md) | Screenshot to Code — visual frontend reconstruction | reference | curated | tools, ai, code, screenshots, figma, frontend, react, vue, tailwind, mit, free, paid |
| [`ui-dialkit/`](ui-dialkit/README.md) | DialKit — live interface tuning controls | reference | curated | ui, development, controls, animation, tuning, react, solid, svelte, vue, javascript, mit, free |
| [`ui-liquid-glass/`](ui-liquid-glass/README.md) | Liquid Glass — refractive glass for the web | reference | curated | ui, effects, glass, react, refraction, accessibility, mit, free |
| [`design-md-resources/`](design-md-resources/README.md) | DESIGN.md generators, catalogs, and UI references | link-digest | curated | design, design-md, design-systems, agents, inspiration, mcp, ui-reference |
| [`tools-voicestudio/`](tools-voicestudio/README.md) | VoiceStudio — local AI voice production workspace | reference | curated | tools, audio, voice, ai, local-first, dubbing, transcription, audiobook, api, mcp, agpl |
| [`tools-shotbase/`](tools-shotbase/README.md) | Shotbase — screen capture and recording workspace | reference | curated | tools, macos, screenshots, screen-recording, video, documentation, sharing, paid |
| [`ui-aicss/`](ui-aicss/README.md) | AICSS — UI components for AI agents | reference | curated | ui, components, ai, agents, chat, react, vue, svelte, shadcn |
| [`ui-annnimate/`](ui-annnimate/README.md) | Annnimate — GSAP motion components | reference | curated | ui, animation, motion, gsap, react, vue |
| [`ui-astryx/`](ui-astryx/README.md) | Astryx — Meta-grown agent-ready design system | reference | curated | ui, components, design-system, react, stylex, themes, templates, cli, mcp, mit, free |
| [`ui-beautiful-ui/`](ui-beautiful-ui/README.md) | Beautiful UI — AI-native interface primitives | reference | curated | ui, components, ai, agents, react, mit, free |
| [`ui-bencho/`](ui-bencho/README.md) | Bencho — interactive UI blocks | reference | curated | ui, components, interactions, react, mit, free |
| [`ui-bestdesignsonx/`](ui-bestdesignsonx/README.md) | Best Designs On X | reference | curated | ui, design, inspiration, gallery, x, instagram, dribbble, behance, fonts, app-icons |
| [`ui-beui-pro/`](ui-beui-pro/README.md) | beUI Pro — premium motion components | reference | curated | ui, components, motion, react, nextjs, tailwind, paid |
| [`ui-reverseui/`](ui-reverseui/README.md) | ReverseUI - premium animated UI components; animated site reference | reference | curated | ui, components, react, motion, animation, paid |
| [`ui-components/`](ui-components/README.md) | UI Components — catalog | reference | curated | ui, components, catalog |
| [`ui-cue/`](ui-cue/README.md) | Cue — curated component references and AI prompts | reference | curated | ui, components, inspiration, prompts, react, motion, free, paid |
| [`ui-evil-buttons/`](ui-evil-buttons/README.md) | Evil Buttons — animated shadcn button components | reference | curated | ui, components, buttons, react, shadcn, motion, apache, free |
| [`ui-feralui/`](ui-feralui/README.md) | FeralUI — playful physics-driven React experiments | reference | curated | ui, components, react, typescript, physics, animation, interaction, free, mit |
| [`ui-halaska/`](ui-halaska/README.md) | UI by Halaska — AI product UI kit | reference | curated | ui, components, ai, agents, react, shadcn, mit, free |
| [`ui-keyline-icons/`](ui-keyline-icons/README.md) | Keyline Icons | reference | curated | ui, icons, shadcn, svg, react, mit |
| [`ui-kobra/`](ui-kobra/README.md) | Kobra — React component system | reference | curated | ui, components, react, shadcn, figma, mcp, free, paid |
| [`ui-libraries-dev/`](ui-libraries-dev/README.md) | Libraries.dev — UI effects for AI agents | reference | curated | ui, components, effects, react, agents, mit, free, paid |
| [`ui-patterns/design-inspiration-screenshots/`](ui-patterns/design-inspiration-screenshots/README.md) | Design inspiration screenshots — September 2026 | reference | curated | ui, design, inspiration, screenshots, bento, iridescent, data-flow |
| [`ui-patterns/features-blueprint-cards/`](ui-patterns/features-blueprint-cards/README.md) | Features blueprint cards — three-up pattern | media-set | curated | ui, patterns, cards, features, blueprint |
| [`ui-openui/`](ui-openui/README.md) | OpenUI — open standard for generative interfaces | reference | curated | ui, generative-ui, agents, streaming, react, vue, svelte, react-native, mcp, mit, free |
| [`ui-page-mascot/`](ui-page-mascot/README.md) | Page Mascot — cursor-aware interactive character | reference | curated | ui, mascot, character, animation, sprite-sheet, react, interaction, mit, free |
| [`ui-patterns/pricing-tier-cards/`](ui-patterns/pricing-tier-cards/README.md) | Pricing tier cards — three-plan pattern | media-set | curated | ui, patterns, pricing, cards, saas |
| [`ui-xiod/`](ui-xiod/README.md) | XiodUI — versioned React component library | reference | curated | ui, components, react, tailwind, base-ui, accessibility, theming, animation, source-available, free |
| [`ui-vibeprompts/`](ui-vibeprompts/README.md) | VibePrompt — UI prompt and Tailwind snippet library | reference | curated | ui, prompts, tailwind, layouts, ai, vibe-coding, free |
| [`ui-shadcncraft/`](ui-shadcncraft/README.md) | ShadcnCraft — production-ready shadcn blocks and Figma kit | reference | curated | ui, components, blocks, shadcn, react, figma, mcp, agents, free, paid |
| [`ui-shadcn/`](ui-shadcn/README.md) | shadcn/ui — primary component foundation | reference | curated | ui, components, shadcn, react, tailwind, primary |
| [`ui-spectrum/`](ui-spectrum/README.md) | Spectrum UI — components and MCP registry | reference | curated | ui, components, react, tailwind, shadcn, mcp, agents |

**UI and design detail folders:** [`ui-shadcn/`](ui-shadcn/README.md) (primary), [`ui-shadcncraft/`](ui-shadcncraft/README.md), [`ui-aicss/`](ui-aicss/README.md) (AI-specific), [`ui-astryx/`](ui-astryx/README.md), [`ui-spectrum/`](ui-spectrum/README.md) (components + MCP), [`ui-beautiful-ui/`](ui-beautiful-ui/README.md), [`ui-bencho/`](ui-bencho/README.md), [`ui-bestdesignsonx/`](ui-bestdesignsonx/README.md), [`ui-beui-pro/`](ui-beui-pro/README.md), [`ui-reverseui/`](ui-reverseui/README.md), [`ui-cue/`](ui-cue/README.md), [`ui-dialkit/`](ui-dialkit/README.md), [`ui-evil-buttons/`](ui-evil-buttons/README.md), [`ui-feralui/`](ui-feralui/README.md), [`ui-halaska/`](ui-halaska/README.md), [`ui-kobra/`](ui-kobra/README.md), [`ui-libraries-dev/`](ui-libraries-dev/README.md), [`ui-liquid-glass/`](ui-liquid-glass/README.md), [`ui-amicro/`](ui-amicro/README.md), [`ui-annnimate/`](ui-annnimate/README.md), [`ui-kinetics/`](ui-kinetics/README.md), [`ui-jakubkrehel-skills/`](ui-jakubkrehel-skills/README.md), [`ui-keyline-icons/`](ui-keyline-icons/README.md), [`ui-openui/`](ui-openui/README.md), [`ui-page-mascot/`](ui-page-mascot/README.md), [`ui-xiod/`](ui-xiod/README.md), [`ui-vibeprompts/`](ui-vibeprompts/README.md), [`design-book-of-shapes/`](design-book-of-shapes/README.md), [`design-playgrnd/`](design-playgrnd/README.md), [`design-quiver-ai/`](design-quiver-ai/README.md), [`design-kage/`](design-kage/README.md), [`design-typeface-fyi/`](design-typeface-fyi/README.md), [`design-uisfx/`](design-uisfx/README.md), [`design-specialized-galleries/`](design-specialized-galleries/README.md), [`design-md-resources/`](design-md-resources/README.md)

**Tool references:** [`tools-screenshot-to-code/`](tools-screenshot-to-code/README.md), [`tools-shotbase/`](tools-shotbase/README.md), [`tools-voicestudio/`](tools-voicestudio/README.md)

**UI pattern folders:** [`ui-patterns/pricing-tier-cards/`](ui-patterns/pricing-tier-cards/README.md), [`ui-patterns/features-blueprint-cards/`](ui-patterns/features-blueprint-cards/README.md), [`ui-patterns/design-inspiration-screenshots/`](ui-patterns/design-inspiration-screenshots/README.md)

Contributions: open a pull request that adds a folder from [`_template/`](_template/) plus a catalog row; entries are merged after maintainer review.


