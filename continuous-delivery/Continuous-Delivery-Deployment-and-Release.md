# Continuous Delivery - Deployment and Release

When you design your system with more independent and flexible components, you can make smaller changes to each part. This helps you to improve your deployment process and reduce the environmental and hardware costs.

Also, when you have smaller changes to make, you can deliver better services to your users faster and safer, because you have less risk of breaking something.

## The main ideas in this section

**Reduce waste**: Two of the most important areas of digital hygiene that can have a huge impact are: 
1. Turning systems off which you aren't using 
2. removing systems, or parts of systems, that you no longer require

**Automation**: You use automation to make waste reduction easier e.g. turning off an environment overnight knowing you can quickly redeploy when it's required.

**Modularity**: When you have smaller parts to change, you can change them more easily. If your system is made of flexible and independent components, you can improve your green software practices without worrying about affecting other parts or causing failures.

### For 1 point

**Reduce waste**: Our environments tend to be long lived whether they are being actively used or not. Given how environments bloat over time, we will almost certainly find provisioned resources which aren't really needed.

**Automation**: We use little automation which means deployments can take a little time.

**Modularity**: We release everything relating to our service at the same time; so managing dependencies is not a problem. Our releases tend to be less frequent as a result of having to deploy everything.

### For 3 points

**Reduce waste**: We use concepts such as infrastructure as code to ensure unused resources get cleaned up over-time though generally speaking, our environments tend to be long-lived.

**Automation**: We use infrastructure as code automation in combination with configuration management to apply changes. Applying new code changes tends to be fully-automated.

**Modularity**: Many of our components are independent of each other so we can release these independently whenever we wish to make a change. We can release these components as often as we like though engaging with third-parties does slow this down.

### For 5 points

**Reduce waste**: Our environments tend to be short-lived and we provision them on-demand using Infrastructure as code.

**Automation**: We use infrastructure as code automation in combination with configuration management to rapidly build new environments and apply code-changes in an end-to-end manner.

**Modularity**: All of our components can be independently deployed and we utilise approaches like API versioning and we work with third-parties to streamline our integration when necessary.