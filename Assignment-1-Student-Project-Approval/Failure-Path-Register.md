# Failure Path Register

| ID | Failure Point | Cause / Trigger | BPMN Solution |
|---|---|---|---|
| F1 | Proposal validation failure | Missing or invalid information | Return proposal for correction using an exclusive gateway and bounded correction loop |
| F2 | Invalid team | Team composition violates project rules | Reject validation and request team correction |
| F3 | Duplicate / similar topic | Proposed topic is too similar to an existing project | Coordinator reviews the similarity result and requests modification or rejection |
| F4 | Submission deadline missed | Proposal is not submitted within the allowed period | Timer event triggers late-submission handling |
| F5 | Revision required | Committee identifies scope, feasibility, or clarity issues | Return proposal for revision with a bounded revision loop |
| F6 | Proposal rejected | Committee determines that the project is unsuitable | Send rejection outcome and allow the defined new-topic path |
| F7 | Committee review delayed | Review is not completed within the expected time | Timer event triggers reminder and escalation |
| F8 | No suitable guide available | No matching guide has sufficient availability | Continue through alternative/manual allocation handling |
| F9 | Guide declines or does not respond | Guide rejects the request or response deadline expires | Event-based response handling followed by another allocation attempt |
| F10 | System / notification failure | Technical failure while recording or notifying | Error handling and retry/manual notification path |
| F11 | Withdrawal after approval | Student/team withdraws after allocation | Message-triggered withdrawal handling and compensation/reallocation |
| F12 | Guide double-booking prevention | Guide allocation conflicts with another project | Workload/availability validation prevents conflicting allocation |
