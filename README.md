# Meet the Team

We are a team of 3 Software Engineers working together for a big European fashion platform.  
We have to make architectural decisions in our daily work and want to be better on this field.

![team](./assets/r_team.png?v=4)

# Narrative
As the new Sysop Squads Software Architects, we have been presented with a system, that is currently live and serving real users. This system has certain properties and certain problems. Our job is to help solve those problems in the best way possible.

To do this we first found what is expected out of the system, who will use it and for what. We created [User stories](docs/user_stories.md). 
We also looked at the issues which the team is facing currently ([Existing problems](./docs/problems.md)). We then identified the architectural requirements for the system ([Software system characteristics](docs/system_characteristics.md)).

Having done this analysis, we identified the components that could serve our user stories, coming up with [Actor Actions Diagram](diagrams/1_actor_action.md).
We then reiterated to club some components, and came up with a domain driven service [diagram](diagrams/50_ui_components.md) with user interface interaction. [Use case diagrams](diagrams/3_use_case_diagram.md) for each of our main actors also helped us to see how these would be used, and if each of these service provide the non-functional requirements for the use cases it supports. We also defined interactions between components [diagram](./diagrams/30_components.md) to check if the level of granularity is not too much. 

This led us to chose **Service Based Architecture**. The reasoning for this can be found [here](adr/2021_04_30_1_service_oriented_architecture.md).
Having done this, we planned the final deployment and depicted it in the [deployment diagram](diagrams/60_deployment.md).

Now, we knew what our preferable end system looks like. What was left was to think about how we would achieve that stage. We looked at all the current components and database to come with a proposal for the migration. Key points we considered during this was that we would want to solve problems as soon as possible. All this was highlighted in our [Migration Plan](docs/migration_plan.md).

# Analysis

[User stories](docs/user_stories.md)

[Software system characteristics](docs/system_characteristics.md)

[Actor actions diagram](diagrams/1_actor_action.md)

[Use case diagram for actors](diagrams/3_use_case_diagram.md)

# Architectural Decision Records

[Use of service based architecture](adr/2021_04_30_1_service_oriented_architecture.md) 

[Separated data warehouse for reporting](adr/2021_04_27_1_separated_warehouse.md)

[Separate workflow manager for ticket](adr/2021_04_30_2_ticket_workflow_manager.md)

[Use 3d party BI tool for reporting](adr/2021_04_27_2__bi_tool.md)

[Use 3d party Knowledge Base tool](adr/2021_04_28_1_kb_tool.md)

[Cloud-based deployment](adr/2021_05_01_cloud_provider.md)

# Logical view

[Components](diagrams/30_components.md)

[Ticket flow components](diagrams/40_ticket_flow_components.md)

[Ticket flow sequence diagram](diagrams/15_ticket_flow_sequence.md)

[UI <--> components diagram](diagrams/50_ui_components.md)

# Deployment view

[Deployment diagram](diagrams/60_deployment.md)
