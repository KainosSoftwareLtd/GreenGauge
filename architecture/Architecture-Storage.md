# Architecture - Storage

The way you classify, store, and access your data is important.

Adjust service levels to match the data access profile and make sure you only backup data that is essential for your business.

The less data you store, the less impact you have. Thinking of data as limited and not infinite, is the attitude we should have.

## The main ideas in this section

**RRD**: To combat the risk of ever growing data, a robust **review, retention and disposal** policy is required. How well is this implemented/adopted across your business today? Does this apply to all data types? What about monitoring data, log data or audit data?

**Storage profiling**: We align the performance profile of the workload to the capabilities of storage and don't just always default to the fastest available.

**Compression**: Do you always make of this feature when available?

### For 1 point

**RRD**: No active RRD policy is in place, data volumes tend to consistently grow and any removal is adhoc based on project needs.

**Storage profiling**: We tend to use the fast storage as it will always meet our needs.

**Compression**: We turn it on when the service offering makes a compression feature available.

### For 3 points

**RRD**: RRD policy is defined and proactively applied to new services being built..

**Storage profiling**: We utilise tiered storage to move less frequently accessed storage to slower (and cheaper) mediums.

**Compression**: We embed data compression into our solutions to ensure all data in transit is encrypted.

### For 5 points

**RRD**: RRD policy is defined and proactively applied to new/existing services.

**Storage profiling**: We utilise tiered storage to dynamically move data across different mediums and match storage performance profiles to non-functional requirements.
**Compression**: We embed data compression into our solutions to ensure all data in transit and at rest is encrypted.
