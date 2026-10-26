# What goes where

> Rules Claude follows when saving a task. Demo.

## Everything produced for the task goes in

| Output | Folder |
|---|---|
| PVD analysis, process analysis, dependency scan | `01-intake/` |
| Benchmark summary, UX research plan, findings summary, UX metrics | `02-research/` |
| Brief, flow map, ideation summary | `03-exploration/` |
| Spec, DS Validation Gate reports | `04-design/` |
| Developer handoff, UAT reports | `05-handoff/` |
| HTML outputs: prototype (at handoff), ideation, benchmark, HTML briefs | `artifacts/<name>/index.html` |
| Screenshots of every screen and state, saved at handoff | `screens/` |
| Dropped alternatives and postponed decisions, with reasons | `not-chosen.md` |
| Every change, with date and reason | `history.md` |
| Anything outside the library, each with a one-line summary | `links.md` |

Every HTML output also gets a short Markdown summary, so search can find it.

## Never goes in

- Personal scratch notes (they stay on the designer's laptop)
- Raw interview notes and recordings (restricted Drive folder, linked in `links.md`)
- Partner or customer data
- Passwords, tokens, keys
