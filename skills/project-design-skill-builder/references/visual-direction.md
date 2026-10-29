# Learn the visual system, then compose the project

Use selectively when visual exploration is needed. First establish the surface mode; a monotonous workbench may need better density and hierarchy rather than marketing imagery. For the task model, use [operate-design-patterns.md](operate-design-patterns.md), [read-design-patterns.md](read-design-patterns.md) or [experience-design-patterns.md](experience-design-patterns.md) as appropriate. The website examples below apply primarily to Persuade / Experience, and do not replace those mode-specific methods. This reference embeds the method; it requires no additional Skill.

## Inspect what is actually rendered

Open the named source in a real browser. Review the first screen, one representative content or task screen, a media screen if relevant, and supported responsive layouts where accessible. A text scrape cannot establish layout, typography, depth, crop, color or motion quality. Save screenshots and distinguish loaded content from placeholders. When a user asks to see the site, open its actual URL in the available visible browser; do not imply a background capture changed their current tab.

Extract a few decisive relationships, not an inventory of widgets:

- **Type:** display-to-body scale, weight contrast, Chinese line breaks, line height, headline measure, optical alignment.
- **Composition:** content edges, hero height, alignment axes, text-to-media area, whitespace distribution, first-fold cut.
- **Color:** dominant canvas (neutral, tinted or saturated as actually observed), brand field, active accents, muted states, text contrast, section transition. Treat a source's background as evidence about that source, not the default for the new project. Use [color-direction.md](color-direction.md) to connect the new theme to its audience and usage context.
- **Shape:** which layers get large radii, which controls are pills, where straight edges carry structure. One radius applied everywhere erases hierarchy.
- **Depth:** foreground, subject, background; material, directional light, grounding shadow, overlap and edge crop. Multiple borders do not substitute for depth.
- **Motion:** which large subject changes, what stays still, duration/easing, image continuity and state transition. A video tag is not proof of a successful animation.

Use browser-computed metrics when helpful; record them as source observations, not mandatory values for the new project.

## Concrete visual observations from the official-site study

Source URLs and access limits are in official-site-observations.md. These are dated observations, not an endorsement or conversion claim.

| Source | Visually observable relationship | Transferable decision |
| --- | --- | --- |
| Qwen Open Platform | Neutral field, strongly weighted centered Chinese headline with local blue emphasis; black capsule CTA; saturated primary access panel next to a subdued panel; translucent cropped artwork; a later softly colored capability region with mixed tile proportions | Distinguish primary and secondary surfaces through contrast, scale and material; let the brand-color surface carry emphasis while the surroundings stay calm |
| ByteDance Seed | Short large statement above a broad model-media stage; model name and actions anchored near the lower edge; adjacent panel peeks into view; restrained controls; later compact news followed by a large product demonstration | Treat media as a stage with stable typography/action anchors; put room and visual energy into the actual result instead of repeated descriptive cards |
| Volcengine | Compact functional header, centered lightweight display type, high-contrast action, wide visual strip; further down, a dark setup surface opposite a white dense model list | Alternate scale, luminance and density according to content; large regions and compact utility can coexist without wrapping every item in a floating card |

Do not copy exact gradients, colors, radii, illustrations or brand marks. A source's glass artwork is brand expression; its specific shape is not a universal AI-site requirement.

## Establish a deliberate visual world

For an expressive surface in any mode, consider the relevant items below. Operate / Read also need appropriate hierarchy, density, typography and component roles; those requirements do not prohibit an audience-led visual world:

1. The visitor's visual impression and the product truth it should express.
2. The dominant composition and biggest visual subject.
3. Type contrast and headline line breaks at desktop/mobile sizes.
4. The role of each color and the primary/secondary surface contrast.
5. The shape/material/lighting rules and how layers are grounded.
6. Where section scale and density change, and why.

Avoid adding these statements as interface copy. They are instructions for building the interface.

If the brief calls for richness, concentrate detail in a hero, demonstration or result stage and give supporting areas room. Richness comes from composed scale, contrast, material, crop and movement; extra UI chrome and explanatory labels can dilute it. If the product needs dense utility, keep the useful content dense rather than inflating it into a marketing layout.

## Visual defects to correct

- Every section uses the same white card, equal gap, thin border and medium title.
- A large heading sits far above a small product sample, so neither forms a strong composition.
- Nested fake browser/editor windows make the visitor decipher the frame before seeing the result.
- Decorations occupy the strongest focal area while actual outputs appear as tiny, low-contrast thumbnails.
- A saturated background, status labels, chips and toolbar all compete with the main subject.
- One generic image is repeated under different labels without conveying a distinct content purpose.
- Important Chinese phrases wrap awkwardly or produce single-character orphan lines.
- A beautiful desktop crop becomes a clipped headline or unreadable miniature on mobile.

Use nested UI when explaining a real multi-surface relationship, not as an automatic sign of sophistication. If an actual screenshot already proves the point, show it at a useful size.

## Pair visual quality with product clarity

Determine what the visitor should understand, trust and do next. The page's strongest visual evidence should support that chain. For this design-skill library, direct page comparisons, readable actual Skill files, genuine recordings and a working download are stronger evidence than unrelated sample applications. Do not invent a three-scenario explorer merely because a large platform has one.

## Review

Review the rendered page at real display size. Check the first screen as one composition before reviewing details. Confirm that the strongest contrast belongs to the intended subject/action, that images and text share a common art direction, and that the middle and end of the page add evidence rather than repeat the opening. Explain remaining issues in concrete visual terms: scale, alignment, hierarchy, density, crop, material or state. Avoid verdicts consisting only of “more premium” or “more dynamic.”

### Measured examples, 1440×1000
On 2026-10-26, computed styles from real browser visits showed Qwen Open Platform's hero at 66px/700, line-height 77.88px, and its main CTA at 160×58px with fully rounded corners and a soft grounding shadow. Volcengine's hero was 64px/300, line-height 89.6px, with a 130×52px CTA using a 2px radius and no shadow. Seed's active model name was 60px/500 with a 57px line-height; its media actions were smaller and subordinate. These differing systems are evidence against applying one universal font weight, corner radius or shadow across all “big-company style” sites.
