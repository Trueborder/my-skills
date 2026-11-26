---
name: awesome-design-md
description: Use VoltAgent's bundled DESIGN.md collection when a frontend task calls for a named brand reference, design-system inspiration, or comparison of visual styles. Find the relevant local design document and adapt its tokens and component rules to the target website.
---

# Awesome DESIGN.md

This is a local adapter around [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md), a reference collection rather than an upstream Agent Skill.

## Find a reference

- Read [the upstream catalog](references/README.md) for categories and descriptions.
- Enumerate `references/design-md/` for the installed brands. Each brand has a `DESIGN.md`; some also have `preview.html`. Folder names include `linear.app`, `mistral.ai`, `opencode.ai`, `x.ai`, `bmw-m`, `dell-1996`, and `nintendo-2001`.
- Read only the selected brand's `references/design-md/<brand>/DESIGN.md`. For example, use [Linear](references/design-md/linear.app/DESIGN.md) for a Linear reference or [Apple](references/design-md/apple/DESIGN.md) for an Apple reference.

## Apply the reference

Extract the relevant palette roles, typography, spacing, layout, component states, and responsive rules. Apply the user's requested degree of similarity while preserving the target site's established branding, language, accessibility, behavior, and routes. When no brand is specified, choose a reference suited to the product and explain the choice briefly.

Treat these documents as third-party visual analyses, not proof of current brand specifications or permission to reuse proprietary fonts, logos, or imagery. Keep the reference inside this skill unless the task calls for a project design document; avoid replacing the project's DESIGN.md as an installation side effect.

The bundled files are an offline snapshot at revision `fcc70284932276d085f01ef9f83edde90b1258cb`. The upstream MIT notice is in [references/LICENSE](references/LICENSE).
