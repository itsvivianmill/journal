---
tags:
  - projects
  - tasks
---
---
Rough example of dynamic listing with Dataview plugin as a possible replacement for the Kanban requirements.

##  Projects with Tasks
```dataview 
TABLE WITHOUT ID
  file.link AS "Project",
  file.frontmatter.Criticality AS "Crit",
  file.frontmatter.Priority AS "Pri",
  file.frontmatter.tags AS "Tags",
  file.frontmatter.Responsible AS "Manager"

FROM "Work/Projects" 
WHERE any(file.tasks, (t) => !t.fullyCompleted)
WHERE file.folder = this.file.folder
WHERE file.name != this.file.name
SORT file.frontmatter.Priority DESC 
```

##  Projects Still Needing Breakdown
```dataview 
TABLE WITHOUT ID
  file.link AS "Project",
  file.frontmatter.Criticality AS "Crit",
  file.frontmatter.Priority AS "Pri",
  file.frontmatter.tags AS "Tags",
  file.frontmatter.Responsible AS "Manager"

FROM "Work/Projects" 
WHERE file.tasks = []
WHERE file.folder = this.file.folder
WHERE file.name != this.file.name
SORT file.frontmatter.Priority DESC 
```

## Tasks:
Full list, ordered by Priority
```tasks
not done
sort by priority
#limit 10
```


```dataview
TABLE WITHOUT ID
  file.link AS "Projects"
FROM "Work/Projects"
WHERE any(file.tasks, (t) => !t.fullyCompleted)
```
