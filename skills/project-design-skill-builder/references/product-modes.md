# Product modes

Use this reference to choose the product's job before selecting a visual direction. A mode is a design priority, not a template.

| Mode | Typical surfaces | Primary success measure | Visual and interaction emphasis |
| --- | --- | --- | --- |
| **Operate** | Admin, workbench, tool, collaboration app | User completes the task accurately and quickly | Information hierarchy, states, keyboard flow, recovery, density, purposeful feedback |
| **Persuade** | Homepage, landing page, product intro, adoption pages | User understands the value and takes the next useful action | Clear proposition, proof, product demonstration, pacing, CTA hierarchy |
| **Read** | Docs, knowledge base, article, learning surface | User finds and understands information | Reading rhythm, outline, line length, anchors, calm transitions |
| **Experience** | Portfolio, exhibition, brand or editorial showcase | User follows and remembers the story | Atmosphere, spatial composition, media, scene transitions, controlled surprise |

## Mode-specific references

Read the guide for the primary surface, then select the applicable methods. A genuine secondary job may justify a second guide; the presence of four modes does not require loading or combining all four.

| Mode | Guide | Main coverage |
| --- | --- | --- |
| Operate | [operate-design-patterns.md](operate-design-patterns.md) | Task flows, work areas, data density, forms, selection, state/recovery and keyboard operation |
| Persuade | [platform-design-patterns.md](platform-design-patterns.md) | Product evidence, page composition, discovery, demonstrations and next actions |
| Read | [read-design-patterns.md](read-design-patterns.md) | Reader needs, navigation/search, anchors, content treatments and reading continuity |
| Experience | [experience-design-patterns.md](experience-design-patterns.md) | Collections/narrative, art direction, scenes, media, exploration and fallbacks |

Embed selected, project-specific decisions in the generated Skill or its own references. These guides are generator resources, not files the downstream user must fetch.

## Routing questions

Ask only what is missing:

1. What does the user come here to finish, understand, or feel?
2. Is success measured by completion, conversion, comprehension, or immersion?
3. Which content, state, or workflow must remain available even if the visual direction changes?

Assign modes per surface: a product may have an Operate editor, Read docs and a Persuade homepage. Setup onboarding often belongs to Operate; a learning guide belongs to Read.

If two answers compete, use the first job as primary mode and document the second as a bounded secondary mode. Do not blend all four into a generic “rich experience.”

## Constraint layers

Make these layers explicit in the generated Skill; the document structure can follow the project:

- **产品底线**: non-negotiable tasks, content, states, accessibility, performance, and technical constraints.
- **本次方案选择**: decisions for this project and this surface.
- **可选建议**: reversible experiments, alternate treatments, or future ideas.

## Mode boundaries

- Do not add hero sections, marketing copy, showcase media, fake demos, or conversion CTAs to an Operate or Read surface unless they serve a documented user task.
- Do not reduce a Persuade surface to a generic dashboard just because the product has complex features; show the product's real proof at the point it helps understanding.
- Do not make Experience an excuse for hidden navigation, slow loading, inaccessible text, or motion without a fallback.
- Images and complex motion are optional in every mode. Include them only when they clarify a task, prove a capability, establish a necessary atmosphere, or provide a meaningful state change.

## Flexible choices

Retain established components and tokens where they work. Record whether visual style is fixed, bounded or exploratory. Select page types by task: a queue, detail view and editor need not share one composition. A chosen layout or animation is a surface-specific decision, not a permanent product invariant. Revisit it when the task or evidence changes.
