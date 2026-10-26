---
layout: feature
feature_id: SD-00000
title: Short title of the task
product_area: Product area
status: Started            # Started | In pre-design | In design | Handed off | In development | Released
status_color: yellow       # yellow | green | gray
designer: Name
pm: Name
started: YYYY-MM-DD
released:
updated: YYYY-MM-DD
updated_note: what changed last
keywords: []               # components, topics: used by search
stages:
  - { name: "0 Start", note: "", state: now }   # done | now | todo | skip
  - { name: "1 Pre-design", note: "", state: todo }
  - { name: "2 Design", note: "", state: todo }
  - { name: "DS Validation Gate", note: "", state: todo }
  - { name: "3 Handoff", note: "", state: todo }
  - { name: "4 Development and UAT", note: "", state: todo }
prototype:                 # artifacts/prototype/ after handoff
artifacts: []              # - { label: "...", path: "artifacts/<name>/" }
links: []                  # - { label: "...", text: "...", url: "...", note: "..." }
skipped: []                # - { stage: "...", why: "..." }
similar: []                # Jira keys of similar tasks
depends_on: []             # components, decisions, Jira keys: used to find what a change affects
---

## What

## Why

## Key decisions

## Not chosen, and why

## What changed after handoff

## Open follow-ups
