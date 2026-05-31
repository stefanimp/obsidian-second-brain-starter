---
type: moc
area:
  - system
  - "[[Areas]]"
topics:
  - "[[Home]]"
aliases:
  - Areas
  - Life areas
description: Main map of the vault without depending on folders.
status: active
lang:
  - en
created: "{{date:YYYY-MM-DD}}"
updated: "{{date:YYYY-MM-DD}}"
---

# Areas

## Main Areas
- [[Projects]]
- [[Learning]]
- [[Work]]
- [[Health]]
- [[Finances]]
- [[Languages]]
- [[Books]]
- [[Life]]

## Active MOCs
```dataview
TABLE WITHOUT ID file.link AS MOC, area AS Area, status AS Status, file.mtime AS Updated
FROM "2-Notes"
WHERE type = "moc" AND status != "archived"
SORT area ASC, file.name ASC
```

## Notes Without Area
```dataview
TABLE WITHOUT ID file.link AS Note, type AS Type, status AS Status, file.mtime AS Updated
FROM "2-Notes"
WHERE !area
SORT file.mtime DESC
LIMIT 40
```

## System Rules
- Folders are trays: `0-Inbox`, `1-Templates`, `2-Notes`, `3-Media`.
- Areas live in the `area` property.
- Themes and relationships live in `topics` and links.
- A note can belong to one main area and connect sideways to many topics.
