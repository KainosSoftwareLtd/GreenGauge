# Architecture - Compute

You have many options to improve compute efficiency.

Depending on your workload, you can choose the best form of compute to boost performance and minimise impact.

Some ways to do this are: using more parallel processes, speeding up computation with GPUs, or switching to ARM-based systems that may use less energy. You can also start with the simple step of adjusting your infrastructure to fit your needs.

## The main ideas in this section

**Hardware efficiency**: Choosing the optimal instruction set or hardware capabilities relative to your workload can improve efficiency; don't just default to x86 everytime.

**Choosing the correct size**: Choosing the service family and tier of your service that best suits its performance needs. You should aim to use your resources efficiently and avoid wasting them. You need to find the optimal balance between the two and reducing unnecessary or low-use resources.

**Async Patterns**: Don't default to microservices and always consider the optimal architecture relative to your workload. Where possible you should prioritise event-driven patterns as they enable 'scale to zero' use-cases which negate some of the need for overlapping controls like intelligent scheduling.

**Intelligent scheduling**: The ability to schedule compute resources to be available only when needed or to execute based on the availability of low-carbon energy sources e.g. running a batch job when the energy mix within a region favours renewable power.

### For 1 point

**Hardware Efficiency**: Our default is x86 and we haven't needed to look at anything else.

**Choosing the correct size**: We plan capacity in advance and always build some room for growth into our solution.

**Async Patterns**: We deploy long-lived services  e.g. microservices.

**Intelligent Scheduling**: Our services remain running all the time, though sometimes we turn some environments off to save money.

### For 3 points

**Hardware Efficiency**: Most workloads align with our default of x86, though we do make use of GPU/ARM  for specific workloads.

**Choosing the right size**: We continuously adjust the size of our infrastructure centrally based on cloud provider recommendations e.g. Azure Advisor.

**Async Patterns**: Whilst we mostly deploy long-lived services  e.g. microservices we also make use of event-driven architectures.

**Intelligent Scheduling**: We have automated scheduling to turn things off when they aren't used to save resources."

### For 5 points

**Hardware Efficiency**: We have no default. We actively require consideration alternative instruction sets to boost performance.

**Choosing the right size**: Our teams are encouraged and rewarded for using the right size for their infrastructure.

**Async Patterns**: Event-driven architectures are preferred and actively considered for all new service delivery.

**Intelligent Scheduling**: We schedule our workloads based on the availability of low-carbon energy sources.