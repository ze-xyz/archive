---
created: 2024-07-29T09:51
updated: 2024-07-29T09:58
---
```dataview
TABLE WITHOUT ID
	file.link as "Curso",
	trilha,
	etapa
FROM !"99 - meta/templates"
WHERE icontains(up, this.file.link)
SORT file.name ASC
```
