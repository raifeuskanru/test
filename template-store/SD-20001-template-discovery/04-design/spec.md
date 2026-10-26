# Design spec

> Written with `/design-directive` on Jul 22, 2026, updated on Aug 21 after the mobile change. Example data.

## Screens and states

| Screen | State | What the user sees |
|---|---|---|
| Template Store | Default | Search field, channel chips, use-case chips, grid of cards |
| Template Store | Filtered | Selected chips highlighted, result count, matching cards |
| Template Store | Empty | Message "No templates match these filters" and a "Clear filters" button |
| Template Store | Narrow screen (under 768 px) | Chips replaced by one "Filters" dropdown (changed Aug 21) |

## Design System components

| Component | Use | Note |
|---|---|---|
| `InChip` | Channel and use-case filters | Standard |
| `InSearch` | Search field | Standard |
| `InCard` | Template card | Thumbnail ratio 4:3, DS exception approved |
| `InEmptyState` | No results | Standard |

## Rules

- Chips within one group combine with OR, groups combine with AND.
- The result count updates on every change.
- Search matches the template name and tags only.
