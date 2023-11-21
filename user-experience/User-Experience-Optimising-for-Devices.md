# User Experience - Optimising for Devices

By designing and optimising for the devices that will use our service, we can lower the energy consumption and extend the hardware lifecycles.

For example, when designing for low-powered or older devices, you might choose to turn off features that may use a lot of power.

## The main ideas in this section

**Device Optimisation**: The more you can tailor your software to a specific device, the more chances you will have to overcome its limitations and prevent it from becoming obsolete.

**App delivery model**: How do you get your software into the hands of your end users e.g. native app or website

### For 1 point

**Device optimisation**: We focus on browser compatibility for only the most modern web browsers. We don't worry about devices and use abstractions to avoid this pain.

**App delivery model**: We do not target specific device capabilities and simply develop generic web-services which we know can be widely consumed across platforms.

### For 3 points

**Device optimisation**: Beyond testing web browser compatibility, we do test across a range of devices to ensure backwards compatibility. We actively profile how our service is consumed on those devices and optimise for reduced energy consumption.

**App delivery Model**: Depending on the device, we try to make a native option for a user to consume our service. Doing this allows us to better use device capabilities like energy saving modes and background refreshes.

### For 5 points

**Device optimisation**: We have explicitly profiled and optimised for consumption by the most-used devices. We may even link this to the energy efficient defaults mentioned previously e.g. understanding what colour themes work best to save energy on different smartphones relative to display technology.

**App delivery Model**: Where possible, we provide native mechanisms to consume our service so we can use the native capabilities of devices e.g. making use of GPU acceleration where it will reduce processing time and energy consumption.
