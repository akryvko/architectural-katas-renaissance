# Separated data warehouse for reporting
## Status
Accepted
##Context
In the  current solution the same database is used for operational activities and for report generation. We want to change this because:
* It is hard to change the data structure, since it has multiple dependencies.
* Data models cannot be optimized for a single purpose.
* Report generation can impact performance of the main system.
## Decision
* Onboard a separated data warehouse solution which allows storing and querying a big amount of data. We are considering Redshift since it scales very good, integrates with other AWS services, and supports a variety of BI tools.
* Import existing data from the operational database.
* Build pipelines for publishing new data into the data warehouse.
![redshift](https://cdn.sisense.com/wp-content/uploads/aws-redshift-connector.png)
## Consequences
* We are getting a reliable data platform for any BI applications.
* Operational database(s) can evolve independently. 
