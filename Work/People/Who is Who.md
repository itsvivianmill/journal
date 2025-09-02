---
tags:
  - contact
  - skills
  - interests
---

This is a rough working draft, using Dataview, to dynamically extract information from pages in the `Work/People` folder and display them in a tabular index.

---
```dataview 
TABLE 
    file.frontmatter.Nickname AS "Nickname",
	file.frontmatter.Role AS "Role", 
	file.frontmatter.Phone AS "Phone", 
	file.inlinks AS "Connections"
FROM "Work/People" 
WHERE file.folder = this.file.folder
WHERE file.name != this.file.name
SORT file.name ASC 
```
---
##### Available Properties
The following is a single object detailing all of the properties available for the table above.
```dataview 
TABLE 
    file AS "Properties"
FROM "Work/People" 
WHERE file.folder = this.file.folder
WHERE file.name != this.file.name
SORT file.name ASC 
LIMIT 1
```

