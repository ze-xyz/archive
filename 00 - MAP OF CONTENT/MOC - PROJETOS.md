---
created: 2024-08-02T07:32
updated: 2024-08-02T07:53
---
```dataview
TABLE WITHOUT ID
	file.link as "Nome",
	type,
	area,
	status
FROM !"99 - meta"
WHERE icontains(up, this.file.link)
SORT file.name ASC
```