---
tags:
  - networks
  - network
  - infrastructure
---

```dataview 
TABLE WITHOUT ID
    file.link AS "Network",
    file.frontmatter as "Properties"
FROM "Work/Networks" 
WHERE file.folder = this.file.folder
WHERE file.name != this.file.name
SORT file.name ASC 
```
