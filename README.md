# Design Library (demo)

> **Demo with example data.** Not a real Insider project. Built to show how the AI-era Design Library and Handoff could work.

**Read it here:** [raifeuskanru.github.io/test](https://raifeuskanru.github.io/test/). That site is the showcase. It is built automatically from the files in this repository.

## What this repository is

Every design task has one folder, named after its Jira key. Everything produced for the task goes into that folder: research, benchmarks, flow maps, ideas, the spec, the developer handoff, the clickable prototype, screens, what was not chosen and why, and the history of changes.

Designers do not open this repository to work. Claude saves the files after the designer approves. People read the showcase, not these folders.

## Folder structure

```
<product-area>/
  <JIRA-KEY>-<short-name>/
    README.md          ID card and the "understand in 5 minutes" summary
    01-intake/         PVD analysis, dependency scan
    02-research/       benchmark summary, UX research plan and findings
    03-exploration/    flow map, ideation summary
    04-design/         spec, DS Validation Gate reports
    05-handoff/        developer handoff, UAT report
    artifacts/         HTML outputs: prototype, ideation, benchmark (clickable on the showcase)
    screens/           screenshots saved at handoff
    not-chosen.md      dropped alternatives and postponed decisions, with reasons
    history.md         every change, with the date and the reason
    links.md           things outside the library, each with a one-line summary
```

## What is in this demo

| Task | Product area | Status | Shows |
|---|---|---|---|
| [SD-20001 Easier template discovery](template-store/SD-20001-template-discovery/) | Template Store | Released | A complete task from start to release |
| [SD-12345 Bulk edit for journey templates](journey/SD-12345-bulk-edit-templates/) | Journey | In pre-design | A task in progress |
| [SD-11870 Template preview](email/SD-11870-template-preview/) | Email | Released | An older task, found through "similar work" |

## Rules and templates

- [_rules/](_rules/): what goes where, naming, what never goes in
- [_templates/](_templates/): the ID card, not-chosen and handoff skeletons Claude starts from
- [_layouts/](_layouts/) and [assets/](assets/): how the showcase looks. Owned by the library owners.
