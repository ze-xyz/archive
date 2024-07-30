---
created: 2024-07-10T08:13
updated: 2024-07-30T16:27
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

## SEMANAS ABERTAS
```dataview
TABLE WITHOUT ID
	file.link as "Disciplina",
	tema
FROM !"Templates"
WHERE icontains(Semana, "1")
AND icontains(tags, "status/active")
SORT file.name ASC
```

## SEMANAS CONCLUÍDAS
```dataview
TABLE WITHOUT ID
	file.link as "Disciplina",
	tema
FROM !"Templates"
WHERE icontains(Semana, "1")
AND !icontains(tags, "status/active")
SORT file.name ASC
```
