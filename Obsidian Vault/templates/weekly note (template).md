```dataview
TABLE WITHOUT ID
file.link as Date,
summary
FROM "journal"
WHERE icontains(week, this.file.link)
SORT date ASC
```