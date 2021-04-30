# Meet the Team

We are a team of 3 Software Engineers working together for a big European fashion platform.  
We have to make architectural decisions in our daily work and want to be better on this field.

![team](./assets/r_team.png?v=3)

# Narrative
As the new Sysop Squads Software Architects, we have been presented with a system, that is currently live and serving real users. This system has certain properties and certian problems. Our job is to help solve those problems in the best way possible.

To do this we first tried to understand what is expected out of the system, who will use it and for what. We created [User stories](docs/user_stories.md). 
We also looked at the issues which the team is facing currently ([Existing problems](./docs/problems.md)). We then tried to identify the architectural requirements for the system ([Software system characteristics](docs/system_characteristics.md)).

Having done this analysis, we tried to identify components that could serve our user stories, coming up with [Actor Actions Diagram](diagrams/1_actor_action.md).
We then tried to club some components, and tried to come up with a domain driven coarse grained service diagram with user interface interaction [diagram]. [Use case diagrams] for each of our main actors also helped us to see how these would be used, and if each of these service provide the non-functional requirements for the use cases it supports. We also defined interactions between components [diagram] to check the if the level of granularity is not too much. 
Having done this, we planned the final deployment and depict it in the [deployment diagram].

Now, we had an idea of what our preferable end sytem looked like. What was left was to think about how we would achieve that stage. We looked at all the current cmponents and database to come with a proposal for the migration. Key points we considered during this was that we would want to solve problems as soon as possible. All this was highlighted in our [Migration Plan]

# Analysis

[User stories](docs/user_stories.md)

[Software system characteristics](docs/system_characteristics.md)

[Actor Actions Diagram](diagrams/1_actor_action.md)

# Architectural Decision Records

[Incremental onboarding of the new system](adr/2021_04_26_1_incremental_onboarding.md)

[Separated data warehouse for reporting](adr/2021_04_27_1_separated_warehouse.md)

[Use 3d party BI tool for reporting](adr/2021_04_27_2__bi_tool.md)

[Use 3d party Knowledge Base tool](adr/2021_04_28_1_kb_tool.md)


# Logical view

Links to component diagrams goes here

# Deployment view

Links to diagrams goes here
