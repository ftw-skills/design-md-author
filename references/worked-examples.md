# Worked examples

## Author a specification

[Waypoint DESIGN.md](../examples/waypoint/DESIGN.md) is a complete portable example. Its body explains why one action is filled, when the two-column layout changes, and how links display keyboard focus. [Google Labs' Totality Festival](https://github.com/google-labs-code/design.md/blob/main/examples/totality-festival/DESIGN.md) is a separate upstream example with deeper component and visual guidance.

## Extract from source

Use the same small frontend as an extraction exercise. Inspect [index.html](../examples/waypoint/index.html) for content and component roles and [styles.css](../examples/waypoint/styles.css) for implemented choices. Run the extraction from the source files alone and compare the result with [the reference document](../examples/waypoint/DESIGN.md).

| Rule | Where to verify |
| --- | --- |
| One filled primary action and an outlined secondary action | The two links in the hero and their modifier classes |
| Two field-note columns on wide screens, one column at 680px and below | The grid and its media query |
| Visible keyboard focus on both action links | The shared `:focus-visible` declaration |
| Muted supporting text stays on the paper surface | Text placement and color in the hero and footer |