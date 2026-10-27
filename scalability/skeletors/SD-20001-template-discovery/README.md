---
layout: feature
feature_id: SD-20001
title: Easier template discovery in Template Store
team: Scalability
subteam: Skeletors
product_area: Template Store
permalink: /scalability/skeletors/SD-20001-template-discovery/
redirect_from: [/tasks/SD-20001/]
status: Released
status_color: green
designer: Product Designer A
pm: Product Manager B
started: 2026-06-02
released: 2026-09-10
updated: 2026-09-12
updated_note: ID card updated after release
keywords: [filters, search, empty state, chips, cards, InChip, InCard, discovery]
stages:
  - { name: "0 Start", note: "Jun 2", state: done }
  - { name: "1 Pre-design", note: "Research, flow map, 3 ideas", state: done }
  - { name: "2 Design", note: "Built on template-store-fe", state: done }
  - { name: "DS Validation Gate", note: "1 exception approved", state: done }
  - { name: "3 Handoff", note: "Aug 4", state: done }
  - { name: "4 Development and UAT", note: "Released Sep 10", state: done }
prototype: artifacts/prototype/
artifacts:
  - { label: "Ideation: 3 options", path: "artifacts/ideation/" }
  - { label: "Benchmark page", path: "artifacts/benchmark/" }
links:
  - { label: "Jira", text: "SD-20001", url: "#", note: "example" }
  - { label: "Decision page", text: "Confluence · Template Store · SD-20001", url: "#", note: "example" }
  - { label: "Built on", text: "template-store-fe · design/SD-20001 · 7c1e2ab", url: "#", note: "example" }
  - { label: "Live review", text: "Zoe prototype", url: "#", note: "deleted after a year, the archive is below" }
  - { label: "Interview recordings", text: "Drive, restricted", url: "#", note: "may contain partner data" }
skipped:
  - { stage: "UX metrics", why: "the PM already tracks Template Store usage on an existing dashboard" }
similar: [SD-11870, SD-12345]
---

## What

Partners can filter Template Store by channel and use case, search by template name, and see a clear empty state when nothing matches. Before this, they scrolled through more than 300 templates.

## Why

- 3 of 5 interviewed partner users scrolled the whole grid before they used search ([finding 2](02-research/ux-findings.md)).
- 41% of Template Store sessions ended without a template being opened (example figure).
- Support received 18 "where is the X template?" tickets last quarter (example figure).

## Key decisions

1. **Filters are horizontal chips above the grid**, so the grid keeps its full width. Decided on Jun 16 with the PM. [Confluence ↗](#)
2. **Search matches the template name and tags, not the content**, because content search returned too many weak matches in the test. [Confluence ↗](#)
3. **Card thumbnails stay 4:3**, which is outside the DS card rule. Approved as a DS exception in #ds-helpline. [Thread ↗](#)

## Not chosen, and why

- **Left sidebar with filters**: dropped. It took a third of the screen on 13-inch laptops, where most partners work.
- **"Recommended for you" row**: postponed. There is no usage data per partner yet.

Details: [not-chosen.md](not-chosen.md)

## What changed after handoff

- On screens narrower than 768 px the chips became a single dropdown. The developer found the chips wrapped to three lines. The PM agreed on Aug 21. See [history.md](history.md).

## Open follow-ups

- Add tracking for "filter used, then template opened" to measure the effect. Owner: PM.
