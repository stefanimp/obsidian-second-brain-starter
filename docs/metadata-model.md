# Metadata Model

The metadata model is intentionally small. It should help you retrieve and review notes without making writing feel heavy.

## Common Fields

```yaml
type: note
area:
  - learning
topics:
  - "[[Obsidian]]"
aliases:
status: draft
lang:
  - en
created: "{{date:YYYY-MM-DD}}"
updated: "{{date:YYYY-MM-DD}}"
```

## Fields

| Field | Purpose |
| --- | --- |
| `type` | Defines the role of the note: `note`, `moc`, `source`, `idea`, `project`, `journal`, or `dashboard`. |
| `area` | Defines the main life/work area. Use one simple value and optionally one linked MOC. |
| `topics` | Connects the note to concepts, MOCs, or related themes. |
| `aliases` | Helps retrieve the note through alternative names, translations, or abbreviations. |
| `status` | Tracks maturity: `draft`, `active`, `stable`, `private`, or `archived`. |
| `lang` | Indicates the main language of the note. |
| `created` | Creation date. |
| `updated` | Last meaningful update date. |

## Optional Fields

| Field | Use When |
| --- | --- |
| `description` | The note is a MOC, dashboard, or central concept. |
| `next_action` | The note is actionable. |
| `deadline` | There is a real date constraint. |
| `impact` | You review ideas or projects by expected value. |
| `effort` | You review ideas or projects by cost. |
| `repo` | The note describes a software project. |
| `rating` | The note describes a source. |
| `link` | The note describes an external source. |
| `project` | The note supports a project and should be linked to the project control-tower note. |
| `ai_context_role` | The note has an optional role in AI handoffs, such as `context_brief`, `decision_log`, `action_log`, or `failed_attempts`. |
| `context_priority` | The note should be considered `high`, `medium`, or `low` priority when preparing AI context. |

## Optional AI Context Fields

Use these only when you actually use AI assistants across project sessions.

```yaml
type: note
project: "[[Project Name]]"
ai_context_role: context_brief
context_priority: high
```

These fields should help a human or tool find the right project context faster. They should not replace clear note titles, links, or short summaries. Do not create a new `type` value for AI memory notes; use `type: note` and keep the type model small.

## Rule

Do not add metadata because it looks organized. Add metadata when it improves search, filtering, review, or action.
