# class 13
## Serverless Functions
erverless is a cloud computing execution model that

Automatically provisions the computing resources required to run application code on demand, or in response to a specific event; Automatically scales those resources up or down in response to increased or decreased demand; Automatically scales resources to zero when the application stops running.

This gives developers more time to develop and optimize their front-end application code and business logic. And with serverless, customers never pay for idle capacity. They pay only for the resources required to run their applications, and only when those applications are running.

The term 'serverless' describes the customer's experience with those servers: they are invisible to the customer, who doesn't see them, manage them, or interact with them in any way.

### Serverless vs. FaaS (function as a service)
Serverless and function as a service (FaaS) are often conflated. But FaaS is actually a subset of serverless - it's the compute paradigm central to serverless, wherein application code or containers run only in response to events or requests. Serverless includes FaaS plus all the other associated resources and cloud services and resources supporting the code - e.g. storage, databases, networks, API gateways, authentication - for which configuration, management and billing of services are invisible to the user.

### PRO's
* As noted above, serverless enables development teams to focus on writing code, not managing infrastructure.
serverless customers pay for execution only.
* Serverless is a polyglot environment, enabling developers to code in any language or framework
* serverless can be both faster and more cost-effective than other forms of compute
* Serverless application development platforms provide near-total visibility into system and user times, and can aggregate that information systematically.
### CON's
* it does not offer the same savings for workloads characterized by predictable, steady or long-running processes; in these cases a traditional server environment might be simpler and more cost-effective.
* sometimes need to start up from zero to serve a new request
* teams may find it difficult or impossible to monitor or debug serverless functions using existing tools or processes.
* deeply integrating with the native managed services of a specific cloud platform is where much of the value of cloud can be found; for others, this cloud lead to material lock-in risks that need to be mitigated.