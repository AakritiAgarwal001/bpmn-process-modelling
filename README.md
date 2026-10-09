# BPMN Process Modelling

BPMN 2.0 process models focusing on business workflows, decision
points, exception handling, and failure-path modelling.

## Included Process Models

### 1. Student Project Approval & Allocation

Models the workflow for student project proposal submission,
validation, committee approval, and faculty-guide allocation.

Key BPMN concepts include:

- User and Service Tasks
- Exclusive and Parallel Gateways
- Event-Based Gateway
- Timer Events
- Error Boundary Events
- Escalation
- Compensation
- Bounded correction and revision loops

[View Assignment 1](Assignment-1-Student-Project-Approval/)

### 2. Loan Origination & Approval

Models a loan application workflow from document submission and
verification through risk assessment, underwriting, approval,
e-signature, and disbursement.

Key BPMN concepts include:

- User and Service Tasks
- Exclusive, Parallel, and Inclusive Gateways
- External Participant Pools
- Timer Events
- Error Boundary Events
- Event Sub-processes
- Compensation
- Exception and escalation handling

[View Assignment 3](Assignment-3-Loan-Origination/)

## BPMN Modelling Focus

The models emphasize:

- Happy-path process modelling
- Identification of failure and exception paths
- Appropriate BPMN task types
- Gateway-based decision making
- Timer-based escalation and expiry
- Error handling
- Compensation and recovery
- Loops for correction and rework
- Clear separation of process participants

## Tool

The BPMN models were created using **Camunda Modeler**.

## Repository Structure

```text
bpmn-process-modelling/
│
├── Assignment-1-Student-Project-Approval/
│   ├── README.md
│   ├── student-project-approval.bpmn
│   └── Failure-Path-Register.md
│
└── Assignment-3-Loan-Origination/
    ├── README.md
    ├── loan-origination.bpmn
    └── Failure-Path-Register.md
