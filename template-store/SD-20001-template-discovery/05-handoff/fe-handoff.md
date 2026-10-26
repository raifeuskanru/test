# Developer handoff

> Written with `designer-fe-handoff` on Aug 4, 2026 for `template-store-fe`. Updated on Aug 21. Example data.

## What to build

The filter and search behaviour described in [the spec](../04-design/spec.md), on the existing Template Store page.

## Behaviour

1. Channel chips: Email, SMS, Web push, WhatsApp. Multi-select.
2. Use-case chips: Welcome, Abandoned cart, Win-back, Promotion. Multi-select.
3. Search filters by name and tags while typing, after 2 characters.
4. Empty state appears when the result count is 0. "Clear filters" resets chips and search.
5. Under 768 px the two chip groups move into one "Filters" dropdown. *(Added Aug 21.)*

## DS approval field

| Exception | Approval |
|---|---|
| `InCard` thumbnail 4:3 instead of 16:9 | Approved in #ds-helpline on Jul 30 ([thread](#)) |

## Prototype

The clickable prototype archived at handoff: [artifacts/prototype](../artifacts/prototype/).
