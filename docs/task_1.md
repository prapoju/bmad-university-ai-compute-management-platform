
- **Contract** — A precise statement of inputs, outputs, and behavior. State exact function/API signatures or interface boundaries, expected data shapes, and error-handling behavior. This section should read like something you could hand to another engineer with zero ambiguity about what "done" means.

- **Why** — One paragraph explaining the problem this solves and who benefits. Ground it in a real need, not a hypothetical.

The academic community from the university  needs to use hardware resources constatly.They use local LLMS to generate learning material. They also use computing power for specialized task, such as experiments or model training. This system is intended to allocate and provide strategies to limit the access of the resources based on the tasks requirements. 


- **Capabilities** — A bullet list of what the system will actually do, phrased as observable behaviors (not implementation details). Each capability should be testable.


1) Teachers, student and staff must be able to log and register in the platform by providing an email and a password.

2) The system must provide an interface to request services by their User. They can be 1) LLMS access, 2) Model training (LLM or Mathematical models) 3)Experiment variations in the outputs with fine tuning or paremeters 4) long jobs 5) distributed training,. All academic community has a quota of computing resources that resets weekly. The services that comes from personal quotas cant stop because the subject attach have a bigger priority. User must know the reasons why it cannot be use or why it sttoped.The access of the services dependes on their permises and roles. They schedule it

3) The teachers can make request to get computing resources. They must select the type of services (1, 2 or 3), the time interval the need it. ANd the number code the class.  THey system must provide feedback and inform the user is the request was possible to do or not. The request are processed in orde

4) Staff must be able to see CPU usage by user, by subject, general usage by time, token consumption, failures rate,

5) THe staff must be able to restrict the acces of models, change quotas, and computing power, and services type. Having groups and permises

6) Users must see the status of the workload and usage ajaj.

7) Cancel a request. ANy request can be cancelled




- **Constraints** — Technical, business, or resource limits that shape the solution: performance budgets, language/framework requirements, security rules, timeline, or dependency restrictions.

- The system balance the resource usage in context of heterogeneous hardware
- It must use kubernetes


- **Non-Goals** — Explicit statements of what is intentionally out of scope. This is the section that skips the novice spec-writers, and the one that prevents scope creep and agent hallucination during implementation.

- Make projections about usage 
- make recomendations about scale
- Must not give access to VMs they are restricted to the named services. Creating new services will require manual coding.
- THe system doesn't garantee that all the requests are satisfied, but it will do its best effort.
- Keep track of the usage of LLMS. How good are they doing or measure how good they are using it.

- **Success Signal** — Concrete, measurable criteria for knowing the task is complete: specific tests passing, a metric threshold, a user-observable outcome. Avoid vague statements like "works well."



- **Assumptions** — Anything you're taking for granted (environment, data availability, upstream services, user behavior) that, if false, would break the spec. Flag which assumptions are risky vs. safe.

- It is expected that if there are no resources available the system will give priority to the academic context. Aside from that the priority depends on the order. There are no subject whose value is greater than others.

- We don't want to invade the privacy and see the specific usage of LLMS. We want to respect the students.




