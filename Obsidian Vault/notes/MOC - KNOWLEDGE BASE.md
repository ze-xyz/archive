---
created-date: 2024-07-22 09:11
tags: "#type/MOC"
summary: all map of content notes, people or projects.
---

```dataview
TABLE WITHOUT ID
file.link AS "name", summary, tags
FROM "notes"
WHERE !icontains(tags, "#type/person")
AND !icontains(tags, "#type/meeting")
AND !icontains(tags, "#type/project")
AND !icontains(tags, "#type/sub-project")
AND !icontains(tags, "#type/MOC")
```