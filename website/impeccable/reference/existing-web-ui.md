# Review existing web UI

## Dashboard polish

Start with the operator's main action and the data they need for it. Align icons and labels, make the current navigation item clear, and keep repeated controls in consistent locations. Check whether the sidebar still scans when labels wrap and whether dense desktop rows remain usable on touch.

Use the existing type roles. Align numeric columns and use tabular figures for changing counts and times. Compare the same role across screens. Check long translations and values at narrow widths before reducing text size.

Give loading, empty, stale, unavailable and confirmed states distinct wording. Show the last successful update where it helps users interpret old data. Display zero only when a source actually reports zero. Connect confirmation text and disabled controls to the system's actual state.

## Forms, tables and charts

Use native inputs with visible labels, stable identifiers, appropriate autocomplete hints and associated errors. Keep surrounding instructions and error messages readable when the keyboard opens. Preserve server validation and the existing submission and recovery flow.

Use a table for exact values and a chart for the comparison the user needs. Start with a line for a time series and ordered bars for category comparisons. Label units and the time window. Provide labels or line patterns alongside color, and make exact values available without relying on hover. Use the project's existing chart or table components where possible.

## Motion across a site

1. Inventory animated routes and components, shared timing and easing tokens, reduced-motion overrides, and interactions triggered by keyboard, pointer or data updates.
2. Sample busy and occasional paths. Test repeated toggles, fast reversals, route changes during transitions, narrow touch layouts and reduced motion. Use recorded or rendered evidence when available and identify gaps.
3. Rank findings by user impact. Start with blocked or delayed actions, broken focus, inaccessible movement and observed frame drops. Next check unnecessary motion on frequent controls, abrupt state changes, timing inconsistencies and duplicated tokens.
4. Report route or file, reproduction, impact and suggested fix. Call out any optional motion opportunity separately. Apply changes when the user asked for implementation.

Dashboard polish includes adapted guidance from [Unslop by Damir Sokolovsky](https://github.com/heydamir/unslop) under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). The review also condenses local references from `emil-design-eng`, `improve-animations`, `html-coder` and `ui-ux-pro-max`.
