---
created: 2024-07-26T07:44
updated: 2024-07-29T12:13
---
```dataview
TABLE WITHOUT ID
	file.link as "Técnica",
	type
FROM !"templates"
WHERE icontains(up, this.file.link)
AND icontains(tags, "study-skill")
SORT file.name ASC
```
