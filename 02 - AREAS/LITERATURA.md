---
created: 2024-07-30T16:15
updated: 2024-08-02T08:00
---
## LIVROS
```dataview
TABLE WITHOUT ID
	file.link as "livro",
	autor,
	status,
	tags as "tipo"
FROM !"99 - meta"
WHERE icontains(type, "livro")
SORT file.name ASC
```

## NOTAS
```dataview
TABLE WITHOUT ID
	file.link as "Nota",
	type
FROM !"templates"
WHERE icontains(area, "literatura")
SORT file.name ASC
```
