---
Criticality: medium
Priority: high
tags:
  - Policy
  - projects
  - tasks
Responsible:
  - "[[Vivian M]]"
  - "[[Garth Johnson]]"
---
---
## Purpose
To make clear and easy to refer to, what is being done, by whom, when, how , and why. Organization begins with good collaboration and communication.
## Description
This is a multi-phase project that will require a few others to be completed first. The components required for this are:
- live collaboration
- version control
- easy access to editing and viewing
- integration with member list
- integration with documentation
- integration with live network scans of devices and network configuration
- feature rich task management (if possible, with a kanban and burndown charts)
## Committee
- [[Garth Johnson]]
- [[Vivian M]]
- [[Ricky M]]
- [[Lilian M]]

## Tasks
- [x] Install the necessary plugins ✅ 2025-08-30 
	- [x] Kanban ✅ 2025-08-30
	- [x] Tasks ✅ 2025-08-30
	- [x] Dataview ✅ 2025-08-30
	- [x] Templater ✅ 2025-08-30
	- [x] Relay ✅ 2025-08-30
- [x] Set up call with interested parties ✅ 2025-08-29
	- [x] Garth ✅ 2025-08-29
	- [x] Viv ✅ 2025-08-29
- [ ] Determine a solution for collaborative editing if possible
	- [x] Relay plugin [code](https://github.com/No-Instructions/Relay) and sync server [code](https://github.com/No-Instructions/relay-server). Relay seems to work very well for everything ***except*** Kanban. So, we will need a better solution to avoid the licensing costs and keep content local-only. ✅ 2025-08-31
	- [ ] Test alternative sync plugin [here](https://github.com/vrtmrz/obsidian-livesync) - it uses WebRTC and would require us to have a live hosted/running copy to sync with at BMS.  I think this may be a better solution. - [[Garth Johnson]] ⏫ 
- [x] Create demonstration Vault ✅ 2025-08-30
	- [x] Create templates for Services, Systems, People, Projects, etc ✅ 2025-08-30
	- [x] see [[Systems and services List]] ✅ 2025-08-30
	- [x] see [[Hardware]] ✅ 2025-08-30
	- [x] Create Folders with templates automatically assigned ✅ 2025-08-30
	- [x] Create example pages for people, systems, and services ✅ 2025-08-30
	- [x] Create example projects ✅ 2025-08-30
- [x] Test to see if Kanban publishes to/through the Relay - [[Garth Johnson]] ✅ 2025-08-31
	- [x] Kanban plugin data is stored within the plugins directory and therefore is incompatible with Relay. Need to checkout self hosting code and see if this can be manually resolved instead - [[Garth Johnson]] ✅ 2025-08-31

## Notes and Cautions:
- Relay plugin stores content remotely by default. This may be a security issue.
- Relay requires a license, even when self hosted.
- Relay does not include the plugins folder or config files!!! This explains a LOT. The Kanban stores its info in a `json` doc within the `plugins` folder.

