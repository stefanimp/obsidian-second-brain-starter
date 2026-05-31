# Dataview Examples

These examples assume your processed notes live in `2-Notes`.

## Recent Notes in an Area

```dataview
TABLE WITHOUT ID file.link AS Note, type AS Type, status AS Status, file.mtime AS Updated
FROM "2-Notes"
WHERE contains(area, "learning")
SORT file.mtime DESC
LIMIT 30
```

## Notes Without Area

```dataview
TABLE WITHOUT ID file.link AS Note, type AS Type, status AS Status, file.mtime AS Updated
FROM "2-Notes"
WHERE !area
SORT file.mtime DESC
LIMIT 40
```

## Active Ideas

```dataview
TABLE WITHOUT ID file.link AS Idea, area AS Area, stage AS Stage, next_action AS "Next Action", impact AS Impact, effort AS Effort
FROM "2-Notes"
WHERE type = "idea" AND stage != "archived"
SORT impact DESC, effort ASC, file.mtime DESC
LIMIT 20
```

## Active Projects

```dataview
TABLE WITHOUT ID file.link AS Project, status AS Status, stage AS Stage, next_action AS "Next Action", deadline AS Deadline
FROM "2-Notes"
WHERE type = "project" AND status != "archived"
SORT deadline ASC, file.mtime DESC
```

## Draft Notes to Process

```dataview
TABLE WITHOUT ID file.link AS Note, type AS Type, area AS Area, file.mtime AS Updated
FROM "2-Notes"
WHERE status = "draft"
SORT file.mtime DESC
LIMIT 20
```

## Upcoming Deadlines

```dataview
TABLE WITHOUT ID file.link AS Note, deadline AS Deadline, type AS Type, next_action AS "Next Action"
FROM ""
WHERE deadline
  AND status != "archived"
  AND date(deadline) >= date(today)
  AND date(deadline) <= date(today) + dur(14 days)
SORT date(deadline) ASC
```

## Open Tasks Related to the Current MOC

```dataview
TASK
FROM [[]]
WHERE !completed
GROUP BY file.link
```
