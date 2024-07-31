---
created: 2024-07-30T19:16
updated: 2024-07-30T19:44
---
```dataview
TABLE WITHOUT ID
	file.link as "nota",
	type,
	status
FROM !"templates"
WHERE icontains(area, "competitive programing")
SORT file.name ASC
```
