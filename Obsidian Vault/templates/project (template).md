---
created-date: <% tp.date.now("YYYY-MM-DD HH:mm") %>
up: "[[MOC - PROJECTS]]"
related: 
aliases: 
tags:
  - "#type/project"
  - "#status/active"
---

>**summary**::

## Sub Projects
```dataview
TABLE WITHOUT ID
	file.link as "Sub Project",
	up,
	created-date,
	summary,
	tags
FROM !"Templates"
WHERE icontains(up, this.file.link)
AND icontains(tags, "type/sub-project")
SORT filename DESC
```

## Meetings
```dataview
TABLE WITHOUT ID
	file.link as session,
	up,
	created-date,
	participants,
	summary
FROM !"Templates"
WHERE icontains(up, this.file.link)
AND icontains(tags, "type/meeting")
SORT filename DESC
```

## Task and Questions

### Open
``` dataview
TASK
WHERE icontains(text, this.file.name)
AND (icontains(text,"#task") OR icontains(text,"#question"))
AND !completed
GROUP BY file.name as filename
SORT filename Desc
```
### Closed
```dataview
TASK
WHERE icontains(text, this.file.name)
AND (icontains(text,"#task") OR icontains(text,"#question"))
AND completed
GROUP BY file.name as filename
SORT filename DESC
```
### Sprints
```dataview
TASK
WHERE icontains(text, this.file.name)
AND icontains(text,"#log/sprint")
GROUP BY file.name as filename
SORT filename DESC
```