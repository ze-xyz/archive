---
created-date: 2024-07-22 09:06
tags: "#type/MOC"
summary: all tasks
---

## Open
>```dataview
>TASK WHERE icontains(text, "#task")
>AND !completed
>GROUP BY file.name as filename
>sort filename desc
>```

## Closed
>```dataview
>TASK WHERE icontains(text, "#task")
>AND completed
>GROUP BY file.name as filename
>sort filename desc
>```