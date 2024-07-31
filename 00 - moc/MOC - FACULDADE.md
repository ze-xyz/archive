---
created: 2024-07-10T08:13
updated: 2024-07-31T14:06
type: "[[index]]"
---
## SEMANAS ABERTAS
```dataview
TABLE WITHOUT ID
	file.link as "Disciplina",
	tema
FROM "04 - projects"
WHERE icontains(semana, "1")
AND icontains(status, "em andamento")
SORT file.name ASC
```

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

## SEMANAS CONCLUIDAS
```dataview
TABLE WITHOUT ID
	file.link as "Disciplina",
	tema
FROM "04 - projects"
WHERE icontains(semana, "1")
AND icontains(status, "concluído")
SORT file.name ASC
```

## REVISÕES
```dataview
TABLE WITHOUT ID
	file.link as "Semana",
	revisão
FROM "04 - projects"
WHERE icontains(revisado, "não") 
SORT file.name ASC
```
