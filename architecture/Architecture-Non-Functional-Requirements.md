# Architecture - Non-functional Requirements

Defining the capabilities and constraints of the services we build, non-functional requirements can greatly impact how efficient our solutions can be.

For example, meeting a 99% vs a 99.9% availability target can dramatically increase environment impact owing to the additional infrastructure required to support this.

Challenging assumptions behind non-functional requirements is one of the quickest ways to identify quick wins with the business e.g. do you really need access to the service on weekends?.

## The main ideas in this section

**Service Availability**: Do you really need such a high availability target?

**Performance**: What is tolerable/noticeable to users vs arbitrary targets?

**Backup**: Do you need to backup everything? Dp you need to replicate your backups across multiple different locations?

**AI Model Accuracy**: How much is 'good enough' vs striving for perfect?

**Sustainability NFRs**: To augment the existing NFRs

### For 1 point

**Service Availability**: We have a really ambitious target set by the business because our service is so important.

**Performance**: Performance targets are set by the architects based on their experience.

**Backup**: We tend to back everything up so we can quickly recover the service and we may have multiple copies of each backup.

**AI Model Accuracy**: We tend to use the most accurate models because they give the best results.

**Sustainability NFRs**: We don't have any explicitly around this

### For 3 points

**Service Availability**: We have a really ambitious target set by the business that we've challenged.

**Performance**: Performance targets are set by the architects based on their experience and are actively tested through automation.

**Backup**: We tend to backup all application data so we can quickly recover the service.

**AI Model Accuracy**: We trade-off model accuracy vs performance/resource usage when a new service is created.

**Sustainability NFRs**: We have established some proxies for sustainability in our existing NFRs.

### For 5 points

**Service Availability**: We have a really ambitious target set by the business that we've challenged and successfully reduced or put mitigations in place to offset.

**Performance**: Performance targets are informed through user feedback using production telemetry and are actively tested through automation.

**Backup**: We only backup business critical data.

**AI Model Accuracy**: We proactively trade-off model accuracy vs performance/resource usage through the lifecycle of a service e.g. as a better/new/more-efficient model becomes available we switch to it.

**Sustainability NFRs**: We have an explicit set of sustainability focused NFRs.
