---
tags:
  - testing
---
## Tags by Number of Pages
```dataview
TABLE WITHOUT ID  
	(tag + " (" + length(rows.file.link) + ")") AS Tags
FROM ""  
WHERE file.tags  
FLATTEN file.tags AS tag  
GROUP BY tag  
SORT length(rows.file.link) DESC
```
## Pages Without  Any Tags
```dataview
LIST
FROM ""  
WHERE !file.tags
```
