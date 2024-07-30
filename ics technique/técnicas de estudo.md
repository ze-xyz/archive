---
created: 2024-07-26T07:44
updated: 2024-07-30T10:45
---
```dataview
TABLE WITHOUT ID
	file.link as "Técnica",
	type
FROM !"templates"
WHERE icontains(tags, "ICS")
SORT file.name ASC
```
