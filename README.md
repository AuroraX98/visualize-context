# Visualize Context

A ChatGPT skill that turns explanations and supplied material into clear, context-aware visuals. It chooses the simplest useful format, labels relationships accurately, and keeps the result readable rather than adding diagrams for decoration.

## ChatGPT and the built-in visualize skill

**The intended interactive experience is in ChatGPT, with its built-in `visualize` skill enabled and available.** Visualize Context decides what to show and how to explain it; the built-in skill provides inline rendering, interaction, accessibility, theme, and export support. This repository does **not** include or install that renderer. It cannot add Intelligent UI capabilities to a chat surface that does not support them.

Without that renderer, the skill can fall back to supported static Mermaid diagrams, Markdown tables, or concise prose. Those instruction-based fallbacks may also be useful elsewhere, but the inline interactive workflow described here is ChatGPT-specific. Availability varies by surface; not every format renders everywhere.

## What it does

- Selects a visual based on the question, not just topic keywords.
- Uses your supplied terms, examples, sources, and constraints.
- Preserves uncertainty and avoids invented numbers or misleading arrows.
- Keeps explanations small and focused, especially for learning.
- Adds interaction only when exploring a change genuinely needs it.
- Uses clear labels and layouts whose meaning does not depend on color alone.

## Visual formats

The format guide covers all 22 of these forms. They are selection and design instructions, not 22 bundled renderers.

| Format | Useful for |
| --- | --- |
| Flowchart | Steps, procedures, and process branches |
| Mind map | Brainstorming themes around a topic |
| Concept map | Labeled relationships between ideas |
| Decision tree | Choices under branching conditions |
| Relationship map | Associations among people, ideas, or entities |
| System diagram | Parts, boundaries, inputs, and outputs |
| Cycle diagram | Processes that repeat |
| Feedback loop | Effects that influence an earlier part of a process |
| Cause-and-effect diagram | Supported causes and possible contributing factors |
| Sequence diagram | Ordered interactions among participants |
| Timeline | Events, development, and milestones |
| Hierarchy diagram | Categories, containment, and levels |
| Venn diagram | Shared and distinct set membership |
| Comparison matrix | Options evaluated against common criteria |
| Quadrant chart | Two meaningful dimensions |
| Journey map | An experience across stages |
| Storyboard | An explanation through a concrete scenario |
| Gantt chart | Task timing, overlap, and dependencies |
| Sankey diagram | Quantified flows |
| Syntax anatomy diagram / labeled code breakdown | What each part of a short code line means |
| Annotated equation/expression | What mathematical symbols, terms, and groups mean |
| Funnel diagram | Items moving through narrowing stages |

When requested and supported, a small simulation or parameter control can help explore how a supplied input changes an outcome. It must use a supported relationship or be clearly labeled illustrative.

## Example requests

- “Use Visualize Context to show how these ideas connect. Use only this chapter.”
- “Show a labeled breakdown of `print("Hello")`, one small idea at a time.”
- “Annotate `3 × 4 = 12` so I can see what each part means.”
- “Show the prediction → loss → weight-update loop in a tiny neural network.”
- “Compare these options using my criteria. Mark anything unknown.”

A labeled code breakdown keeps one line visible and identifies its parts with short labels and leader lines. For `print("Hello")`, it distinguishes the function name, parentheses, and string argument. The quotation marks delimit the string; they are not part of the displayed output.

## Use the skill

Add the [SKILL.md](SKILL.md) and [references/formats.md](references/formats.md) together through the skill import workflow available in your ChatGPT account, preserving their relative paths. Then ask ChatGPT to use Visualize Context with your material. For inline interactive visuals, also make sure the built-in `visualize` skill is enabled and available. This package does not enable it for you.

If your interface does not provide skill import or inline rendering, the files remain readable guidance, not an executable app or a replacement runtime.

## Files

- [SKILL.md](SKILL.md): selection, source fidelity, accessibility, and verification rules.
- [references/formats.md](references/formats.md): format-by-format guidance and code/math anatomy examples.

No API key, backend, or additional package is included. Standalone images, documents, websites, and apps use their own authorized creation workflows.
