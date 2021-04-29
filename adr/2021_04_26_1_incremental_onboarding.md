# Incremental onboarding of the new system
## Status
Proposed
## Context
Current solution has a bunch of problems which impact business directly. They should be solved as soon as possible:
* Customers complaints due lost tickets, wrong consultants and wrong time.
* Availability problems
* Reliability issues - freezes, probably on spikes of usage.
## Decision
Since the ticketing workflow is the most critical and visible part of the system we offer to implement and onboard a new system here first. This partial solution will include:
* New ticket management UI for customers
* New ticket management UI for experts
* A layer of backend services for the new UI
* Data import mechanism so all existing tickets will be available in the new system
* Data replication mechanism so all tickets created in the new system will be available in the old one for purposes of reporting and billing.

Next step - BI solution for reports.

Next step - knowledge base.

And the final step - all the rest of components.

## Consequences
With incremental rollout we can benefit from the new system much faster. 
