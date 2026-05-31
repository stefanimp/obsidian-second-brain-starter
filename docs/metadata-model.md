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

## Rule

Do not add metadata because it looks organized. Add metadata when it improves search, filtering, review, or action.
