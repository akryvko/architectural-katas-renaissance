# Need of a separate workflow manager for ticket workflow
## Status
Proposed
## Context
![workflow](../assets/ticket_worklfow.puml) 
* There is a certain [workflow](../assets/ticket_worklfow.puml) associated with tickets. 
* This workflow has many decision points. 
* It can also evolve over time.
* The different stages of a particular ticket needs to be visible to various stakeholders of the system for various business operations.
* Analytics needs to be done on the current workflow state to identify pain points and improve it.
* It is important that data doesnt get lost between these different stages of the workflow
## Decision
We need a worflow manager with the following properties:
- state persistence
- timers and delays
- long running operations support
- ability to install process in arbitrary state - so manager can change state
- visibility - allows to view items on each state
- visibility - allows to view whole transitions/states history

For this we may use a third party workflow manager (e.g. Activity) 
or we can build a workflow manager of our own. 
We think it would be good to explore a third party solution if we need a quick solution, 
the same could be used for contract management as well. 
We need to still explore the different options to come up with a favourable solution.
## Consequences
* It will be much easier to manage and improve workflow without impacting the core components.
* With the increased visibility it would be easier to come up with process improvements.

