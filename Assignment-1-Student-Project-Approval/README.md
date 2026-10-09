# Assignment 1 – Student Project Approval & Allocation

## Overview

This BPMN 2.0 process models the approval and allocation workflow for
student project proposals.

The process covers proposal submission, validation, coordinator
screening, committee evaluation, faculty-guide allocation, and final
notification.

## Main Participants

- Student / Team
- Project Coordinator
- Review Committee
- Faculty Guide
- Project Management System

## Main Process Flow

1. Student submits the project proposal.
2. The system validates the proposal and team information.
3. The Project Coordinator screens the proposal.
4. The system checks for similar or duplicate topics.
5. The Review Committee evaluates the proposal.
6. The proposal is either approved, returned for revision, or rejected.
7. For an approved proposal, guide availability and workload are checked.
8. A suitable faculty guide is allocated.
9. The guide reviews the allocation request.
10. The system records the allocation and notifies the student.

## Exception and Failure Handling

The model includes handling for cases such as:

- Invalid or incomplete proposal
- Invalid team composition
- Duplicate or similar project topic
- Missed submission deadline
- Committee-requested revision
- Proposal rejection
- Delayed committee review
- No suitable faculty guide available
- Faculty guide declining or not responding
- System or notification failure
- Student/team withdrawal after approval

## BPMN Concepts Used

The process demonstrates several BPMN 2.0 constructs, including:

- User Tasks
- Service Tasks
- Business Rule Tasks
- Send and Receive Tasks
- Exclusive Gateways
- Parallel Gateways
- Event-Based Gateway
- Timer Events
- Error Boundary Events
- Message Events
- Escalation
- Compensation
- Bounded Loops

## File

`student-project-approval.bpmn` contains the BPMN 2.0 process model and
can be opened using Camunda Modeler.

## Tool

The process was modelled using Camunda Modeler.
