---
tags:
  - services
---


---
Create a page in this folder with all available information for each of the following:
(everyone can help with this - and indeed will need to on an ongoing basis)

- [ ] DNS
- [ ] Firewall
- [ ] DHCP
- [ ] Storage (primary)
	- [ ] Shared and network
- [ ] Storage (backup)
- [ ] Backup service(s)
- [ ] VPN (Wireguard)
- [ ] Hypervisor (Proxmox)
- [ ] Docker Production swarm
- [ ] Docker Development Swarm
- [ ] Git version control repo (internal)
- [ ] Git version control repo (external and public - GitHub)
- [ ] Task management software (this?) ⏫
- [ ] Documentation service(s)
- [ ] Discord (all relevant, list admins for each)

NOTE: Continue to add more as we think of them or add them. This page should continue to be updated.

NOTE: Continue to modify the [[Device]] and [[Service]] templates as we find more properties or format changes that make better sense.  Remember to retro-fit existing pages as we do so.  For this reason, we will want to add a few, test it out thoroughly, make mods to the templates and pages, then after that add a few more using the updated templates again - until the format is clean and consistent.

NOTE: Each of the pages should include links to the hardware used to implement them
This is a rough working draft using Dataview to dynamically extract information from pages in the People folder and display them in a tabular index.

---
### Managed Services
```dataview 
TABLE 
file.frontmatter.Ports AS "Ports"
FROM "Work/Services" 
WHERE file.folder = this.file.folder
WHERE file.name != this.file.name
SORT file.name ASC 
```
---
##### Available Service Page Properties
```dataview 
TABLE 
    file AS "Properties"
FROM "Work/Services" 
WHERE file.folder = this.file.folder
WHERE file.name != this.file.name
SORT file.name ASC 
LIMIT 1
```
## Tasks
- [ ] Review all services available in the network. Use our SIEMs and etc 🔁 every month 