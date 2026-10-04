---
name: visualize-context
description: "Choose and tailor AI diagrams, flowcharts, mind maps, concept maps, decision trees, timelines, and visual comparisons to the user's question and source material. Use for visual explanations, learning, planning, relationships, and meaningful exploration. Works best alongside ChatGPT's built-in visualize skill; use static Mermaid diagrams or Markdown tables when it is disabled or unavailable. Prefer prose when clearer; route standalone apps, websites, and files to their appropriate workflow."
---

# Visualize Context

## Coordinate with the built-in visualize skill

- Treat this skill as the selection and meaning layer. It works best alongside the enabled built-in `visualize` skill in ChatGPT, which supplies inline HTML rendering, interactive behavior, theme, accessibility, runtime, and export guidance. This package does not include or install that built-in skill or its runtime.
- Resolve an enabled `visualize` skill through the current skill catalog and read its complete instructions before producing inline HTML. Do not assume a user-supplied local plugin path exists in this environment.
- Follow the renderer's output, theme, accessibility, runtime, and export contracts. Do not duplicate its instructions or silently replace its renderer. Apply the selection rules here without overriding higher-priority instructions.
- If the built-in skill is disabled, explicitly excluded, or unavailable, respect that state even if its files remain readable. Do not reopen it, re-enable it, or reconstruct its host-only runtime to bypass the user's choice. Use static Mermaid diagrams or normal Markdown tables when the current surface supports them, otherwise use concise structured prose.
- Keep automatic format selection, context tailoring, source fidelity, and readability checks active in fallback mode. Do not promise support for all 20 formats on every surface; substitute a faithful supported representation when necessary. This skill's fallback mode does not provide inline HTML controls, live simulations, or the built-in export workflow.
- If interaction is essential to the request, explain briefly that the built-in skill must be enabled and available for this skill's inline interactive workflow. Provide the useful static portion when possible. Use a separate standalone artifact workflow only when the user requests or authorizes that deliverable.
- Explain the active mode only when it affects the requested result; do not repeat availability warnings on every response. Never claim an interactive visual was rendered without a supported enabled renderer.
- Route standalone document, image, presentation, website, and application deliverables to the appropriate artifact or project workflow; apply these selection principles there without imposing the inline HTML contract.
- Do not create a visual for every response. Treat invocation as a request to assess the most useful presentation; honor an explicit visual request whenever a faithful supported visual is possible.

## Select automatically

1. Identify the question the user needs answered: understand, compare, choose, plan, explain, or explore a change.
2. Identify the dominant relationship: sequence, branching, association, hierarchy, containment, overlap, feedback, chronology, experience, or quantified flow. Distinguish the desired insight from keywords in the prompt.
3. Check the available evidence, units, dates, constraints, audience knowledge, and relevant stated preferences. Use the current request and relevant available context; retrieve only material needed for this task. Never infer unrelated preferences, diagnoses, emotions, or personal history.
4. Read [Format selection and tailoring](references/formats.md). Choose the simplest format that exposes the relationship accurately. Prefer one coherent visual. Add a second only when it answers a distinct necessary question.
5. Honor an explicitly requested format when it fits. If it would imply unsupported structure or quantities, briefly explain the issue and use a faithful version or a better format. Do not manufacture missing data to satisfy the format.
6. Choose prose for a simple fact or linear explanation; choose a normal Markdown table for exact comparisons and mappings that are clearest as rows and columns. Do not build an interactive fragment merely to reproduce a table.

Make these choices without asking the user to select a diagram. Ask only when a missing fact materially changes the meaning or an important decision. Otherwise proceed using a conservative, clearly identified assumption where necessary. Do not narrate the internal selection process; briefly explain how to read the result only when helpful.

## Tailor to the context

- Use the user's actual terms, supplied examples, goals, options, and constraints. Match technical depth to the task and known background; use plain labels without removing important qualifications.
- For supplied study material, derive relationships from that material and respect source restrictions. Label a paraphrase, inferred connection, or illustrative example when the distinction matters.
- For spiritual or philosophical material, attribute its claims to the source. Preserve distinctions between a described belief, metaphor, personal experience, and established fact. Do not turn a spiritual analogy into an asserted physical mechanism.
- For personal inquiry, show only feelings and beliefs the user has stated. Present possible connections as possibilities, not diagnoses or confirmed causes. Avoid implying that personal experience must follow a fixed sequence.
- For decisions, reflect the user's criteria and tradeoffs. Do not invent rankings, probabilities, or recommendations from missing preferences.
- For plans, distinguish known commitments from proposed steps and estimated dates or durations. Include dependencies only when supported or explicitly proposed.
- For numerical visuals, preserve values, units, scale, totals, denominators, and uncertainty. Distinguish missing values from zero. Do not convert qualitative ideas into invented percentages or scores.

## Preserve meaning in the structure

- Give every arrow a specific meaning. Distinguish happens-next, influences, communicates-with, contains, and depends-on. Label ambiguous edges or provide one compact legend for repeated meanings.
- Use directional arrows only for a supported direction. Use undirected links for association. Use a cycle only when recurrence exists; use feedback only when an effect influences an earlier part of the process.
- Treat branching conditions, sequence, authority, containment, and importance as different structures. Never imply inevitability or value from position alone.
- Preserve exceptions, alternative paths, uncertainty, and relevant cross-connections. Do not simplify a qualified source claim into a universal one.
- Represent multiple relationship types clearly. Prefer labeled concept-map edges or a small second view over forcing every relationship into a flowchart.

## Adapt complexity and interaction

- Start with the smallest readable overview that answers the question. Group related details while keeping essential distinctions, comparisons, and outcomes visible together.
- For long sources, summarize faithfully; show supporting detail on selection or expansion only when the question benefits from exploration. Make omitted or grouped structure clear. Do not conceal an exception that changes the conclusion.
- Use a meaningful interaction only when explicitly requested or intrinsically required by the user's exploration request. Selecting a concept may highlight its connections; a requested step-through may advance a process. Keep ordinary explanation visuals static by default.
- Treat a request to explore how a supplied parameter changes an outcome as authorization for the minimum necessary parameter control. Use sliders only for meaningful ordered numerical quantities and a supported model; label illustrative models. Do not add search, reset, toggles, scores, animation, or toolbars as decoration.
- Keep the initial view useful and essential labels visible without hover. Preserve stable node identities and category meanings across states; ensure every interaction changes the intended visual content.
- Adapt orientation, wrapping, grouping, and panel stacking to actual width. On small screens reflow instead of shrinking labels. Avoid long horizontal chains and more than five main nodes across a Mermaid diagram.
- Keep meaning accessible without color, pointer hover, dragging, or animation. Use native accessible controls and the renderer's keyboard and touch guidance. Respect reduced motion and avoid autonomous looping animation.

## Verify before presenting

- Verify that the chosen format answers the user's question and that all requested dimensions are represented.
- Check every node, edge, condition, date, value, unit, and caption against the supplied evidence. Check totals where appropriate; identify assumptions and illustrative content.
- Check that layout does not imply unsupported causation, order, rank, proportionality, or certainty.
- For rendered visuals, inspect narrow and normal widths, light and dark themes where supported, longest labels, alternative paths, and essential touch or keyboard access. Repair overlap, clipping, misleading edge placement, and unreadable text.
- Exercise the primary interaction and a materially different state. Confirm that labels, connections, quantities, and accessible state change consistently. Use the renderer's preview guidance when producing inline HTML; do not claim a visual check that was not performed.
- Present the visual using the renderer's response contract and only the concise explanation needed to interpret it. Do not repeat its contents in prose.
