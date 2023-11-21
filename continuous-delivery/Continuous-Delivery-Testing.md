# Continuous Delivery - Testing

Testing is an integral part of how we validate the quality of the software solutions we build, but do you test in a way that aligns with green software practices, minimising the resources required to prove whether the code works?

For example, do you always run every integration/BDD test relating to the component or just the subset of tests relating to the area where you have made a change?

## The main ideas in this section

**Change aware**: Testing only what has changed means you don't waste resources testing what hasn't changed.

**NFR testing**: You should keep checking your NFRs while making your service more efficient. If you change to a new and better service level, how do we make sure our performance is still good enough?

**Benchmarking**: Sometimes tests are binary pass/fail and in other cases adding tolerances is more appropriate. Do you fail the build when any of your tests or static analysis for sustainability fail? Perhaps one issue is not enough to fail the build but what would you consider to be an acceptable level of green debt issues?

**Production Datasets**: You might get unexpected results if you don’t test with production data. How fast is your database search or your result calculation indexing? You might not notice big performance issues with a small dataset.

### For 1 point

**Change Aware**: We execute all tests on each code commit.

**NFR Testing**: Around major releases we do significant NFR testing e.g. system testing. But on each code change in-between, we don't really apply any.

**Benchmarking**: A test either passes or breaks the build.

**Production Datasets**: We don't regularly test with production datasets that replicate either the scale or variance of the data.

### For 3 points

**Change Aware**: We execute all tests relating only to the component which has been changed and its integrations.

**NFR Testing**: We regularly (at least once a sprint) undertake some form of scheduled NFR testing to review system performance and to test component resiliency.

**Benchmarking**: We have some rudimentary tolerance checks built in to break the build under certain conditions e.g. if static analysis has found more than 5 high priority green software actions that require fixing.

**Production Datasets**: We have some environments where we regularly test with production datasets to ensure that performance/behaviour remains consistent with test data.

### For 5 points

**Change Aware**: We execute all tests relating only to the feature which has been added/changed and its integrations.

**NFR Testing**: On each code change we are able to execute NFR testing relating to the feature or component that has been changed.

**Benchmarking**: We integrate the output of NFR testing to determine failure tolerances for new builds e.g. if performance degrades.

**Production Datasets**: We have on-demand environments where we can regularly test with production datasets to simulate production size, scale and variance.
