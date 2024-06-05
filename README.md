Notes and Resources for the AZ-900 certification.

# Describe cloud concepts


## Describe cloud computing


### What is cloud computing?

Cloud computing is the delivery of computing services over the internet.


### What is the shared responsibility model

Customers are always responsible for:
- The information and data stored in the cloud
- Devices that are allowed to connect to your cloud
- The accounts and identities of the people, services, and devices within your organization

The cloud provider is always responsible for:
- The physical datacenter
- The physical network
- The physical hosts

Your service model will determine responsibility for things like:
- Operating systems
- Network controls
- Applications

This depends on the Type of Service:

|Type|Client Responsibility|
|-|-|
|**S**oftware **a**s **a** **S**ervice|Less|
|**P**latform **a**s **a** **S**ervice|Neutral|
|**I**nfrastructure **a**s **a** **S**ervice|More|

![Infographic Overview Responsibility](https://learn.microsoft.com/en-us/training/wwl-azure/describe-cloud-compute/media/shared-responsibility-b3829bfe.svg)


### Define cloud models


|Public cloud|Private cloud|Hybrid cloud|
|-|-|-|
No capital expenditures to scale up|Organizations have complete control over resources and security|Provides the most flexibility|
Applications can be quickly provisioned and deprovisioned|	Data is not collocated with other organizations’ data|	Organizations determine where to run their applications|
Organizations pay only for what they use|	Hardware must be purchased for startup and maintenance|	Organizations control security, compliance, or legal requirements|
Organizations don’t have complete control over resources and security|	Organizations are responsible for hardware maintenance and updates||

Multi-cloud:
- Multiple public cloud providers

Azure Arc:
- Set of technologies that helps manage the cloud environment.

Azure VMware Solution:
- Run your VMWare workloads in Azure


### Consumption based model
Capital Expenditure(CapEx):
- Typically one-time up-front payment
- E.g new datacenter

Operational Expenditure(OpEx):
- Spending money on services over time
- Leasing a company vehicle

Consumption-based model is OpEx

This consumption-based model has many benefits, including:

No upfront costs.
- No need to purchase and manage costly infrastructure that users might not use to its fullest potential.
- The ability to pay for more resources when they're needed.
- The ability to stop paying for resources that are no longer needed.

You typically pay only for the cloud services you use, which helps you:

- Plan and manage your operating costs.
- Run your infrastructure more efficiently.
- Scale as your business needs change.


## Describe the benefits of using cloud services

### High availability and scalability

#### Availability
- focuses on ensuring maximum availability
- Azure is highly available cloud environment
- Service Level Agreements define the availability

|Uptime|per Week|per Month|
|-|-|-|
|99%|1.6h|7.2h|
|99.9%|10min|43min|

--> SLAs should be selected accordingly

#### Scalability
Ability to adjust resources to meet demand. 
- Adding resources to match increasing demand
- No overpaying for services

**Vertical Scaling**
- scaling up by increasing the resources quality -> e.g more CPU or RAM
- scaling down by decreasing the resources quality

**Horizontal Scaling**
- scaling out -> Adding resources (More servers)
- scaling in -> Removing resources (Less servers)
- One can scale horizontally by simply increasing the number of resources

Scaling can happen manually or automatically to match demand.

### Benefits of reliability and predictability in the cloud

#### Reliability
- Ability to recover from failures and continue to function.
- The clouds decentralized design enables reliable and resilient infrastructure.
- Global scale helps in catastrophic events

#### Predictability 
Performance predictability and cost predictability helps building confidence

**Performance**
- Performance predictability focuses on predicting the resources needed to deliver a positive experience for your customers.
- Cloud features like Autoscaling, load balancing, high availability lead to performance predictability

**Cost**
- Cost predictability is focused on predicting or forecasting the cost of the cloud spend
- Real time tracking, Data Analysis, Total Cost of Ownership, Pricing Calculator

### Security and governance
**Governance and compliance**
- Cloud based auditing
- Templates
- Automatic Updates

**Security**
- Maximum control via IaaS
- Well suited to handle things like distributed denial of service (DDoS) attacks

### Manageability
Two types:

#### Management of the cloud
Management of the cloud speaks to managing your cloud resources. In the cloud, you can:
- Automatically scale resource deployment based on need.
- Deploy resources based on a preconfigured template, removing the need for manual configuration.
- Monitor the health of resources and automatically replace failing resources.
- Receive automatic alerts based on configured metrics, so you’re aware of performance in real time.

#### Management in the cloud
Management in the cloud speaks to how you’re able to manage your cloud environment and resources. You can manage these:

- Through a web portal.
- Using a command line interface.
- Using APIs.
- Using PowerShell.

## Cloud service Types

### Infrastructure as a Service

Infrastructure as a service (IaaS) is the most flexible category of cloud services, as it provides you the maximum amount of control for your cloud resources.

Refer to the shared responsibility model.

Some common scenarios where IaaS might make sense include:

- Lift-and-shift migration: You’re setting up cloud resources similar to your on-prem datacenter, and then simply moving the things running on-prem to running on the IaaS infrastructure.
- Testing and development: You have established configurations for development and test environments that you need to rapidly replicate. You can start up or shut down the different environments rapidly with an IaaS structure, while maintaining complete control.

### Platform as a Service
Platform as a service (PaaS) is a middle ground between renting space in a datacenter (infrastructure as a service) and paying for a complete and deployed solution (software as a service).
Refer to the shared responsibility model.

Some common scenarios where PaaS might make sense include:

- Development framework: PaaS provides a framework that developers can build upon to develop or customize cloud-based applications. Similar to the way you create an Excel macro, PaaS lets developers create applications using built-in software components. Cloud features such as scalability, high-availability, and multi-tenant capability are included, reducing the amount of coding that developers must do.
- Analytics or business intelligence: Tools provided as a service with PaaS allow organizations to analyze and mine their data, finding insights and patterns and predicting outcomes to improve forecasting, product design decisions, investment returns, and other business decisions.

### Software as a Service
Software as a service (SaaS) is the most complete cloud service model from a product perspective. With SaaS, you’re essentially renting or using a fully developed application. 

Some common scenarios for SaaS are:

- Email and messaging.
- Business productivity applications.
- Finance and expense tracking.

