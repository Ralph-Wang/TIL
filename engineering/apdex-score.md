# Apdex Score

Apdex Score is a metric to measure user satisfaction about a service at the response time.

We only defined a time T that when the response is less than T, the customer will be satisfied.

Then we can use T to get other level which is called Apdex Level:

|level|Time|
|Satisfied| RT <= T |
|Tolerated| T < RT <= 4T |
|Frustrated| RT > 4T |


For lots of requests, they must be located in one of these levels. We can suppose there are *Sa, To, Fr* of each level.
So the Apdex Score can be caculated by:

```
Score = (Sa + (To / 2)) / (Sa + To + Fr)
```


Refer to: https://docs.newrelic.com/docs/apm/new-relic-apm/apdex/apdex-measure-user-satisfaction
