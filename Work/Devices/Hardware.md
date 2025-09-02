---
tags:
  - infrastructure
  - devices
  - hardware
  - assets
---


---
- [ ] Create pages for each of the following with all available information
	- [ ] Advantec fiber modem
	- [ ] Mikrotik RB4011(?) router
	- [ ] Mikrotik CRS326 router
	- [ ] Mikrotik CS326 switch
	- [ ] Mikrotik CapAC
	- [ ] HP - PVE
	- [ ] HP - Crash
	- [ ] Dell R630 - PVE2
	- [ ] Dell R630 PVE3
	- [ ] IBM - Proxmox Backup
	- [ ] Camera system
	- [ ] Doorlock system
	- [ ] Lab systems
		- [ ] Lab1
		- [ ] Lab2
		- [ ] lab3
		- [ ] lab4
		- [ ] lab5
	- [ ] Woodshop1
	- [ ] Woodshop2
	- [ ] Caleb's laptop
	- [ ] front (greeter) desk system
	- [ ] Trundle Cart system
	- [ ] Tech area system
	- [ ] Frank
	- [ ] Lazer cuter system
	- [ ] IoT devices in Jim's area


---
```dataview 
TABLE
  file.frontmatter.IP AS "Address",
  file.frontmatter.Requires AS "Requires" 
FROM "Work/Devices" 
WHERE file.folder = this.file.folder
WHERE file.name != this.file.name
SORT file.name ASC 
```
---
### Available Properties
```dataview 
TABLE 
    file AS "Object"
FROM "Work/Devices" 
WHERE file.folder = this.file.folder
WHERE file.name != this.file.name
SORT file.name ASC 
LIMIT 1
```
