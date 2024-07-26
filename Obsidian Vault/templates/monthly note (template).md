---
created: 2024-07-22T08:57
updated: 2024-07-26T13:08
---
```dataview
TABLE WITHOUT ID
file.link as Date,
summary
FROM "journal/01 daily/<% moment(tp.file.title,'YYYY-MM-DD').format("YYYY") %>/<% moment(tp.file.title,'YYYY-MM-DD').format("MM") %>"
SORT date ASC
```
