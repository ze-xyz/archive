---
created: 2024-07-30T19:26
updated: 2024-07-30T19:27
---
```dataview
TABLE WITHOUT ID
	file.link as "Notas"
FROM !"templates"
WHERE icontains(area, "matemática")
SORT file.name ASC
```
