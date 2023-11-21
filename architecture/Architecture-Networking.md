# Architecture - Networking

Optimise data transmission between software components to significantly influence efficiency and energy use. For example, the shorter the distance and fewer the components, the less the impact.

Explore the use of things like GraphQL to reduce transmission of unneeded data or leverage content-delivery networks to deliver services closer to your end user.

## The main ideas in this section

**Number of Requests**: Each request has an overhead including the TLS handshake; the more that can be done to reduce the number of requests in addition to payload size can improve energy efficiency.

**Bandwidth**: Minimising data transmission through use of compression and service optimisation to reduce unneeded data exchange.

**Local POP**: The more proximate the service to consumers, the lesser the transmission distance and energy costs.

**Edge**: How can you minimise data transmission through pre-processing?

### For 1 point

**Number of Requests**: Aware of how many requests are made but little efforts to reduce.

**Bandwidth**: Aware of bandwidth cost but little efforts to reduce.

**Local POP**: Services delivered centrally for everyone

**Edge**: We transmit the raw data to be processed centrally.

### For 3 points

**Number of Requests**: Aware of how many requests are made and some efforts to optimise the number.

**Bandwidth**: Aware of bandwidth cost and turning on compression where possible to reduce volume.

**Local POP**: Most services delivered centrally but we make use of a CDN for commonly accessed assets.

**Edge**: We try to clean-up the raw data on the users device prior to transmitting centrally.

### For 5 points

**Number of Requests**: We have actively adjusted our architecture to reduce the number of requests and data transmitted e.g. adoption of GraphQL.

**Bandwidth**: Active efforts to prioritise and reduce things like page weights.

**Local POP**: We make use of a CDN and prioritise efforts to reduce things like server response time/time-to-interactive..

**Edge**: We clean-up the data on the users device and at each transmission hop to minimise onward transmission costs.