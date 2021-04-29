# Software system characteristics
Here we define the most important characteristics of the target system. Some of them are architecturally significant so influence architectural decisions, others we will fulfill using other ways, e.g. software design and engineering practices.
##Architecturally significant characteristics

| Characteristic | Motivation. Why? |
|---|---|
| Availability | The business is dependent on how the system is available. Also it was identified that the current system suffers from lack of availability. |
| Scalability | We want to be able to address potential performance limitations and growing users auditory by adding resources to the system. We don't need to design for an exponential scale here. Expected load - hundreds requests per second.|
| Elasticity | It was identified that the current system suffers from user activity spikes. |
| Testability | We want to avoid the current situation when it is risky to make changes into the system. |
| Maintainability | We want to avoid the current situation when it is risky to make changes into the system. |
| Evolvability | Since the problems of the existing system are quite urgent we need to develop a system which can be onboarded asap partially to cover the most painful areas but also evolve to the comprehensive solution. |
| Recoverability | In the current system some data is getting lost in case of system failures (experts do not get tickets). We need to ensure that this does not happen as this leads to customer frustration. |
| Monitor-ability | In the current system, they do not know why the system crashes (they are guessing it's due to high traffic but there isn’t any proof). We should be able to monitor the new system appropriately to help debug issues. |

