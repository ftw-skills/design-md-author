---
name: design-md-author
description: Find, write, or update a UI DESIGN.md. Use for design-system references, extracting visual rules from an existing frontend, or authoring a specification from a brief, screenshots, or examples.
---

# Author DESIGN.md

Produce a portable design specification with machine-readable YAML tokens and Markdown instructions for applying them. Use [format and verification](references/format.md) for every document you write or update.

## Choose the workflow

- **Find examples.** Open the original files using [sources and comparison](references/sources.md). Report useful token and prose examples with source links. Write a project document only when requested.
- **Extract a work's style.** When frontend source is available, use Google Labs' `stitch::extract-design-md` for source discovery and extraction. Follow [frontend extraction](references/extraction.md) to use its findings, reconcile conflicts, and write the final document. For a screenshot or a visible page alone, use the reference workflow and identify what is inferred.
- **Write from a brief or references.** Identify the intended audience, surfaces, and visual priorities. Use reference prose as evidence for specific layout, hierarchy, and interaction rules, then adapt the rules to the target product. Apply the user's approved direction and constraints.

## Resolve conflicts

Follow the user's explicit source priority. For documenting current behavior, use the implementation as evidence of what ships and record divergences from existing design guidance. For a redesign, use the approved brief for the target and label intentional changes. For an update, preserve unrelated rules and explain overlaps or contradictions that affect the result. Mark unresolved choices and distinguish observed behavior from proposed rules.

## Deliver

- Use the requested path. Otherwise update the relevant existing `DESIGN.md` or write it in the frontend root. For a document without a project, use the task's deliverable directory.
- Check the token structure, the actionable coverage of the prose, and agreement between both. If an implementation or preview is in scope, trace its key rules to visible elements, states, or viewport behavior.
- Report the file, the material sources, and checks performed. Use [worked examples](references/worked-examples.md) when you need a concrete reference for prose or source reconciliation.