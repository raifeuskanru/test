# Flow map

> Output of the flow-map skill, Jun 13, 2026. Example data.

```mermaid
flowchart LR
  A[Open Template Store] --> B{Knows the channel?}
  B -->|Yes| C[Pick a channel chip]
  B -->|No| D[Type in search]
  C --> E[Pick a use-case chip]
  D --> F{Results?}
  E --> F
  F -->|Yes| G[Open a template]
  F -->|No| H[Empty state]
  H --> I[Clear filters]
  I --> F
```

## Steps that changed compared to today

| Step | Today | New |
|---|---|---|
| Find by channel | Scroll and read tags on every card | One chip |
| No results | Blank grid | Empty state with a way out |
