---
type: dashboard
area:
  - system
  - "[[Areas]]"
topics:
  - "[[Areas]]"
aliases:
  - Home
status: active
lang:
  - en
created: "{{date:YYYY-MM-DD}}"
updated: "{{date:YYYY-MM-DD}}"
---

# Home

## Quick Entry
- [[0-Inbox/Inbox|Inbox]]
- [[Areas]]
- [[Projects]]
- [[Sources]]

## Deadlines: Next 14 Days
```dataview
TABLE WITHOUT ID file.link AS Note, deadline AS Deadline, type AS Type, status AS Status, next_action AS "Next Action"
FROM ""
WHERE deadline
  AND status != "archived"
  AND date(deadline) >= date(today)
  AND date(deadline) <= date(today) + dur(14 days)
SORT date(deadline) ASC, file.mtime DESC
LIMIT 30
```

## Inbox
```dataview
TABLE WITHOUT ID file.link AS Note, file.mtime AS Updated
FROM "0-Inbox"
SORT file.mtime DESC
```

## Notes That Need Processing
```dataview
TABLE WITHOUT ID file.link AS Note, type AS Type, area AS Area, status AS Status, file.mtime AS Updated
FROM "2-Notes"
WHERE !type OR !area OR status = "draft"
SORT file.mtime DESC
LIMIT 10
```

## Weekly Review
- [ ] Empty Inbox: delete, promote, connect, or incubate with a clear next action.
- [ ] Review tasks without dates.
- [ ] Review projects and active ideas.
- [ ] Update `next_action` fields.
- [ ] Create or update MOCs where navigation is getting weak.
