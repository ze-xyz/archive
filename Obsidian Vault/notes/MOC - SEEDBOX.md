---
created-date: 2024-07-22 09:16
tags: "#type/MOC"
summary: all notes that need processing
---

## Seed logs
```dataview
task
WHERE icontains(text, "log/seedbox")
```
## Seed  notes
```dataview
TABLE
dateformat(file.name, "yyyy-MM-dd") AS "Last modified"
FROM "seedbox"
SORT file.ctime ASC
```