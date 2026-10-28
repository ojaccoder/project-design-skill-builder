# Operate: workbenches, administration and tools

Use when the primary job is completing work accurately: processing a queue, editing a record, comparing resources or coordinating a task. Read after [product-modes.md](product-modes.md). Select the patterns supported by the actual project; this is not a requirement to build a dashboard, add features or adopt a component library.

## 1. Map the work before arranging the screen

Inspect representative routes, components, data and role rules. Establish the actor, object, entry point, decision, action and observable result. Include the path back to ongoing work:

`enter → locate → inspect → decide → act → confirm result → continue`

Record what makes the work difficult: volume, similar records, missing information, urgency, permission boundaries or an expensive mistake. Use observed product facts; do not invent personas, usage metrics or business rules. Separate an improvement to presentation from a change to the workflow or API.

Choose the work area by the task, not by the word “admin”:

| Task | Useful composition | Context to preserve |
| --- | --- | --- |
| Compare and process many records | Filterable table or structured list with relevant row actions | Query, sort, page, selection and return position |
| Inspect a record while scanning a queue | List/detail split or a detail route with a reliable return path | Active record, queue position and pending changes |
| Create or edit structured information | Grouped form; steps only when there are meaningful stages | Entered values, dependencies and validation results |
| Manipulate a document or visual object | Dedicated editor with contextual tools | Selection, viewport and real save state |
| Triage exceptions | Actionable summary linked to the affected records | Metric definition, time range and filter scope |

These are alternatives. A short settings form does not need a sidebar, KPI cards or an activity feed. A chart belongs only when it changes a user's decision.

## 2. Give navigation and actions stable roles

Separate product navigation, the current work area and contextual actions. Reuse the project's business names and existing navigation model. Make the current location and object identity legible without repeating them in decorative labels.

Place frequently used actions close to the objects they affect. Distinguish the next useful action from secondary tools and destructive actions. Do not give every button equal emphasis, or impose one global primary button when several independent work areas exist.

Use tabs for meaningful views or categories, not to hide required steps or merely recolor the same content. Avoid drawers within drawers. Choose a full page when a task needs substantial space, deep linking or a durable return path; use an overlay for a bounded task whose surrounding context matters.

## 3. Set density around recognition and comparison

Determine which fields let users recognize a record and make the next decision. Keep those fields visible; reveal secondary detail where needed. Preserve units, precision, time zones and status meaning from the actual data model. Use text as well as color for consequential states.

For tables and lists:

- Align comparable values consistently. Use headers and stable columns when cross-record comparison matters; use cards when their grouping better serves the content.
- Put filters, search and sort where their scope is evident. Show active filters and provide a practical reset. Preserve context when opening and returning from a record.
- Define whether selection covers the current page or the entire filtered result. Show an accurate selected count, a clear-selection action and eligibility for each batch action.
- Decide what happens to selection after filtering, pagination or a data refresh; do not silently act on a different set of records.
- Use realistic long names, empty fields, large values and mixed statuses while reviewing the layout. Do not truncate identifiers or values needed to distinguish records without an accessible way to inspect them.
- Add pagination or virtualization when the real dataset and existing implementation warrant it. Preserve keyboard access and stable record identity; do not use array position as the identity of a changing row.

Density is not the smallest font or padding. Compare scan effort and action accuracy at realistic volume before changing spacing tokens.

## 4. Make forms and editing states explicit

Group fields by the user's decisions and dependencies. Use persistent labels, indicate required information consistently and explain unfamiliar formats beside the relevant field. A placeholder is not a label.

Keep input when validation or submission fails. Associate errors with their fields and provide a summary when errors may be out of view. On a failed submission, guide the user to a meaningful error location without moving focus on every keystroke. Keep optional guidance available without covering controls.

Distinguish editing, saving, saved and save-failed states. Do not claim autosave, draft retention, undo or conflict resolution unless the application supports it. Where unsaved changes or concurrent edits are possible, document the actual leave/reload/conflict behavior. A visual redesign must not imply a new persistence guarantee.

Use confirmation in proportion to the consequence and reversibility of the actual action. A routine reversible edit does not need the same interruption as an irreversible batch operation. Confirmation text should name the affected objects and consequence.

## 5. Cover the states the workflow can actually reach

Record a compact state/action matrix for the representative flow. Include only applicable states, but do not document only the successful populated screen:

| State | What the user needs | Available next action |
| --- | --- | --- |
| Initial loading | Stable context and an honest pending state | Wait or cancel if cancellation exists |
| No records yet | What belongs here and who can create it | A permitted first action, if one exists |
| No matching results | Which query or filters caused the result | Change or clear the relevant filters |
| Permission restriction | The available view and applicable limitation | An existing request-access path, if supported |
| Mutation pending | Which action and records are pending | Prevent duplicate submission; keep unrelated work usable |
| Failure | The operation that failed, known cause and retained input | A supported retry or correction |
| Partial batch success | Which records succeeded or failed | Inspect failures; retry only eligible failures |
| Stale or conflicting data | What changed and whether local edits remain | The product's supported refresh or resolution path |
| Success | The confirmed result and updated record state | Continue the current task without losing context |

Present server truth and local pending changes distinctly when that distinction matters. Avoid reordering or removing rows so abruptly that users lose their place. If a completed row leaves the queue, define where keyboard focus and the next action go. A toast alone is insufficient for a persistent error that needs correction.

## 6. Preserve keyboard flow and practical responsive behavior

Prefer native controls and semantic tables. An interactive spreadsheet-style grid requires its own keyboard model; do not add grid roles merely because content looks tabular. Give icon actions accessible names and expose selected, expanded, disabled and pending states appropriately.

Document focus entry, dismissal and return for overlays. Keyboard users must be able to reach row actions, filters, validation messages and batch controls. Useful shortcuts supplement visible controls; they do not replace them.

Adapt the work to supported devices. On narrow screens, preserve identifying fields and essential actions before secondary metadata. A contained, clearly usable horizontal table scroll may be preferable to unreadable miniature columns. If a complex task is desktop-only, record that real product boundary rather than inventing unsupported mobile functionality.

## 7. Decide images and motion by the work

Use thumbnails when recognizing an asset or person is part of the real task, diagrams when they explain a relevant process, and charts when they support a decision. An operational page can have a visual identity without a decorative hero. Follow the existing project design system.

Use motion to connect an action with its result, maintain orientation during a panel change or track a processed item when useful. Keep frequent actions fast, interruptible and usable with reduced motion. Immediate feedback is valid. Record a deliberate use/reuse/generate/omit decision for imagery and motion separately.

## 8. Put selected decisions in the generated Skill

Include the actual route/component/token paths, representative task flow, identifying fields, action priority, applicable state matrix, permissions and recovery behavior. Distinguish existing behavior from a proposed implementation change. Scope layout and density choices to the relevant surfaces, with reasons to revisit them.

Example for an existing approval queue: document the filter-to-detail-to-decision-to-return sequence; retain the current filters; identify the real approval permission and server responses; show record-level failures. Do not add approvals, batch endpoints or an undo promise if the product does not have them. This example is a method, not a feature specification.

Embed the selected rules and project-specific examples in the generated Skill or its own references. The next assistant should not need this generator's files or an external design system to execute them.

## 9. Verify through work, not just screenshots

When implementing UI, use representative records and supported roles. Check that:

- A user can find the correct object, inspect it, act and continue with the expected context intact.
- Sorting, filtering, pagination and selection agree about scope, including a boundary between pages if applicable.
- Loading, no records, no matches, denied actions and the actual failure paths are understandable and recoverable.
- A failed save retains input; a partial batch result does not invite duplicate successful work.
- Keyboard operation reaches the whole flow and leaves focus in a useful place after overlays and row changes.
- Supported desktop/mobile layouts handle long content and realistic density; reduced motion preserves all feedback.

Capture representative screens and exercise the interactions. A generated-rule task records these checks without claiming the application passed them.

## Reference provenance

These are synthesized workflow recommendations, not observations of a particular deployed product. Optional primary references: [Carbon data tables](https://www.carbondesignsystem.com/building-blocks/core/components/data-table/guidelines) informs table anatomy, selection and batch-action considerations; [Ant Design Form](https://ant.design/components/form/) provides examples of field dependencies, validation and error navigation. They do not prescribe this project's appearance or require installing either library.
