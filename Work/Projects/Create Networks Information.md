---
Criticality: medium
Priority: high
tags:
  - infrastructure
  - network
  - projects
  - tasks
Responsible:
  - "[[Garth Johnson]]"
  - "[[Vivian M]]"
---
---

## Purpose
We need to be able to easily reference all networking information that comprises our domain. With this info we can devise better and more effective security and maintenance plans and policies.
## Description
A folder with automatic templates that include all relevant information stubs to maintain a list of each network, vlan, etc.

## Tasks
- [ ] Create a `Work/Networks` folder and populate it with the following:
	- [ ] create a [[Network]] template in `_templates`
	- [ ] Assign the [[Network]] template to be automatically used for the folder using Templater plugin
	- [ ] populate Networks folder with example items from out current domain using the template
	- [ ] create [[Network INDEX]] page to dynamicly list all network info pages added
