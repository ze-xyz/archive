---
created-date: 2024-07-22 09:09
tags: "#type/MOC"
summary: all sprints
---

```dataview
TASK
FROM !"templates"
WHERE icontains(tags, "#log/sprint")
GROUP BY file.link as filename
SORT filename DESC
```