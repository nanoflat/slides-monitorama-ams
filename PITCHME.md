# Monitorama Amsterdam  

---
#### What I learned about myself:
@snap[west]
conference =  new knowledge
@snapend
new knowledge = @snap[east splitscreen fragment]
![Reward](https://www.leafscience.com/wp-content/uploads/2014/05/marijuana-and-dopamine-2.jpg) 
@snapend

SRSL: go to conferences. Best - go where you are not expert.

--- 
Notes and hihlights from conference

---

Best talk - CTO

---
Best graphics - ai for graphite
---

Main takeaway:

https://photos.google.com/photo/AF1QipMr4Tmd1sBDwwaD2EwbgVSHR3463cFsnQ0qqO0I


### Main highlights

- Alert in urgent cases
- Invest in tooling (does not mean we need to write everyting from scratch​)
- Avoid false alerts at any costs​ 
- Allert right person: (if db is dead, do not allert frontend)​
- Start building alerts from SLA, rest is telemetry​
- Things will break and our jobs are problems solvers​
- Keep learning on failures, even it's hard​
- Stay positive 
- Eat, sleep, $INTERESTING_THINGS, repeat​
- Involve everyone​
    - Monitoring owned by a team, SRE/DevOps to support​
    - 100% permissions by default, degrade in case of misuse​
    - Weekly meetings of teams​
- Share knowledge, share responsibility, encourage ownership
- Change phase is fast and will never be as slow again
---
What to monitor​
Monitor things that you don't know:​

Check that things that you expect to happen - doesn’t' happen

[image of plane with bullets]

---
Lambda monitoring:
- Lambda->CW (which is Kinesis underneath) -> Kinesis(10 shards) ->lambda->DD​
- CW log retention (store for 10 days)​
- Middlewares for lambdas are way to go https://github.com/middyjs/middy ​
- We need to opensource them asap – a lot of ppl working on them already​
- Real-time controlled log levels without redeploys
- Capture errors of lambdas to use as test invocatios for debugging
---
DD Postmortems
[photos] 
---
Adobe alerting pipeline
---
kubernetes meetup


---
Monitoring Serverless Things
Mandy Waite

serverless - ability to run work in clouds based on events

everyone talking about new infra is for developers. Servelrss for developers.
Scale - right amount of scale
managed, no worries
GCF had outage today
pay per use

serverless is more then functions

FaaS

Who ensures reliability
cloud-provider and you, but goals are not shared

microservicies - more stuff to monitor

autoscaling
coldstarts

events are hard to trace

Assume that everything will fail

functions: at most once (http) and at least once (background functions)

make functions idempotent

no real tracing in GC

---
How AI Helps Observe Decentralised Systems
Dominic Wellington

Monitoring != observability

a lot of isuues escaleted because noone knows how things works

[best chanel of notification of incidents - shouts and screams]

[survivor bias, bullet plain] 

wrong assumptions

Dashboards:
internal health is irelevevant
dashboard is artifact of past failure

Observability:
Huge streams, instrumented, insights-driven

information is cheep, valuable if queried

30% incidents are requring, 70% happens for a first time

AI OPS
---
Incremental-decremental Methods For Real-Time Monitoring
Joe Ross

---

