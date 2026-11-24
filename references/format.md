# Format and verification

Follow the [Google Labs specification](https://github.com/google-labs-code/design.md/blob/main/docs/spec.md). Prefer a single YAML front-matter block for new files. Preserve supported interleaved YAML when updating a document that already uses it.

## Tokens

Use meaningful roles for colors, typography, spacing, shape, and components as applicable. Use structured typography fields, dimension units, and quoted references such as `"{colors.primary}"`. Confirm every reference resolves and each top-level key and body heading is unique. Represent concrete, reusable values that can be verified against the source or are part of the proposed design.

## Prose

Use level-two headings for the main topics and level-three headings for variants or component families when they help navigation. Cover the design direction, color roles, type hierarchy, layout and spacing, shapes, elevation, and components where applicable. Explain a rule's use and scope. When conditions matter, state when it changes or what exception applies.

For example, a button token can define teal and an 8px radius. The prose can specify that the filled button goes on the main action, secondary actions stay outlined, and keyboard focus uses a visible ring. Document relevant responsive changes, states, usage restrictions, and do/don't rules. Keep unknown details marked and leave unrelated sections out.

## Acceptance

1. Run the project's documented validator when present. Otherwise use the official linter when available. Check syntax and token references, address applicable errors, and report the actual result.
2. Verify that key prose rules are actionable and consistent with the tokens. For an extraction, check representative values and behaviors against source declarations or verified rendering. For a reference-driven design, identify the specific borrowed rules and document meaningful adaptations. Surface disagreements instead of silently resolving them.
3. If a preview or implementation is in scope, verify representative rules from the prose as well as token values. Where relevant, inspect a viewport change or exercise a state. Record the rule, where it is implemented, evidence of the result, and any meaningful omission. If the deliverable is only a document, check whether its rules are specific enough to implement.

```powershell
npx -p '@google/design.md' designmd lint DESIGN.md
```

This PowerShell command uses the official dot-free alias and may fetch the package. If the validator is unavailable, do a local review and report the checks performed.