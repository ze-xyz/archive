---
created-date: 2024-07-22 09:15
tags: "#type/MOC"
summary: all people
---

```dataview
TABLE WITHOUT ID
file.link AS "name", summary, tags
FROM !"templates"
WHERE icontains(tags, "#type/person")
```