# Naming and hierarchy

> Demo. Team and subteam names in this demo are examples.

## The hierarchy

```
<team>/
  <subteam>/
    <JIRA-KEY>-<short-name>/      one folder per task
```

Example: `scalability/skeletors/SD-20001-template-discovery/`

Every task has exactly one place. Three levels, always.

## Rules per level

| Level | Folder name | Where the name comes from |
|---|---|---|
| Team | lowercase, words joined with `-` (`scalability`) | The official team name in the company directory. Claude never invents one. |
| Subteam | lowercase, words joined with `-` (`skeletors`) | The official subteam name. A team without subteams uses `general`. |
| Task | `<JIRA-KEY>-<short-name>` (`SD-20001-template-discovery`) | The Jira key keeps its uppercase form. The short name is lowercase, words joined with `-`, no spaces, no Turkish characters. |

## What is not a folder

- **Designer.** Written in the ID card (`designer:`). The showcase filters by designer. A task can change hands, or have two designers, without moving.
- **Product area.** Written in the ID card (`product_area:`), searchable and shown on the task page.
- **Status.** Written in the ID card. The showcase groups and colours by it.

## When teams change

- Claude moves the task folder with `git mv`, so its history stays.
- The ID card's `team`, `subteam` and `permalink` change with it. `permalink` is always the folder path, so the task page address and the short link stay correct.
- The short link `/tasks/<JIRA-KEY>/` keeps working, because every ID card has `redirect_from: [/tasks/<JIRA-KEY>/]`. Share that link in Jira and Confluence, not the long one.

## Files

- Files written by design skills keep the date the skill gives them (`pvd-analysis-2026-06-03.md`). Do not rename them.
- Files the library owns have no version or date in the name (`spec.md`, `history.md`). Git keeps every version.
- Commit messages start with the Jira key: `SD-20001 | save: pre-design outputs`.
