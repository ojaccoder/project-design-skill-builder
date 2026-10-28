# Read: documentation, knowledge and long-form content

Use when users primarily need to find, understand or return to information. Read after [product-modes.md](product-modes.md). Adapt the guide to the actual content: a reference manual, learning article and policy page need different structures. Reading does not imply a bland visual style or a marketing layout.

## 1. Identify the reading task and content model

Inspect real documents, their navigation, metadata, links and rendering components. Determine what readers arrive knowing, what they need to learn or look up, and what they should be able to do afterward. Distinguish reading from editing the content or administering a knowledge base; those work areas may be Operate.

Use the content's purpose to choose its organization:

| Reader need | Useful structure | Important context |
| --- | --- | --- |
| Learn through a guided first attempt | Ordered tutorial with prerequisites and a visible outcome | Where the reader is and what is already complete |
| Complete a known task | Goal, prerequisites, steps, checks and recovery notes | Applicable product/version and consequences |
| Look up an exact fact | Consistent reference sections, terms, parameters and examples | Units, defaults, version and exceptions |
| Understand a concept or argument | Explanation with a clear line of reasoning | Definitions, supporting evidence and related concepts |
| Follow an article or research narrative | Meaningful sections, figures and source context | Author/date when relevant and the argument's progression |

These purposes can link to each other without being forced into one page template. Do not invent a documentation taxonomy or learning progression when the source material does not support it.

## 2. Make finding and returning reliable

Organize navigation with the reader's vocabulary and the project's existing content hierarchy. Make page titles distinguishable in navigation and search results. Use breadcrumbs when the hierarchy provides useful orientation; use a local outline when section length warrants it. A short article may need neither.

For existing or selected search:

- Define what content, language and version it searches. Keep the query visible and show enough surrounding context to distinguish results.
- Distinguish no matches from a failed search. Offer a useful query adjustment or an existing browse path.
- Preserve query and position when opening and returning from a result. Do not promise full-text or semantic search if the project only provides a local title filter.

Keep existing URLs and heading anchors stable where possible. If changing them is within scope, provide the appropriate redirects or anchor compatibility. Account for sticky headers when jumping to a section. Browser Back and deep links should return to meaningful content; do not reset the reader to the top on every small UI change.

For versioned or translated content, keep the current version/language evident when it affects interpretation. A version switch should preserve the corresponding page where a real counterpart exists; otherwise explain the actual destination. Do not fabricate equivalent translations or versions.

## 3. Build a readable text system

Define roles for title, headings, body, captions, lists, code and secondary metadata using existing tokens where suitable. Establish reading measure, line height and paragraph spacing from real content and the supported scripts, not one universal numeric recipe.

Check long Chinese paragraphs and mixed Chinese/Latin terms, English URLs, inline code and numeric units. Avoid isolated final characters in display headings where practical, but do not insert arbitrary manual breaks that fail at another width. Keep body text selectable and responsive to zoom.

Use heading hierarchy to express the document's structure. Visual size should not replace semantic headings. Provide a clear main-content region and a way to skip repetitive navigation. Avoid placing important text only inside images or using hover-only explanations for essential terms.

Keep navigation visually subordinate to the active content. Persistent controls should not consume the reading area or cover a focused anchor on small screens. A table of contents helps only if its labels are informative and it does not compete with every paragraph.

## 4. Treat different content types deliberately

| Content | Presentation decision | What to preserve |
| --- | --- | --- |
| Code or commands | Legible code block; copy action when useful; local overflow for long lines | Exact syntax, language, required context and honest copy feedback |
| Data table | Semantic headers, readable comparison and contained overflow if needed | Units, relationships and access to every cell |
| Procedure | Ordered steps, relevant examples and a checkable result | Prerequisites, sequence and necessary warnings before the affected action |
| Figure or diagram | Useful scale, caption and an appropriate text alternative | The actual relationship or evidence, not just a decorative summary |
| Callout | Consistent role for a genuine note, caveat or exception | Its meaning without relying only on color or an icon |
| Citation or source | Identifiable link near the supported claim | Authorship, date or version where material |

Do not style every paragraph as a card or every sentence as a callout. Keep exceptions visible without turning ordinary prose into a wall of warnings. Do not rewrite factual claims, commands or required legal text as part of a visual cleanup without authorization.

## 5. Protect continuity through states and interactions

Reserve media space when dimensions are known so loading does not keep shifting the paragraph being read. Keep content visible before decorative animation. Do not gate an explanation behind scroll reveals, autoplay or opening a series of unrelated panels.

Include applicable states in the generated rules:

- Missing or moved page: explain the actual condition and provide useful existing navigation.
- Empty category: distinguish an unpublished collection from a failed content request.
- Search loading/failure/no results: preserve the query and offer an appropriate next step.
- Image, embed or example failure: keep captions and a meaningful textual or static fallback available.
- Collapsed content: expose the control and state; preserve deep-link access to the relevant content when the product supports it.

Only include interactive exercises, progress, bookmarks or reading history when they exist or are explicitly selected for implementation. Never claim completion tracking or cross-device position persistence without support.

## 6. Use images and motion to explain

Choose images because readers need to understand an object, relationship, process or actual result. Use accurate diagrams for technical relationships and real screenshots for real UI. Generated illustration can establish an editorial mood when requested, but cannot stand in for factual evidence.

For a complex diagram, retain the key explanation in text or an accessible description; a generic “diagram” alternative does not convey its meaning. For screenshots, supply relevant context and ensure important labels remain legible at supported sizes.

Use motion when it explains a sequence or a change that a static view cannot show as well. Offer a stable alternative and controls when playback requires them. Keep ordinary reading calm; reduced motion must not remove the explanation. Record image and motion decisions separately, including an explicit omission when appropriate.

## 7. Adapt the reading area, not just the outer width

On narrow screens, give the main content room. Rehouse the section outline or navigation in accessible controls when needed; do not hide the only route to other content. Keep global and local navigation distinguishable.

Test code, tables, captions and long links separately from ordinary prose. Local horizontal overflow may be appropriate for inherently wide content; the whole page should not become a miniature desktop canvas. Keep content usable at enlarged text sizes and avoid fixed-height containers that clip translated or zoomed text.

Printing, offline access and export are conditional product needs. If selected or already supported, specify what happens to navigation, code, references and figures in those outputs; otherwise do not introduce new export functionality.

## 8. Put selected decisions in the generated Skill

Record the actual content/renderer/token paths, reader tasks, content types, navigation and anchor conventions, relevant version/language behavior, typography roles and special-content treatments. Include project-specific examples of a title, section, code/table treatment and necessary state where applicable; do not impose a fixed number of examples.

Example for a deployment guide: preserve the supported-version notice, copyable commands and existing section links; place prerequisites before commands; retain the reader's place after expanding a detail. If no search or progress API exists, do not add it to the design rules as an existing capability.

Embed selected guidance in the generated Skill or its own references so later implementation does not require this generator or a remote documentation framework.

## 9. Verify finding and understanding

When implementing UI, use actual long and short documents. Check that:

- A reader can find a specific answer from navigation or existing search, understand its context and return without losing the query or position.
- A deep link reaches the intended section without a sticky control covering its heading; Back behaves usefully.
- A reader can follow a representative procedure and identify its expected outcome without guessing prerequisites.
- Headings, lists, tables, figures and code retain meaning with keyboard navigation, text zoom and supported screen sizes.
- Version/language context, content failures and no-result states are truthful.
- Media loading, expanded content and reduced motion do not interrupt the explanation or make content unreachable.

Review the full reading sequence as well as representative screenshots. Generating design rules alone does not establish that the rendered documents have passed these checks.

## Reference provenance

These are synthesized reading-interface recommendations. [Diataxis](https://diataxis.fr/) informs the distinction among tutorial, how-to, reference and explanation needs; it is not a mandatory site taxonomy. [W3C WAI page structure](https://www.w3.org/WAI/tutorials/page-structure/) informs meaningful regions and heading structure; [WAI complex images](https://www.w3.org/WAI/tutorials/images/complex/) explains communicating essential diagram information beyond a short image label. These links are optional provenance, not runtime dependencies or a claim of a completed accessibility audit.
