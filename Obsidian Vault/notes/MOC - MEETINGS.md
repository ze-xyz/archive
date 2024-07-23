---
created-date: 2024-07-22 09:08
tags: "#type/MOC"
summary: all meetings
---

```dataview
TABLE WITHOUT ID
file.link AS "meeting", up, summart, tags
FROM !"templates"
WHERE icontains(tags, "#type/meeting")
```
