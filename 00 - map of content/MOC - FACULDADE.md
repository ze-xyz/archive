---
created: 2024-07-10T08:13
updated: 2024-07-26T14:34
type: "[[index]]"
---
## DISCIPLINAS ABERTAS
```dataview
TABLE WITHOUT ID
	file.link as "Disciplinas",
	Nome,
	Semestre
FROM !"99 - meta/templates"
WHERE icontains(up, this.file.link)
AND icontains(tags, "type/disciplina")
SORT file.name ASC
```

## SEMANAS 1
```dataview
TABLE WITHOUT ID
	file.link as "Disciplina",
	tema
FROM !"Templates"
WHERE icontains(Semana, "1")
SORT file.name ASC
```