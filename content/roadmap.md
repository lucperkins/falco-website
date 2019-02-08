---
title: The Falco roadmap
---


Here's a sketch of the features we're planning on adding to Falco in the next several releases. When relevant, we've included links to the relevant github issues. Afterward, we'll list the specific features we're planning on adding in the next Falco relase (0.7.0). Of course, plans may change, but this should give you an idea of what's on the roadmap for Falco. If you see specific features you're especially excited for, or if you have features that you'd like to see that aren't on this list, let us know!

## Overall Roadmap

### Rule Improvements

Improvement | Pull request
:-----------|:------------
Bring back rulesets devoted to specific applications like apache, cassandra, etc. We originally commented these out as enabling them all slowed down falco too much, but we probably have more headroom now that rules are initially filtered by event type. Also if we add rule triggers they will only be enabled when the process is running. | [#183](https://github.com/draios/falco/issues/183)
Add rules that implement as much of the CIS Docker benchmark as possible in falco. | [#186](https://github.com/draios/falco/issues/186)

### Rule Mechanics Improvements

Improvement | Pull request
:-----------|:------------
Rule triggers--load/unload sets of rules based on other rules firing. This allows gateways based on processes starting/stopping. | [#149](https://github.com/draios/falco/issues/149)

### New measurement capabilities

Improvement | Pull request
:-----------|:------------
Have the trigger for a rule be meta-information like resource usage instead of a specific action. | [#167](https://github.com/draios/falco/issues/167)
Flight data recorder--when a rule triggers, save the last N events to a trace file. | [#81](https://github.com/draios/falco/issues/81)

## 0.14.0 Planned Features

* Add rulesets that provide support for specific applications packaged as containers.
* Add rules that implement as much of the CIS Docker benchmark as possible in falco.
