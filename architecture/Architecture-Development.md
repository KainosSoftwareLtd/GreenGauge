# Architecture - Development

The environmental impact of our software depends on how we choose to develop it throughout all its different stages.
For example, if our development approach requires each developer to have a new, high-specification device to create a development environment or troubleshoot problems locally, our impact can be much greater than if leveraging cloud development environments.

## The main ideas in this section

**Language**: Choice of programming language can impact upon energy efficiency with some studies showing that interpreted languages, such as Python, are significantly more impactful than compiled languages, such as C.

**Developer environments**: How well can your developers test/validate changes on their local machines prior to committing code? The sooner they can fail and the more easily they can do this without requiring high-powered workstations the better.

**Build environments**: How best can we catch failure at the earliest possible point to fail a build?

### For 1 point

**Language**: You have a default language that you always use when building a new service.

**Developer Environments**: Depending on the resources of your local workstation, you may be able to create a representative test environment validate changes locally.

**Build Environments**: All changes are built and progressed through long-lived test environments until a release is ready or a failure is noted."

### For 3 points

**Language**: You have several preferred languages and you pick the best of these relative to your teams capability and the problem domain.

**Developer environments**: Clear processes supporting developers validating changes in locally provisioned test environments prior to committing code. This requires developers to have a high specification laptop.

**Build environments**: All changes are built and progressed through short-lived on-demand test environments.

### For 5 points

**Language**: You pick the most efficient language relative to the problem domain.

**Developer environments**: Developers can validate changes they are making using 'just-in-time' cloud workstations and personal environments.

**Build environments**: All changes are built and progressed through short-lived on-demand test environments which are created on-demand. Test tolerances actively break the build where quality thresholds are not met.
