# Architecture - Scalability

Increasing or decreasing capacity gracefully relative to demand is one of the key challenges of modern technology platforms which often offer consumption based pricing.

Ultimately, when there is no-demand you'll want to scale in/down as you want to minimise resource usage and cost when there is no demand.

Using event-driven architectures you can do just this with ‘scale to zero’ patterns.

## The main ideas in this section

**Scaling Approach**: Scaling is not a one size fits all; scaling on demand based on custom metrics is normally more efficient than scheduling services to scale during fixed windows.

**Carbon Shifting**: Determining in which locations you scale or the intelligent shifting of workloads based on the availability of lower carbon energy sources.

**Caching**: Caching should be embedded through the application stack to reduce unnecessary requests and demands being placed on the system.

**Utilisation**: Utilisation, in this context, is indicative of energy proportionality; it is the relationship between power consumed by a device and the rate at which useful work is done. You should aim for high utilisation for your systems to be the most efficient.

### For 1 point

**Scaling Approach**: We either don't scale or schedule it in advance based on known seasonality.

**Carbon Shifting**: We don't do this, we tend to operate in one region.

**Caching**: We do the basics like in-memory caching and utilising local storage for caching frontend static assets like images.

**Utilisation**: We design our workloads to accommodate expected peaks in demand with sufficient capacity to safely weather this. Outside of peaks we can have low-rates of utilisation.

### For 3 points

**Scaling Approach**: We are able to quickly scale based on observed demand to minimise wasted resources.

**Carbon Shifting**: Whilst we have multiple regions we tend to site services based on factors other than local carbon intensity e.g. compliance with local laws.

**Caching**: Beyond local caching we make use of content delivery networks to distribute status assets from local points of presence (POP) minimising the network roundtrip and latency.

**Utilisation**: We try to achieve maximum utilisation by dynamically scaling to meet demand. We do keep some flex capacity in the system to accommodate for scale-out time/delays.

### For 5 points

**Scaling Approach**: We are able to quickly scale based on observed demand to minimise wasted resources.

**Carbon Shifting**: We have multiple regions and actively shift/balance workloads in favour of the prevailing carbon intensity within those regions.

**Caching**: We make use of application level caching

**Utilisation**: We design our workloads maximise utilisation by dynamically scaling to meet demand. We optimise our systems for rapid scaling to minimise the need for extra capacity.