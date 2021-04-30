# Existing problems
* Customer complains due lost tickets, wrong consultants and wrong time. [Recoverability](./system_characteristics.md).
  >Customers are complaining that consultants are never showing up due to lost tickets, and often times the wrong consultant shows up to fix something they know nothing about.
* [Availability](./system_characteristics.md) problems.
  >Customers and call-center staff have been complaining that the system is not always available for web-based or call-based problem ticket entry.
* Difficult and risky changes in monolith. [Testability](./system_characteristics.md). [Maintainability](./system_characteristics.md).
  >Change is difficult and risky in this large monolith - whenever a change is made, it takes too long and something else usually breaks.
* Reliability issues - freezes, probably on spikes of usage. [Elasticity](./system_characteristics.md).
  >Due to reliability issues, the monolithic system frequently “freezes up” or crashes - they think it’s mostly due a spike in usage and the number of customers using the system