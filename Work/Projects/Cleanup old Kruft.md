---
Criticality: medium
Priority: low
tags:
  - projects
  - tasks
  - infrastructure
Responsible:
  - "[[Vivian M]]"
---
---
## Description
Many old VMs, Containers and devices are cluttering up our environment and are not in use. The can cause issues in the form of wasted resources, security holes, or just annoyances.

## Purpose
Recover all "unknown" hardware and validate our systems itemization list.

## Tasks
- [ ] Ensure that a tool such as NtopNG or similar are installed to interrogate the network on a constant basis
- [ ] Using `arp-scan` and simialr tools, generate a hardware "connected" list
- [ ] Ensure all devices found, match the [[Hardware]] list, hunt down what we cant define - and address it with prejudice ;)