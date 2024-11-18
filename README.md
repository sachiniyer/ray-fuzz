# Ray Fuzz

The goal is to create a testing harness to fuzz the API of Ray with [AFL++](https://github.com/AFLplusplus/AFLplusplus). Specifically, we plan to use [persistent mode](https://github.com/AFLplusplus/AFLplusplus/blob/stable/instrumentation/README.persistent_mode.md). Additionally, we plan to utilize a grammar tailored to the [Ray API](https://docs.ray.io/en/latest/ray-core/api/core.html).

We will evaluate the performance of the harness based on:
- How many executions per second we reach with the harness
- How deep into the call stack we are reaching within ray
