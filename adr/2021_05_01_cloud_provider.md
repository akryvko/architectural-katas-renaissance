# Cloud based deployment
## Status
Proposed
## Context
We are about to develop and spin-up numerous new system components. Selected architecture style - service based architecture - implies that there will be multiple deployment units. The solution is designed for horizontal scalability, so we want to utilize such features as load balancing and load-based scaling. Also we would like to use some managed database solutions.
We tolerate multi-tenancy and other implications of cloud based solutions.
## Decision
* Deploy application components as well as databases to a cloud.
* Consider AWS as a cloud provider.
* For better resource utilization and cloud provider abstraction - use Kubernetes over AWS
* Consider another AWS managed services: S3, Kinesis, Dynamodb, Elasticache and other
# Consequences
* We are getting cost-efficient and stable infrastructure platform
* Developers and other teams have access to computing resources in few clicks
* Utilize secured solutions from well known provider


![aws](https://jsconsulting.services/wp-content/uploads/2018/05/AWS-Logo-small.jpg)
![k8s](https://www.stratoscale.com/wp-content/uploads/2019/04/Kubernetes-logo.png)