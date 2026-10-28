# Rich, coherent platform websites

Use for Persuade surfaces and Experience surfaces with a documented product-adoption goal. For portfolios, exhibitions and authored experiences, start with [experience-design-patterns.md](experience-design-patterns.md); a conversion sequence is not their default. These are optional patterns, not defaults for operational applications or reading interfaces. These are synthesized design recommendations informed by the official-site observations, not claims that every reference implements every technique.

## 1. Show what the product does

Identify the tangible thing visitors can inspect: an output, a working surface, a model result, or a real scenario. Give it a large, legible stage. Product-linked media should carry more explanatory weight than a paragraph of adjectives.

For a design-skill library, examples include a background answer becoming a design token set, an actual page responding to a rule change, or a real before/after browser comparison. A paper sculpture can establish brand tone; it cannot explain generated project rules. Combine brand art with working UI where useful.

Pick the medium according to evidence:

| Goal | Effective medium | Implement it as |
| --- | --- | --- |
| Explain a workflow | Input → decision → actual output | Stateful DOM preview or guided demonstration |
| Explore capabilities | Select a scenario → matching result and action | Tabs with materially different content |
| Establish visual identity | Art-directed image or short visual scene | Local asset, intentional crop, text-safe area |
| Demonstrate motion/output quality | Real recording or playable result | Video with poster, controls and reduced-motion fallback |
| Support a purchase/adoption decision | Truthful constraints and evidence | Comparison, documentation, genuine case detail |

Do not fabricate logos, customer endorsements, metrics, model calls, or generated outputs. Label local demonstration where necessary without repeating the disclaimer everywhere.

## 2. Compose a page, not a stack of templates

Choose a dominant first-screen composition and a narrative sequence. Useful possibilities:

- Large product/media stage followed by compact selection controls.
- Centered product promise followed immediately by strongly differentiated action paths.
- Wide result showcase followed by a smaller, denser capability explorer.
- Real scenario preview followed by a concrete adoption path or developer example.

Vary the scale and density at meaningful boundaries. A wide feature stage, a compact comparison, and a scenario selector can coexist within the same grid, typography, palette and component language. Do not turn every section into headline + subtitle + three equal cards. Do not force variation into a short utility form or a dense operational dashboard.

Use colored or tonal section backgrounds to signal a new topic, focused capability, or interactive region. A gradient, dimensional asset, or glass treatment needs a role, consistent light/material direction, and readable contrast. Avoid globally banning techniques merely because generic templates also use them.

Establish a dominant, supporting, and quiet level of emphasis. A primary path and unavailable path should not appear equally actionable; use contrast, placement, scale and true state before adding status labels.

## 3. Give motion a scene and an outcome

Define each meaningful interaction as:

`trigger → subject → state change → timing → user benefit → fallback`

Example for this library: select baseline/new Skill → real evidence updates at the same scale → the matching rule/artifact becomes inspectable → a short interruptible transition preserves context → visitors can judge the result → instant update under reduced motion. Use project-specific scenarios only when requested or genuinely needed; do not invent a student app or unrelated product to fill a demo.

For a richer product reveal, sequence selection, focused input, generated artifact, and inspect/download state. One coherent focal sequence usually communicates more than animating every heading. Entrance animation, button lift, and pointer tilt remain supporting details.

Timing starting points, to tune to the content rather than enforce universally:

- Press/selection feedback: 100–180 ms.
- Tab/content transition: 180–320 ms, preserving the current layout anchor.
- Large media/scene transition: 350–650 ms when it helps track continuity.
- Demonstration playback: slow enough to read, pauseable, never blocking navigation.

No scroll hijacking. If using a sticky demonstration, keep it short, ensure all content is reachable on small screens and keyboards, and provide a natural document-flow fallback. Pause offscreen media; stop unsolicited playback for reduced motion; provide controls for prolonged automatic movement. Never infer performance or actual playback quality from a screenshot or a video element's presence.

## 4. Use media as a coordinated set

Plan subject, function, crop, text-safe area, light, material and palette per asset. Reuse composition rules for consistency, not one image everywhere. Do not add images solely to fill empty sections.

For product websites, use real browser UI and actual output examples alongside generated brand imagery. For video, capture real interaction when evidence is needed; use authored motion graphics only as explicitly labeled illustration. Keep important text in HTML. Provide image dimensions, loading strategy, poster and media fallback; defer below-fold media.

## 5. Make exploration change something

Tabs, carousels and navigation need meaningful destinations, not color-only theatrics. Match preview, title, explanation and CTA to the selected state. Preserve keyboard navigation and selected semantics.

Use a carousel when visitors benefit from browsing related examples; do not hide the only essential explanation behind auto-rotation. Offer visible controls, pause behavior, and a mobile swipe/stack alternative. A large product catalog may need category tabs and compact grids; a small library may only need a few scenario previews.

## 6. Keep the words lean

Avoid unnecessary secondary labels and descriptions. Let the layout do the explaining.

Remove copy that paraphrases an obvious component. Keep necessary names, form labels, errors, limitations and state. Show the result before explaining that results exist. Do not add English eyebrows, numbered markers, chips or tooltips merely to make the interface look designed.

## 7. Acceptance checks for expressive websites

Review one desktop and one mobile sequence. Confirm:

- First-screen promise and next action remain obvious despite richer media.
- Media communicates the actual subject/product, not just mood.
- The middle of the page adds evidence or exploration, not another hero.
- Section rhythm changes without losing the shared identity.
- A representative interaction produces a meaningful state change.
- Reduced motion, loading failure and mobile do not remove the explanation.
- Content is readable and usable before animation starts.

If the brief asks for visual richness and the result is only huge type, whitespace, one picture and thin rules, revise the composition and evidence. Do not compensate with more words or random animation.

For detailed visual extraction and concrete source relationships, use [visual-direction.md](visual-direction.md). Product-flow analysis does not replace typography, material, crop, shape and composition analysis.
