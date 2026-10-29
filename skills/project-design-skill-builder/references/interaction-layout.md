# Interaction and layout from real tasks

Use when turning project context into task paths, information order and interface structure. Combine with the relevant product-mode guide. This is a synthesis of public guidance, with project adaptations and limits; it is not a fixed page template or a substitute for user research. Selected rules belong in the generated project Skill itself.

## 1. Start with a situation and an outcome

Describe who arrives, what triggers the task, what they already know, their relevant device/environment constraints, and what successful completion means. Reuse repository evidence, supplied research and user answers. Mark missing evidence as assumptions; do not invent personas or claim research occurred.

Map the useful path at the detail warranted by the task:

`entry context → find the object/content → inspect and decide → act → understand the result → continue or return`

For a reading or experience surface, “act” may be following a reference or exploring a work; do not add a transaction funnel. For an operational flow, include a relevant failure or change-of-mind path. Distinguish new and returning users only when their needs actually differ.

**Project example, not research evidence:** a rehearsal group knows its date and group size. Capacity, availability and total price matter before contact details; a returning visitor may instead need to find or cancel an existing booking. Arrange those decisions around what is known rather than opening with a generic feature tour.

Basis: [GOV.UK user needs](https://www.gov.uk/service-manual/user-research/start-by-learning-user-needs) and [USWDS design principles](https://designsystem.digital.gov/design-principles/). Their public-service context informs the method, not a requirement to copy government layouts or processes.

## 2. Reduce effort, not just clicks

Identify steps that make people detour, re-enter known data, guess a label or carry information between screens. Remove or combine them when the actual business rules allow it. Keep necessary permissions, eligibility checks and consequential decisions; explain their purpose at the point it matters.

Keep information that users compare or adjust together within a useful shared context. Stage genuinely separate decisions when that improves comprehension. A single huge screen and a wizard with one trivial field per step can both add effort. Do not invent gates, nested overlays or extra confirmations just to make the flow look substantial.

Preserve search, filters, selections, position and entered data on return where the product supports it; specify any missing behavior as proposed work rather than implying it already exists. Favor useful defaults when their assumptions are safe and visible. Frequent actions may have shortcuts, while the visible path remains understandable.

Do not require “three clicks,” an arbitrary number of steps or a universal maximum depth. Evaluate meaningful decisions, repeated work, uncertainty, recoverability and completion of the actual task. Basis: [NN/g on the three-click rule](https://www.nngroup.com/articles/3-click-rule/); context retention is this guide's application of the broader control and recognition principles below.

## 3. Give actions a clear priority

Within a task area, make the next useful action recognizable. Distinguish it from secondary navigation, optional tools and destructive actions through position, emphasis and clear labels. Place actions beside the object or decision they affect; distinguish navigation to a destination from a mutation.

In a single-purpose form, competing equally prominent submit actions make the next step ambiguous. An editor with independent work areas can have separate local primary actions; do not impose one primary button on an entire application. Reserve interrupting confirmation for consequences that warrant it, not routine reversible actions.

Button text should predict the actual result. Keep cost, timing, eligibility and important consequences available before commitment. Basis: [GOV.UK buttons](https://design-system.service.gov.uk/components/button/); the per-task-area scope is an adaptation for interfaces beyond government forms, rather than a quotation of GOV.UK's page-level guidance.

## 4. Make layout express relationships

Establish an intended reading order: current location/object, decision-critical content, current action, and supporting detail as the scenario warrants. Use relative scale, weight, contrast and placement to communicate importance; not every item can be the focal point.

Keep labels and headings close to their content. Use a consistent alignment axis and spacing rhythm, with clearer separation between unrelated groups than within a group. Borders or containers should clarify a real relationship; avoid wrapping every label and value in another card. Repeated rows or cards are useful when they make comparison predictable.

Choose the work area from the decision: a list/table for comparing stable fields, a list/detail split for inspecting objects while retaining a queue, a grouped form for dependent input, or a readable content column for sustained reading. Keep comparable values and units aligned. These compositions are project adaptations, not a mandatory component library.

On smaller screens, preserve the useful order and essential actions. Reflow or change the composition rather than shrinking all desktop panels. Keep content order, keyboard order and visible focus coherent; check long labels and realistic values. Basis: [NN/g visual hierarchy](https://www.nngroup.com/articles/visual-hierarchy-ux-definition/). Its examples inform relationships, not a mandatory number of font sizes, grid columns or spacing tokens.

## 5. Reveal detail without hiding the decision

Show common, decision-critical information directly. Defer infrequent advanced options and lengthy secondary explanation when users can find them predictably. Use explicit labels that indicate what will expand or open.

Do not hide required fees, availability, consequential constraints, form errors or the primary action merely to make the surface cleaner. Repeated opening and closing to compare basic facts is a signal that disclosure has split the wrong information. Preserve the chosen values when showing additional detail.

Basis: [NN/g progressive disclosure](https://www.nngroup.com/articles/progressive-disclosure/). Select disclosure by actual frequency and task dependence, not by a rule that every screen needs tabs, accordions or an “advanced” drawer.

## 6. Keep users oriented and able to recover

Use the users' business vocabulary consistently, and show important choices where they are needed rather than requiring recall. Make the current object, selection and operation state clear. Distinguish pending from completed work; show a confirmed result and the next available action.

Provide a clear way to leave a bounded task, go back or correct a choice. Support undo only when implemented; otherwise describe the real recovery path. Prevent accidental repeat submission and costly errors where the actual workflow warrants it.

For forms, use persistent labels, actionable errors near affected fields and an error summary when errors may be out of view. Associate messages with controls; after submission, guide focus to a useful error location without interrupting every keystroke. Retain valid input when correcting errors. Choose inline feedback, a persistent status or an overlay according to the attention needed; not every result needs a modal.

Basis: [NN/g usability heuristics](https://www.nngroup.com/articles/ten-usability-heuristics/) for status, vocabulary, control, consistency, recognition and recovery; [W3C WAI form notifications](https://www.w3.org/WAI/tutorials/forms/notifications/) for accessible feedback and error association. Retention and duplicate-submission behavior must be verified in the project, not inferred from a success message.

## Carry the choices into the generated Skill

Record only what changes the implementation:

| Project decision | What to make concrete |
| --- | --- |
| Scenario and finish | Starting knowledge, relevant usage conditions and observable outcome; label assumptions |
| Task path | Necessary decisions, removed detours and any business constraints that keep a step necessary |
| Information and actions | Fields users compare, what remains visible, primary versus secondary actions and grouping |
| States and continuity | Pending/result/error, preservation on return and actual recovery behavior |
| Responsive behavior | Which work areas reflow and which information/actions remain available |
| Verification | A representative task and return/error path, plus the observations required to assess them |

Do not paste a long universal checklist into every project's rules. A small search page and a complex editor need different detail. Keep the three constraint layers: real business/accessibility invariants, this solution's choices, and unselected experiments.

## Verify through a walkthrough

Walk through the representative scenario using realistic content. Check whether the user can find the correct item, make the decision without unnecessary memory or backtracking, identify the action, understand its outcome and continue. Exercise a relevant changed-choice or failure path; compare the intended hierarchy with the rendered page at supported sizes.

Record observed friction, such as a lost filter, hidden total, repeated field, ambiguous next step or an unavailable recovery action. If comparing designs, keep task/data conditions comparable and describe differences without inventing efficiency percentages. An agent walkthrough establishes observed behavior, while claims about real users need actual user testing. Revisit assumptions when that evidence becomes available.

## Source record

The eight linked primary sources were read on 2026-10-29. They support the named principles, not the fictional project example or every implementation suggestion. The rules above are paraphrased and adapted; users do not need to install their design systems, adopt their visual themes or reread them to execute a generated project Skill.
