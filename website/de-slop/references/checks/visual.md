---
type: check
layer: 2-company
status: active
last-refreshed: 2026-11-01
source: tomaspisar.cz/assets/css/tokens.css and site styles
---

# Check: visual

Grade only the product and account interfaces in this Website repository. The public site uses a warm neutral canvas, dark ink, teal action color, amber decision/focus color, and coral for warnings. Typography uses Barlow Condensed for display, Barlow for body text, and DM Mono for compact labels. Preserve this system and distinguish the public studio site from the product-branded account portal.

## Design language

Use a practical, editorial interface with clear hierarchy and restrained technical detail. Keep decorative grids, uppercase micro-labels, and product previews subordinate to the content. Account screens should make the current task and state clear. Do not flatten intentional product branding or functional state cues.

## Palette and type

Use the shared tokens in `tomaspisar.cz/assets/css/tokens.css` as the source of truth: bg `#f2f0e9`, surface `#fbfaf6`, text `#11191c`, muted `#58676b`, line `#bcc9c7`, cyan `#087f70`, amber `#9c5d08`, coral `#a74231`. Use the three declared font families and fallback stacks. Keep body copy comfortably readable and functional controls clearly distinguishable.

## Structural rules

Use the existing spacing and width tokens. Prefer clear surfaces, subtle borders and intentional shadows over gratuitous layered cards. Preserve visible focus, responsive layouts, contrast, and reduced-motion behavior. Flag generic decoration only when it competes with task clarity or conflicts with the actual tokens.

## Surface application

- Public marketing and product pages: a clear product choice, direct descriptions, consistent Novaryn identity, English/Czech parity where provided.
- LJR account pages: focused account task, LongJumpReplay identity, readable form labels, truthful status, and no ornamental content that obscures login or account actions.
- Legal pages: legible document structure, accurate language and operator state; do not hide unresolved placeholders.

## Grading

Aligned means the actual token palette, typography and hierarchy support the page task, with functional accessibility intact. Drift means a minor hierarchy or spacing inconsistency. Misaligned means unreadable text, deceptive state, broken language/navigation, inaccessible interaction, or a visual system that competes with the task.
