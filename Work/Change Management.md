---
tags:
  - tasks
  - projects
  - Policy
---
Policy proposal by [[Vivian M]]
## Definitions 
- **Change**: Any modification to IT services, infrastructure, applications, or configurations. 
- **Change types/levels**:
	- **Standard Change**: Low-risk, pre-approved changes (e.g., patching). 
	- **Emergency Change**: Critical change needed to fix a major incident or vulnerability.
	- **Normal Change**: All other changes requiring assessment and approval. 
## Roles and Responsibilities 
- **Change Initiator**: Proposes and documents the change request 
- **Change Manager**: Manages the overall change process and ensures policy compliance
- **Change Advisory Board**: Reviews and approves Normal and Major changes.
- **Implementers**: Execute the approved changes. 

## Approval Workflow 
This depends on the type of change, as listed here:
- **Standard Changes**: Pre-approved, documented in a standard change catalog.
- **Normal Changes**: Reviewed and approved by CAB during weekly meetings.
- **Emergency Changes**: Approved by Change Manager + IT Director (or delegated authority) outside of regular CAB. 
### Testing Validation 
All changes must be tested in a staging environment *before* production deployment unless deemed unnecessary (standard/emergency changes). 

Testing results must be documented. 

Testing process may vary depending on various things, but should always have sanitized-live-data to test with and be a repeatable process.
## Communication Plan 
Send follow-up communication after successful implementation or in case of issues Consistent list of members (perms, access, etc.) 

Post-Implementation Review:
	Was the change successful? 
	Any unanticipated issues? 
	What lessons were learned? 

Update documentation if needed.
## Monitoring and Metrics 
All IT changes will be monitored using real-time dashboards and alerting systems configured in Grafana and notify system administrators of anomalies or failures. 
## Compliance Policy 

## Review and Updates