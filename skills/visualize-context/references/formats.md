# Format selection and tailoring

## Contents

- Selection priority
- Format rules
- Context examples
- Misleading matches to avoid

## Selection priority

Select from the relationship needed to answer the question, not the topic's vocabulary. Prefer an explicitly requested faithful format. Otherwise prefer the smallest readable representation with the fewest unsupported implications. Use these rules as guidance, not a rigid classifier. Keep unrelated concepts out merely because they appear elsewhere in context.

Use a flowchart for process logic, a concept map for labeled conceptual relationships, and a system diagram for interacting parts. Use a decision tree only when choices or conditions create real branches. Prefer a table when exact comparison matters more than spatial structure. Use interactive rendering only when exploration benefits from it; otherwise use the supported static representation.

## Format rules

| Format | Select for | Tailor to the material | Protect meaning |
|---|---|---|---|
| Flowchart | A procedure, action sequence, or process with branches | Use short action labels, clear entry and exit points, conditions on branches, and relevant alternatives | Distinguish sequence from cause; do not force a network into a linear chain |
| Mind map | Brainstorming or exploring themes around a topic | Center the actual topic; organize branches into meaningful, clearly named themes | Do not imply causal direction, chronology, or ranking from branch position |
| Concept map | Explaining how ideas relate | Use source terms and labeled edges such as includes, depends on, or influences; retain relevant cross-links | Qualify inferred connections; avoid unlabeled generic arrows |
| Decision tree | Choosing actions under branching conditions | Use actual options, constraints, and questions; label uncertain outcomes | Do not fabricate options, likelihoods, exhaustive branches, or guaranteed results |
| Relationship map | Associations among people, ideas, or entities | Group relevant entities; distinguish connection types; direct links only when needed | Avoid unsupported social, emotional, or causal inferences |
| System diagram | Parts, boundaries, inputs, outputs, and exchanges | Include only parts necessary to the question; label exchanges and boundaries | Distinguish information, material, and conceptual relationships; avoid invented mechanisms |
| Cycle diagram | A process that returns to an earlier stage | Show the return path and relevant variations; use stage labels from the material | Do not imply a mandatory start, rigid timing, or inevitable recurrence |
| Feedback loop | An effect changes an earlier influence | Label each influence and whether it increases, decreases, or otherwise changes the next element; include known delays | Verify the returning influence; a repeating sequence alone is not feedback |
| Cause-and-effect diagram | Examining contributors to an outcome | Group factors by relevant themes and separate supported causes from hypotheses | Label possibilities; do not present association as established cause |
| Sequence diagram | Ordered actions among participants | Use participant lanes and actual messages or actions in order | Use temporal order, not guessed durations; include meaningful alternative paths |
| Timeline | Chronology, development, or milestones | Use verified dates and required time granularity; mark approximate dates | Distinguish chronology from cause; use proportional spacing only with a real time scale |
| Hierarchy diagram | Categories, containment, reporting, or levels | Name the parent-child relationship; retain meaningful levels and exceptions | Distinguish classification, authority, developmental level, and importance |
| Venn diagram | Shared and distinct membership or features of a few sets | Put supported common items in overlaps and distinctive items outside them | Use schematic areas unless sizes are calculated from data; use a table or membership grid for many sets |
| Comparison matrix | Options compared against common criteria | Use user-relevant criteria, consistent units and language, and exact available values | Mark unknowns; do not invent ratings, weights, or a winner |
| Quadrant chart | Organizing items by two meaningful dimensions | Name axes and direction; use actual values or label placements as qualitative | Do not imply measured distances, exact scores, or rankings from subjective positions |
| Journey map | An experience unfolding through stages | Show relevant actions, stated feelings, obstacles, and opportunities; preserve possible paths | Do not invent emotions or treat every experience as identical |
| Storyboard | Explaining an idea through a concrete scenario | Maintain the same scenario or characters; show only scenes needed to explain the change | Label invented scenes as illustrative; avoid presenting them as real events |
| Gantt chart | Tasks with timing, overlap, and dependencies | Use actual deadlines and durations; label proposed estimates; align tasks on a common time axis | Do not imply commitment to estimated dates; distinguish tasks, milestones, and dependencies |
| Sankey diagram | Quantified flows among categories or stages | Make widths proportional to supplied values; use consistent units; show important losses, sources, or sinks | Do not invent quantities; reconcile flows when conservation applies; label accounting differences |
| Funnel diagram | Items progressing through stages that narrow | State qualification or transition at each stage; include actual counts or clearly schematic stages | Use proportional widths only with counts; do not force a non-narrowing process into a funnel |

## Context examples

- For a chapter describing relationships among faith, intention, and action, derive a concept map from its stated relationships. Attribute claims to the chapter; do not add causal links from outside teachings.
- For a user describing a possible belief-feeling-action cycle, show feedback only if the account includes a returning influence. Otherwise show a labeled relationship map; qualify interpretations.
- For a music project asking what to do next, show a flowchart of supported production steps. For the same project asking how sessions overlap before a deadline, use a Gantt chart with labeled estimates.
- For comparing creative projects against time, cost, and enjoyment, use a matrix with stated values and unknowns. For enjoyment-versus-effort positioning, use a qualitative quadrant with user-supplied placements or clearly proposed estimates.
- For exploring how a supplied input changes an outcome, use a compact simulation only with a supported relationship or explicitly illustrative model. Include the minimum necessary control; avoid invented precision.
- For explaining who sends what during an app request, use a sequence diagram. For the components of the same app, use a system diagram.

## Misleading matches to avoid

- Do not choose a timeline merely because a passage includes dates when the question asks how concepts connect.
- Do not draw feedback merely because the prompt contains the word cycle; verify a returning influence.
- Do not choose a hierarchy merely because some concepts sound more advanced or spiritually important.
- Do not invent numerical scores to fill a quadrant, matrix, Sankey, funnel, or simulator.
- Do not use geographic maps for metaphorical journeys; use a journey map or concept map.
- Do not use proportional bars, widths, areas, distances, or time spacing without corresponding data or a clearly identified schematic interpretation.
- Do not hide required comparison dimensions behind switches or replace a simple exact table with an elaborate interactive interface.
