# Architecture maturity

This pillar of the maturity model covers ....

* [Principles](#Principles)
* [Design](#Design)
* [Storage](#Storage)
* [Compute](#Compute)
* [Networking](#Networking)
* [Non-functional requirements](#Non-functional-requirements)
* [Governance](#Governance)
* [Scalability](#Scalability)
* [Development](#Development)

### Principles
The way you design, build and operate software is influenced by your architecture principles and approach.
The following factors can affect how much carbon your software emits:<ul><li>using public cloud services</li><li>choosing managed services</li><li>adopting a certain architecture style</li></ul> 

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Green Software Principles** | Considering how to save energy, use hardware effectively and be aware of carbon emissions.| The organisation is partially aware of the principles but they are not being yet applied. | The organisation has defined clear principles though is is not clear how well this has cascaded across the organisation. | Clear principles defined with clear adoption across the organisation. |
| **Cloud selection guidance** | Defining the preference by which cloud service offerings are considered in declining order of importance: SaaS->PaaS->IaaS. | People are free to select what they think is right and works best for them.| Preference is given the PaaS and provider managed offerings over bespoke. | Preference is given the SaaS solutions with IaaS being the least preferred. |

### Design  
Design your software with energy and hardware efficiency in mind.This helps to optimise carbon impact both now and in the future.Adopt modular, decoupled architectures to enable targeted changes or quick improvements.

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Architecture Guidance** | How do you assist people in architecting solutions aligned to green software principles? Do golden paths exist? |People draw on their own experience and what they can find on the internet to design what they think is right. | Guidance exists for how to deploy commonly utilised components in an energy/hardware efficient manner e.g. 12-factor apps.| There are guidelines based on scenarios that show the best way and the ideal steps to achieve results in a way that saves energy and hardware. |
| **Pattern Library** | Where can people discover previously implemented patterns or versions of good for solutions aligned with green software principles? | Patterns are shared across informal employee networks | Patterns are stored/maintained by the architecture community. | A pattern library is actively contributed to and maintained across the organisation. |

### Storage 
The way you classify, store, and access your data is important.Adjust service levels to match the data access profile and make sure you only backup data that is essential for your business.The less data you store, the less impact you have. Thinking of data as limited and not infinite, is the attitude we should have.

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **RRD** | To combat the risk of ever growing data, a robust **review, retention and disposal** policy is required. How well is this implemented/adopted across your business today? Does this apply to all data types? What about monitoring data, log data or audit data? | We have no RRD policy in place, our data volumes tend to grow and data is removed only on an ad-hoc basis. | RRD policy is defined and proactively applied to new services being built. | RRD policy is defined and proactively applied to new and existing services. |
| **Storage profiling** | We use the most appropriate type of storage required and don't just always default to the fastest available. | We tend to use the fast storage as it will always meet our needs. | We use tiered storage to move less frequently accessed storage to slower (and cheaper) mediums. | We use tiered storage to dynamically move data across different mediums and match storage performance profiles to non-functional requirements. |
| **Compression** | Do you always make of this feature when available? | We turn it on when the service offering makes a compression feature available. | We embed data compression into our solutions to ensure all data in transit is compressed. | We embed data compression into our solutions to ensure all data in transit and at rest is compressed. |

### Compute
You should choose the best form of compute to boost performance and minimise impact for your workload. Some ways to do this are: using more parallel processes, speeding up computation with GPUs, or switching to ARM-based systems that may use less energy. You can also start with the simple step of adjusting your infrastructure to fit your needs.  

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Hardware efficiency** | Choosing the optimal instruction set or hardware capabilities relative to your workload can improve efficiency; don't just default to x86 everytime. | Our default is x86 and we haven't needed to look at anything else. | Most workloads align with our default of x86, though we do make use of GPU/ARM for specific workloads. | We have no default. We actively require consideration alternative instruction sets to boost performance. |
| **Choosing the correct size** | Choosing the service family and tier of your service that best suits its performance needs. You should aim to use your resources efficiently and avoid wasting them. You need to find the optimal balance between the two and reducing unnecessary or low-use resources. | We plan capacity in advance and always build some room for growth into our solution. | We continuously adjust the size of our infrastructure centrally based on cloud provider recommendations for example, from Azure Advisor. | Our teams are encouraged and rewarded for using the right size for their infrastructure. |
| **Async Patterns** | Don't default to microservices and always consider the optimal architecture relative to your workload. Where possible you should prioritise event-driven patterns as they enable 'scale to zero' use-cases which negate some of the need for overlapping controls like intelligent scheduling. | We deploy long-lived services such as microservices. | Whilst we mostly deploy long-lived services such as microservices we also make use of event-driven architectures. | Event-driven architectures are preferred and actively considered for all new service delivery. |
| **Intelligent scheduling** | The ability to schedule compute resources to be available only when needed or to execute based on the availability of low-carbon energy sources e.g. running a batch job when the energy mix within a region favours renewable power. | Our services remain running all the time, though sometimes we turn some environments off to save money. | We have automated scheduling to turn things off when they aren't used to save resources. | We schedule our workloads based on the availability of low-carbon energy sources. |

### Networking
Optimise data transmission between software components to significantly influence efficiency and energy use. For example, the shorter the distance and fewer the components, the less the impact. Explore the use of things like GraphQL to reduce transmission of unneeded data or leverage content-delivery networks to deliver services closer to your end user.                                                                                                                      

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |                                                                                                                                  
| **Number of Requests** | Each request has an overhead including the TLS handshake; the more that can be done to reduce the number of requests in addition to payload size can improve energy efficiency. | We are aware of how many requests are made but we don't make many efforts to reduce them. | Aware of how many requests are made and some efforts to optimise the number. | We have actively adjusted our architecture to reduce the number of requests and data transmitted e.g. adoption of GraphQL. |
| **Bandwidth** | Minimising data transmission through use of compression and service optimisation to reduce unneeded data exchange. | We are aware of bandwidth cost but we don't make many efforts to reduce it. | Aware of bandwidth cost and turning on compression where possible to reduce volume. | Active efforts to prioritise and reduce things like page weights. |
| **Local POP** | The more proximate the service to consumers, the lesser the transmission distance and energy costs. | Services delivered centrally for everyone. |  Most services delivered centrally but we make use of a CDN for commonly accessed assets. | We make use of a CDN and prioritise efforts to reduce things like server response time. |
| **Edge** | How can you minimise data transmission through pre-processing? | We transmit the raw data to be processed centrally. | We try to clean-up the raw data on the users device prior to transmitting centrally. | We clean-up the data on the users device and at each transmission hop to minimise onward transmission costs. |

### Non-functional requirements
Non-functional requirements can greatly impact how efficient our solutions can be. For example, meeting a 99% vs a 99.9% availability target can dramatically increase environment impact owing to the additional infrastructure required to support this. Challenging assumptions behind non-functional requirements is one of the quickest ways to identify quick wins with the business, for example, do you really need access to the service on weekends? 

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Service Availability** | Do you really need such a high availability target? | We have a really ambitious target set by the business because our service is so important. | We have a really ambitious target set by the business that we've challenged. | We have a really ambitious target set by the business that we've challenged and successfully reduced or put mitigations in place to offset. |
| **Performance** | What is tolerable/noticeable to users vs arbitrary targets? | Performance targets are set by the architects based on their experience. | Performance targets are set by the architects based on their experience and are actively tested through automation. | Performance targets are informed through user feedback using production telemetry and are actively tested through automation. |
| **Backup** | Do you need to backup everything? Dp you need to replicate your backups across multiple different locations? | We tend to back everything up so we can quickly recover the service and we may have multiple copies of each backup. | We tend to backup all application data so we can quickly recover the service. | We only backup business critical data. |
| **AI Model Accuracy** | How much is 'good enough' compared with striving for perfect? | We tend to use the most accurate models because they give the best results. | We trade-off model accuracy against performance and resource usage when a new service is created. | We proactively trade-off model accuracy vs performance/resource usage through the lifecycle of a service e.g. as a better/new/more-efficient model becomes available we switch to it. |
| **Sustainability NFRs** | To augment the existing NFRs | We don't have any explicit sustainability requirememts defined | We have established some proxies for sustainability in our existing NFRs. | We have an explicit set of sustainability focused NFRs. |

### Governance
The way technology governance guides architecture and technology principles can have a big influence on how things are done and what results are achieved. For instance, not only should you have some green software principles, but they need to be implemented and monitored by a green software governance framework.  

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Decision Making** | What rules and processes do you use for making technology choices? | We decide based on each situation and with the input of our peers. We try our best, but the views are subjective of the people involved. | New service delivery and change controls require consideration of carbon/environmental impact and the risks involved. | We use a strict method for delivering new services and making changes that requires us to base our decisions on data. |
| **Evaluation** | Which weighting do you apply to sustainability functional and non-functional requirements when making decisions? Do you apply a stronger weighting for vendors whom report on their own carbon impact and less for those that don't? | Some consideration given to alternative options but these can prioritise functional rather than non-functional fit. | Consideration of alternatives spans functional and non-functional concerns. | Consideration of alternatives spans functional and non-functional concerns with a clear framework in place. |

### Scalability
Increasing or decreasing capacity gracefully relative to demand is one of the key challenges of modern technology platforms which often offer consumption based pricing. Ultimately, when there is no-demand you'll want to scale in/down as you want to minimise resource usage and cost when there is no demand. Using event-driven architectures you can do just this with ‘scale to zero’ patterns.  

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Scaling Approach** | Scaling is not a one size fits all; scaling on demand based on custom metrics is normally more efficient than scheduling services to scale during fixed windows. | We either don't scale or schedule it in advance based on known seasonality. | We are able to quickly scale based on observed metrics such as CPU or Memory utilisation to minimise wasted resources. | We are able to quickly scale based on workload specific metrics, such as active users or request count to minimise wasted resources. |
| **Carbon Shifting** | Determining in which locations you scale or the intelligent shifting of workloads based on the availability of lower carbon energy sources.| We don't do this, we tend to operate in one region. | Whilst we have multiple regions we tend to site services based on factors other than local carbon intensity e.g. compliance with local laws. | We have multiple regions and actively shift/balance workloads in favour of the prevailing carbon intensity within those regions. |
| **Caching** | Caching should be embedded through the application stack to reduce unnecessary requests and demands being placed on the system. | We do the basics like in-memory caching and utilising local storage for caching frontend static assets like images. | Beyond local caching we make use of content delivery networks to distribute status assets from local points of presence (POP) minimising the network roundtrip and latency. | We make use of application level caching. |
| **Utilisation** | Utilisation, in this context, is indicative of energy proportionality; it is the relationship between power consumed by a device and the rate at which useful work is done. You should aim for high utilisation for your systems to be the most efficient. | We design our workloads to accommodate expected peaks in demand with sufficient capacity to safely weather this. Outside of peaks we can have low-rates of utilisation. | We try to achieve maximum utilisation by dynamically scaling to meet demand. We do keep some flex capacity in the system to accommodate for scale-out time/delays. | We design our workloads maximise utilisation by dynamically scaling to meet demand. We optimise our systems for rapid scaling to minimise the need for extra capacity. |

### Development
The environmental impact of our software depends on how we choose to develop it throughout all its different stages. For example, if our development approach requires each developer to have a new, high-specification device to create a development environment or troubleshoot problems locally, our impact can be much greater than if using cloud development environments.  

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Language** | Choice of programming language can impact upon energy efficiency with some studies showing that interpreted languages, such as Python, are significantly more impactful than compiled languages, such as C. | You have a default language that you always use when building a new service. | You have several preferred languages and you pick the best of these relative to your teams capability and the problem domain. | You pick the most efficient language relative to the problem domain. Libraries are regularly assessed for against performance impact |
| **Developer environments** | How well can your developers test/validate changes on their local machines prior to committing code? The sooner they can fail and the more easily they can do this without requiring high-powered workstations the better. | Depending on the resources of your local workstation, you may be able to create a representative test environment validate changes locally. | Clear processes supporting developers validating changes in locally provisioned test environments prior to committing code. This requires developers to have a high specification laptop. | Developers can validate changes they are making using 'just-in-time' cloud workstations and personal environments. |
| **Build environments** | How best can we catch failure at the earliest possible point to fail a build? | All changes are built and progressed through long-lived test environments until a release is ready or a failure is noted. | All changes are built and progressed through short-lived on-demand test environments. | All changes are built and progressed through short-lived on-demand test environments which are created on-demand, functionaly matching production and scaled up as required. Test tolerances actively break the build where quality thresholds are not met. |
