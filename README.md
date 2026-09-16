# Mortise

A component workbench for product design teams — mock SaaS app, single HTML file,
no build step, no dependencies.

Open `index.html` in a browser.

## What it does

Mortise is where a design system team keeps the components every product ships.
Pick a component from the rail, drive its properties from the inspector, and see
the change on the stage and across the whole variant matrix at once.

- **Stage** — the live component, on a light or dark product surface that is
  independent of the app's own theme.
- **Variant matrix** — every combination of two axes (tone × size, state × size,
  …). Click a cell to make it the live configuration.
- **Inspector** — properties, token overrides (corner, padding, label size,
  weight), the resolved design tokens, adoption over the last 12 months, and the
  activity thread.
- **Library health** — how many components are stable, and how many instances
  across products have drifted off-token.

Eight components ship in the mock library: Button, Segmented control, Text
field, Switch, Toast, Badge, Avatar stack and Usage meter.

## Keyboard

| Key | Action |
| --- | --- |
| `/` | Focus search |
| `↑` `↓` | Move through the component rail |
| `Enter` / `Space` | Apply the focused matrix cell |
| `Esc` | Leave search |

## Design notes

Chrome stays quiet so the components carry the color. Neutrals are biased toward
the verdigris accent rather than pure grey; semantic color (good / warning /
critical) is kept separate from the accent so status reads at a glance. Georgia
sets the wordmark and the large figures, a monospace face carries labels and
metrics, and the UI runs on the system sans.

Both app themes are supported, and the preview surface toggles independently —
the point of a workbench is to check a component against the surface it will
actually ship on.

## Data

All content is fictional: the Northbeam design system, its components, adoption
numbers and activity threads are mock data defined in `LIB` inside `index.html`.
