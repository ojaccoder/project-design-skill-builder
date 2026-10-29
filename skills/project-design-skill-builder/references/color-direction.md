# Choose a theme for this project's users

Use before selecting or changing colors in any product mode. This is a decision method, not a palette catalogue. Embed the selected decisions in the generated project Skill so implementation does not depend on this reference.

## Start with evidence

Collect only the context that changes the choice:

- **People and activity:** what users are trying to do, what they compare, and which errors matter.
- **Environment:** supported devices, session length, density, lighting or usage conditions when actually known.
- **Brand and content:** existing tokens, supplied references, recognizable assets, photography and explicit preferences or exclusions.
- **Expression:** what the interface should communicate while supporting its task; distinguish a brand impression from an operational need.

Label unknowns as assumptions. Do not infer that young users want neon, women want pink, technical users want blue, cultural products want beige, or dance bookings happen at night. A user's actual preference is stronger evidence than a category association. Preserve confirmed brand constraints, while allowing the project's theme to change within the user's authorization.

“Quiet,” “clean,” “premium,” and “expressive” describe desired effects, not specific hues or light/dark modes. They do not by themselves justify warm off-white, black or any other canvas.

## Ask whether the current color is a brand constraint

An existing project's theme may change. Its current color values, a variable named “brand,” and an assistant's earlier color choice do not establish a brand requirement. “Keep brand continuity” is not a sufficient reason when the user has never confirmed the brand or its protected colors.

Before choosing whether to preserve or replace an unresolved theme, ask one concise question:

> 当前主色是必须保留的品牌色，还是可以重新设计的主题色？

Use the answer:

- **No fixed brand color / redesign authorized:** reassess the theme against the actual tasks, imagery, context and stated taste. Keeping, adjusting and replacing colors are all valid outcomes; continuity is not a default constraint.
- **Required brand color:** keep the confirmed protected color and ask about its scope only if necessary. A protected logo color does not automatically fix page backgrounds, surfaces, secondary colors, selection or status roles.
- **Some colors protected, others open:** record those boundaries and design within them.
- **Already answered in the session:** use that answer and do not ask again. An explicit instruction to change the theme is authorization within its stated scope.

While a necessary brand clarification is pending, continue independent work such as task-flow analysis, preserving the comparison baseline and checking functionality. Do not silently decide that an unknown color must stay or must change. Record the user's answer as a constraint; record the existing palette only as implementation evidence.

## Make a deliberate choice

When no confirmed brand or user decision determines the theme, consider a small set of plausible directions, including a new theme for an existing project when authorized. Compare what changes the experience: dominant canvas luminance and temperature, surface separation, accent emphasis, content compatibility and reading comfort. Do not manufacture alternatives when the user has already confirmed which direction to preserve.

Select a direction for its task fit and expression, and record one meaningful tradeoff. Keep unselected candidates brief; the user need not approve a mood board unless their preference is necessary. Familiar patterns and palettes remain valid when justified. Difference for its own sake is not a goal.

These examples show reasoning boundaries, not prescribed themes:

| Context | Evidence that could change the choice | Decision to make |
| --- | --- | --- |
| Dance rehearsal space booking | Room photography, individual versus group rehearsal, device use, stated brand taste | How to express movement while keeping capacity, time and price easy to compare; do not assume a nightclub aesthetic |
| Teacher research workspace | Long reading/editing sessions, dense source material, existing school or product branding | Canvas contrast, annotation colors and restrained action emphasis; an academic identity does not require cream |
| Exhibition or cultural collection | The works' own colors, curatorial intent, visitor reading needs | Whether the canvas recedes or participates in the exhibition; avoid tinting or overpowering the artifacts |

Use a short project-specific record:

> **Evidence:** supplied facts and clearly labeled assumptions. **Choice:** theme and its role in the task and expression. **Tradeoff:** what this choice gives up or needs to protect. **Revisit when:** new brand, user or usage evidence would change it.

Write this in the design rules, not as visible product copy. Do not present inferred preferences as user research or claim improved conversion without measurement.

## Translate the choice into semantic roles

Provide concrete values or existing token names for the roles the actual interface uses. Scope them to relevant surfaces rather than making one page's palette a universal rule.

| Role | What the implementation needs to know |
| --- | --- |
| Canvas and surfaces | Dominant page field, containers, raised surfaces and overlays; define light/dark or mixed regions if selected |
| Text and muted content | Readable primary and secondary text on each applicable surface; muted must remain legible |
| Boundaries | Dividers, field borders and separators that communicate structure |
| Action and on-action | Primary button/link emphasis and a readable foreground for each action background |
| Selection and focus | Selected date, tab or row; keyboard focus visible on the applicable surfaces |
| Status | Applicable success, warning, error and unavailable states, supported by text or icons |

Assign colors by meaning instead of scattering literal values through components. Distinguish brand accents from status meaning. A prominent accent need not fill every container; a quiet neutral canvas can still be an intentional choice. Do not tint the full interface with a brand hue just to make it feel less generic.

The generated Skill must name the relevant project token files, CSS variables or component theme boundary when known. If the stack is not yet selected, provide a semantic table and an implementation mapping requirement rather than inventing paths.

## Review the result, including its background

For rules-only work, check the reasoning and token roles without claiming to have inspected a rendered page.

For implementation work:

- Inspect the first, middle and final viewport. Confirm the computed canvas, containers, form fields and overlays use the selected roles. A changed CTA with the same unintended cream background is an incomplete theme update.
- Exercise selected, hover, focus, disabled and error states that the flow can reach. Check text and control contrast in their real background combinations; do not rely on hue alone for status.
- Check long Chinese labels, time/price values and image crops on supported desktop and mobile sizes. A strong brand treatment must still allow quick task completion.
- Keep any comparison baseline independent when the user requested a controlled before/after or A/B demonstration.

Before accepting the palette, ask whether its rationale names this project's users and task or could be pasted into an unrelated brief unchanged. If the reasoning is generic, revisit the evidence or the choice. Reusing a proven system is valid when the reason is explicit; randomizing hues or replacing cream with one universal dark/neon preset repeats the same failure.
