---
tema:
---
```dataview
TABLE WITHOUT ID
	file.link as "Notas"
FROM !"templates"
WHERE icontains(area, "{{title}}")
SORT file.name ASC
```
