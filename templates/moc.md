---
type: moc
area:
  - area-name
topics:
  - "[[{{title}}]]"
aliases:
description:
status: active
lang:
  - en
created: "{{date:YYYY-MM-DD}}"
updated: "{{date:YYYY-MM-DD}}"
---

# {{title}}

## Manual Map
-

## Related Notes
```dataview
TABLE WITHOUT ID file.link AS Note, type AS Type, area AS Area, status AS Status, file.mtime AS Updated
FROM "2-Notes"
WHERE file.path != this.file.path
AND (
  contains(topics, this.file.link)
  OR contains(topics, this.file.name)
  OR contains(area, this.file.link)
  OR contains(area, this.file.name)
)
SORT status ASC, file.mtime DESC
```

## Open Tasks
```dataview
TASK
FROM [[]]
WHERE !completed
GROUP BY file.link
```
