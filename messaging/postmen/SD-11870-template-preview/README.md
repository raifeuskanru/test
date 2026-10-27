---
layout: feature
feature_id: SD-11870
title: Template preview before editing
team: Messaging
subteam: Postmen
product_area: Email
redirect_from: [/tasks/SD-11870/]
status: Released
status_color: green
designer: Product Designer E
pm: Product Manager B
started: 2025-09-01
released: 2025-11-20
updated: 2025-11-22
updated_note: released
keywords: [preview, modal, templates, InModal]
stages:
  - { name: "0 Start", note: "Sep 1, 2025", state: done }
  - { name: "1 Pre-design", note: "Benchmark only", state: done }
  - { name: "2 Design", note: "", state: done }
  - { name: "DS Validation Gate", note: "No findings", state: done }
  - { name: "3 Handoff", note: "Oct 14, 2025", state: done }
  - { name: "4 Development and UAT", note: "Released Nov 20, 2025", state: done }
links:
  - { label: "Jira", text: "SD-11870", url: "#", note: "example" }
skipped:
  - { stage: "UX research", why: "a small change, validated with 2 partners in a call instead" }
  - { stage: "Exploration", why: "one clear option after the benchmark, no ideation round needed" }
similar: [SD-20001]
---

## What

A large preview opens when a user clicks a template, before they start editing it.

## Why

Users opened templates only to see them, then left the editor without saving (example figure: 35% of editor sessions).

## Key decisions

1. **Preview in a modal, not a new page**, so the user keeps their place in the list. [Confluence ↗](#)

## Not chosen, and why

- **Hover preview**: dropped, it does not work on touch screens.
