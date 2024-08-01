---
created: 2024-07-30T16:09
updated: 2024-07-30T16:25
---
```dataview
TABLE WITHOUT ID
	file.link as "notas",
	type,
	status
FROM !"99 - meta" 
WHERE icontains(area, "ciência da computação")
SORT file.name ASC
```
