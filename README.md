# Design MD Author

An agent skill for creating and updating `DESIGN.md` specifications for user interfaces. It combines machine-readable YAML design tokens with Markdown guidance on using them.

## Quick start

1. Add this repository as a skill in your agent's skill manager, or point your agent to [SKILL.md](SKILL.md).
2. Supply the frontend source, screenshots, approved brief, or reference docs. Identify which source takes priority if they disagree.
3. Ask the agent to update an existing specification or name the path for a new one.

```text
Use $design-md-author to document our current frontend in DESIGN.md. Extract
the tokens from the source and record any differences between the shipped
screens and the existing design rules.
```

- [Format and verification](references/format.md) covers token syntax, references, and acceptance.
- [Frontend extraction](references/extraction.md) covers source inspection and normalization.
- [Worked examples](references/worked-examples.md) show how to reconcile sources and write actionable rules. See the [Waypoint specification](examples/waypoint/DESIGN.md) for a concrete example.

For changes to the skill, keep the guidance and worked examples in agreement. Recheck the documented token references and the rendered UI where applicable.
