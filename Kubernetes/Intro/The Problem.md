#kubernetes 
# Monoliths
The classic method of structuring applications is creating monoliths. All inclusive bundle of code that has everything it needs.

## Challenges
The monolith structure presents challenges as it grows larger. Functions become too tightly coupled. So more knowledge and understanding of each and every part is required to expand or rewrite even small pieces. 

Horizontal hardware expansion isn't supported, cost of upgrading the system to meet new requirements grows exponentially the larger the system gets. 

Updating a monolith often means taking down the entire application or service, because of how tightly coupled functions and processes are.

# Microservices
A common modern approach is to breakdown an application or service into microservices, that is standalone applications or services which can be easily created or destroyed and run on the same or separate resources. Microservices are aligned with [[Event-Driven Architecture]] and [[Service-Oriented Architecture]], which enables complex applications to be broken down into simpler pieces that are more easily maintained, secured, and expanded.
## Benefits
Microservices are simpler to maintain. Due to the nature of a microservice being loosely coupled to other components it is more narrow in scope than its monolith counterpart.

Due to the nature of Microservices being loosely coupled, it means that different services can be written in different languages.

Horizontal scaling is easier. Microservices being standalone applications means it is simpler to enable a service to run across multiple devices.

Updating can be done progressively. Where it makes sense updating can be performed as a rollout, so the service can be live and available even while parts are being progressively changed. Minimized downtime with microservices.

## Costs
Microservices make the architecture surrounding a large application more complex. More unique tools will be required to be built, implemented, or possibly imported. The most common solution is to use a tool like Kubernetes to solve this problem.

# Next
[[Containers]] are how microservices are implemented within Kubernetes.