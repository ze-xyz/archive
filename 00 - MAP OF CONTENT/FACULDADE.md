---
created: 2024-07-10T08:13
updated: 2024-08-02T16:36
up: "[[MOC - PROJETOS]]"
tags:
  - moc
type:
  - curso
area:
  - ciência da computação
status:
  - em andamento
---
## DISCIPLINAS ABERTAS
```dataview
TABLE WITHOUT ID
	file.link as "Disciplinas",
	Nome,
	Semestre
FROM !"99 - meta"
WHERE icontains(up, this.file.link)
AND icontains(tags, "type/disciplina")
SORT file.name ASC
```

## SEMANAS ABERTAS
```dataview
TABLE WITHOUT ID
	file.link as "Disciplina",
	tema,
	inicio
FROM "03 - PROJECTS"
WHERE icontains(semana, "")
AND icontains(status, "em andamento")
SORT file.name ASC
```


## SEMANAS CONCLUIDAS
```dataview
TABLE WITHOUT ID
	file.link as "Disciplina",
	tema
FROM "03 - PROJECTS"
WHERE icontains(semana, "1")
AND icontains(status, "concluído")
SORT file.name ASC
```

## REVISÕES
```dataview
TABLE WITHOUT ID
	file.link as "Semana",
	revisão
FROM "03 - PROJECTS"
WHERE icontains(revisão, "")
SORT file.name ASC
```
