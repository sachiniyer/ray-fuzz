# Ray Fuzz

The goal is to create a testing harness to fuzz the API of Ray with [AFL++](https://github.com/AFLplusplus/AFLplusplus). Specifically, we plan to use [persistent mode](https://github.com/AFLplusplus/AFLplusplus/blob/stable/instrumentation/README.persistent_mode.md). Additionally, we plan to utilize a grammar tailored to the [Ray API](https://docs.ray.io/en/latest/ray-core/api/core.html).

We will evaluate the performance of the harness based on:
- How many executions per second we reach with the harness
- How deep into the call stack we are reaching within ray


Btw, Ray is a bit weird in that it does not actually host any authentication (and expects isolation as stated [here](https://github.com/ray-project/ray/blob/master/doc/source/ray-security/index.md)).
