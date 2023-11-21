# Continuous Delivery - Operations

Feedback from ongoing operations and monitoring data can be used to identify trends to continuously improve and optimise your service.

For example, understanding that a trends follows a specific cycle, for example a season, or that most of your users access the service from a specific region may impact some of the decisions you make around ongoing operations.

## The main ideas in this section

**Patching**: Software is regularly updated to make performance improvements. You regularly patch your software to ensure you are running the latest versions. This gives you the benefit of those improvements.

**Feature toggling**: Being able to dynamically control/toggle features within your application provides opportunities to optimise for certain scenarios.

### For 1 point

**Patching**: We apply urgent security updates when they are available.
**Feature Toggling**: We don't make use of this. Turning something off would necessitate a code change.

### For 3 points

**Patching**: We apply security updates when they are available and consider patching/upgrading other components when new features touch those components.
**Feature Toggling**: We can toggle certain software features on or off to reduce the environmental impact of our software.

### For 5 points

**Patching**: We regularly patch and upgrade all software underpinning the service.
**Feature Toggling**: We automatically toggle certain software features on or off to reduce the environmental impact of our software based on external parameters.