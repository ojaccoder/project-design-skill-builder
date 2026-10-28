# Experience: portfolios, exhibitions and editorial worlds

Use when the primary job is exploring, encountering or remembering content: a body of work, an exhibition, a place or an authored story. Read after [product-modes.md](product-modes.md). An Experience surface can be quiet, expressive or immersive. It does not automatically need a sales funnel, a carousel, a cinematic introduction or 3D.

## 1. Start from the subject and intended experience

Inspect the actual works, project records, imagery, narrative text, media and available interactions. Establish what the visitor should encounter, understand or feel, and which content must remain identifiable. Distinguish facts supplied by the project from an art direction proposed for this design.

Choose a structure that serves the material:

| Content and visitor intent | Useful structure | What keeps visitors oriented |
| --- | --- | --- |
| Browse a body of work at a chosen pace | Legible collection/index with project or work detail | Titles, meaningful ordering and a return path |
| Follow an authored argument or story | Editorial sequence with deliberate changes of scale | Section identity, coherent reading order and continuation |
| Encounter a curated exhibition | Chapters, rooms or thematic clusters | Current location, accessible alternatives and a way to revisit works |
| Inspect spatial or material qualities | A focused scene or object view, if the assets support it | Discoverable controls and an equivalent descriptive/static view |
| Experience an audiovisual piece | Explicit entry/playback with supporting context | Playback controls, text alternatives and a clear exit |

These can be combined only where the content warrants it. A portfolio may work best as a direct index; an exhibition may invite a guided sequence. Do not impose a linear journey on a reference-like archive or a freeform canvas on a short article.

If the actual primary goal is adoption or purchase, classify that surface as Persuade and use [platform-design-patterns.md](platform-design-patterns.md). Add its conversion patterns to an Experience surface only for a documented secondary job. A meaningful ending can be a work index, credits or a return path; a commercial CTA is not mandatory.

## 2. Plan the content sequence before the spectacle

Map the selected content in order or by relationship. For each chapter or region, identify:

`subject → visitor action or attention → revealed meaning → transition or next choice`

Establish orientation, an encounter with the actual material, development and an appropriate ending when the structure calls for a sequence. These are narrative functions, not four required page sections. A visitor entering through a deep link should still understand the current work and find a useful path onward.

Vary scale, proximity, density and pace where the content changes. Give important work enough space, then use quieter supporting regions to make details readable. Do not make every region a full-screen hero or repeat an identical title-plus-three-cards layout. Repeated frames are useful when they invite comparison among related works.

Keep titles, creators, dates, captions and credits when they identify or explain the work. Remove ornamental labels that narrate the interface rather than the subject. Do not invent an artist statement, testimonial, provenance or exhibition history.

## 3. Define a coherent visual language

Select typography, palette, shape, material, light, crop and spatial relationships from the content and brief. Document their roles and the existing project tokens/components they affect. A visual signature should have a reason to recur; it need not be a logo-like motif on every section.

Choose the dominant subject and its relationship to text. Preserve useful negative space and deliberate overlap, but keep reading order and contrast clear. Set art direction across the media set rather than applying one image everywhere. Keep essential text in accessible page content; decorative lettering must not become the only title or navigation label.

Make crop rules specific to the asset. A full-bleed scene, a complete artwork and a readable document image need different treatment. Preserve the supplied subject and material details; do not crop out the feature visitors are meant to inspect. Where a complete view matters, provide it through the selected existing interaction or composition.

Explore genuinely different structures when a user choice is needed: for example, a browsable archive versus an authored sequence. A color swap or changing which side holds an image is not a different narrative approach.

## 4. Give motion a subject, a role and an exit

Use motion to direct attention, reveal a relationship, express a material quality or establish an intended rhythm. Do not require a utility justification for every expressive movement, but be able to name the experience it contributes to.

For each selected scene or interaction, record:

`trigger → subject → start/end states → timing and pacing → intended effect → interruption → reduced-motion/static alternative`

Choose which element moves and which anchors the scene. A stable title or navigation region can help visitors follow a larger media transition. Stage a small number of meaningful changes rather than animating every caption and control. Tune duration to the subject and reading time; do not impose a universal reveal speed.

Keep visitors in control. Let them skip an introduction or leave a scene without waiting for playback. Avoid scroll hijacking and interactions that depend solely on pointer position. If scroll-driven choreography is selected, preserve ordinary document navigation and access to all chapters with keyboard, touch and reduced motion.

Do not make a loading animation stand in for content, or hide essential work until an entrance animation completes. Continuous decorative motion needs a practical way to stop when it competes with content. Most interactive web motion should be implemented in the existing stack or native APIs; a generated video is appropriate only when the selected deliverable actually requires video.

## 5. Make exploration discoverable

Show enough affordance to understand what can be opened, selected, advanced or manipulated. Preserve the content's identity when changing presentation. Do not use a custom cursor, hover state or drag gesture as the only navigation cue.

For a gallery or object interaction, specify the selected item, previous/next behavior, detail entry and exit, and return context. Provide visible controls for important gestures. Keep controls keyboard accessible and focus states legible against the media.

Overlays and full-screen views should have an evident close/exit path and useful focus return. A selected work should remain addressable when the project supports routes or deep links. Browser Back should not unexpectedly restart the entire experience. Avoid trapping page scroll while a media control only needs a small adjustment.

An interaction should reveal actual additional content, perspective or meaning. Do not add fake hotspots, empty scene selectors or filters that only alter accent color. A static editorial presentation is valid when interaction adds no value.

## 6. Plan media as usable assets

For each chosen asset or related set, record its role, supplied/generated source, local path, aspect ratio, composition, crop behavior, text-safe area and fallback. Distinguish authentic work/documentation from commissioned or generated atmosphere. Do not fabricate real works, records, people or events and present them as existing evidence.

| Medium | Decisions to carry into implementation |
| --- | --- |
| Photography or illustration | Appropriate source, desktop/mobile crop, dimensions and meaningful alternative text |
| Video | Real file, poster, playback trigger, controls and a static/textual alternative |
| Audio | Explicit playback choice, useful controls and transcript or other appropriate equivalent |
| 3D or WebGL | The actual model/data, discoverable controls, loading/error behavior and useful non-WebGL content |
| Editorial text | Reading order, type roles, captions/credits and access independent of animation |

Use existing assets when they serve the selected direction. When generated raster art is selected, the later implementing assistant must create it with the available image capability and connect the real file; a prompt or placeholder is not the asset. State unavailable capabilities accurately. Do not quietly replace selected work with an unrelated decoration.

## 7. Design the experience under ordinary constraints

Prioritize the first meaningful content and the active scene. Use appropriately sized assets, reserve media space and defer heavy offscreen work when useful. Avoid requiring all high-resolution media or a 3D engine to finish loading before visitors can navigate.

Specify what visitors see while media loads, if it fails, or when reduced motion is enabled. A fallback should retain the subject and explanation, even if it cannot reproduce the same atmosphere. Do not leave a permanent empty canvas or an endless loading loop.

Translate the composition for touch and smaller screens. Reconsider overlaps, crops and panel relationships rather than shrinking the desktop scene. Replace hover-only disclosure with a visible/tappable equivalent. Keep captions and controls readable, and account for changing mobile viewport height if a scene uses viewport-sized regions.

Respect the user's motion and playback choices. Sound should not unexpectedly start. Provide appropriate captions/transcripts and alternatives for meaningful audiovisual content. Do not mistake successful desktop playback or a screenshot for proof that mobile, keyboard or reduced-motion behavior works.

## 8. Put selected decisions in the generated Skill

Include the actual content/asset/component/token paths, the experience's purpose, chosen navigation model, content sequence or collection relationships, visual language, media decisions and interaction scenes. Define the fallback alongside the selected treatment, not as an unrelated future suggestion. Scope each composition to its surface.

Example for an existing ceramics portfolio: choose whether visitors browse a collection or follow an editorial sequence; keep real work titles and material details; specify how photographs show both whole objects and texture; define the existing detail/return path. Do not assume an online shop, contact funnel, 3D scanner or soundtrack.

Embed the selected guidance in the generated Skill or its own references. The next assistant should be able to produce the chosen experience without fetching this generator or copying the reference websites.

## 9. Verify the encounter and the paths through it

When implementing UI, review an actual sequence on supported desktop and mobile layouts. Check that:

- A first-time visitor can identify the subject, find an entry and understand how to continue or leave.
- An actual work remains identifiable through selection, detail, media playback and return.
- The beginning, middle and ending develop the content rather than repeating one visual treatment.
- Keyboard, touch, direct entry and browser Back have useful paths through the selected structure.
- Media failure, slower loading and reduced motion retain the essential material and usable navigation.
- Crops, captions, contrast and text size work at real display sizes; generated/supplied assets follow the chosen art direction.
- Motion can be interrupted where needed, playback can be controlled and no decorative sequence blocks content access.

Capture screenshots for composition; exercise real triggers for behavior. Use recordings when motion is a deliverable or interaction alone cannot establish the result. A rule-generation task does not claim the media or experience has already been built.

## Reference provenance

These are synthesized experience-design recommendations, not measured results from the platform-site study. [W3C WAI animation from interactions](https://www.w3.org/WAI/WCAG22/Understanding/animation-from-interactions.html) informs optional-motion alternatives; [WAI pause, stop, hide](https://www.w3.org/WAI/WCAG22/Understanding/pause-stop-hide.html) informs control of qualifying automatic movement. These are focused primary references, not a claim that this guide alone establishes WCAG conformance. For dated website observations, see [official-site-observations.md](official-site-observations.md); those examples are not required compositions for an exhibition or portfolio.
