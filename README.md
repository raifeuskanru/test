# Design Library (demo)

> **Demo with example data.** Not a real Insider project. Built to show how the AI-era Design Library and Handoff could work.

**Read it here:** [raifeuskanru.github.io/test](https://raifeuskanru.github.io/test/). That site is the showcase. It is built automatically from the files in this repository.

## What this repository is

The library is organised in three levels: **team, then subteam, then task**. Every design task has one folder, named after its Jira key. Everything produced for the task goes into that folder: research, benchmarks, flow maps, ideas, the spec, the developer handoff, the clickable prototype, screens, what was not chosen and why, and the history of changes.

Designers do not open this repository to work. Claude saves the files after the designer approves. People read the showcase, not these folders.

## Folder structure

```
<team>/                          e.g. scalability/
  <subteam>/                     e.g. skeletors/
    <JIRA-KEY>-<short-name>/     e.g. SD-20001-template-discovery/
      README.md        ID card (team, subteam, designer, status) and the "understand in 5 minutes" summary
      01-intake/       PVD analysis, dependency scan
      02-research/     benchmark summary, UX research plan and findings
      03-exploration/  flow map, ideation summary
      04-design/       spec, DS Validation Gate reports
      05-handoff/      developer handoff, UAT report
      artifacts/       HTML outputs: prototype, ideation, benchmark (clickable on the showcase)
      screens/         screenshots saved at handoff
      not-chosen.md    dropped alternatives and postponed decisions, with reasons
      history.md       every change, with the date and the reason
      links.md         things outside the library, each with a one-line summary
```

The designer is not a folder level: it is written in the ID card, and the showcase filters by it. Every task also has a short link, `/tasks/<JIRA-KEY>/`, that keeps working when teams change and folders move. Full rules: [_rules/naming.md](_rules/naming.md).

## What is in this demo

Team and subteam names are examples.

| Task | Team / Subteam | Product area | Status | Shows |
|---|---|---|---|---|
| [SD-20001 Easier template discovery](scalability/skeletors/SD-20001-template-discovery/) | Scalability / Skeletors | Template Store | Released | A complete task from start to release |
| [SD-12345 Bulk edit for journey templates](scalability/pathfinders/SD-12345-bulk-edit-templates/) | Scalability / Pathfinders | Journey | In pre-design | A task in progress |
| [SD-11870 Template preview](messaging/postmen/SD-11870-template-preview/) | Messaging / Postmen | Email | Released | An older task, found through "similar work" |

## Rules and templates

- [_rules/](_rules/): what goes where, naming, what never goes in
- [_templates/](_templates/): the ID card, not-chosen and handoff skeletons Claude starts from
- [_layouts/](_layouts/) and [assets/](assets/): how the showcase looks. Owned by the library owners.
