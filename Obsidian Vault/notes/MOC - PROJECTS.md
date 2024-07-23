---
created-date: 2024-07-22 09:03
tags: "#type/MOC"
summary: all projects
---

### Open Projects
```dataview
TABLE WITHOUT ID
	file.link as "project",
	up,
	created-date,
	summary,
	tags
FROM !"templates"
WHERE icontains(tags, "type/project")
AND !icontains(tags, "status/complete")
SORT filename DESC
```

### Close Projects
```dataview
TABLE WITHOUT ID
	file.link as "project",
	up,
	created-date,
	summary,
	tags
FROM !"templates"
WHERE icontains(tags, "type/project")
AND icontains(tags, "status/complete")
SORT filename DESC
```