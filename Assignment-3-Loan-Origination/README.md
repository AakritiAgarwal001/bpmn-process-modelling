# Assignment 3 – Loan Origination & Approval

## Overview

This BPMN 2.0 process models a loan origination and approval workflow,
from application submission through verification, risk assessment,
underwriting, approval, e-signature, and disbursement.

The model focuses on both the normal approval flow and exception
handling throughout the loan lifecycle.

## Main Participants

- Applicant
- Loan Processing System
- KYC / Verification Team
- Credit Bureau
- Fraud & Compliance Team
- Underwriting / Credit Committee

## Main Process Flow

1. Applicant submits a loan application and required documents.
2. The system checks document completeness.
3. KYC, credit, and income verification are performed.
4. The application is assessed for eligibility and risk.
5. The application is automatically approved, sent for manual review,
   or rejected depending on the assessment.
6. Underwriting and additional checks are performed where required.
7. A loan offer is generated for an approved application.
8. The applicant accepts the offer and completes e-signature.
9. The applicant's account details are verified.
10. The loan is disbursed and the loan account is created.
11. The applicant is notified of the final outcome.

## Exception and Failure Handling

The model includes handling for cases such as:

- Missing or incomplete documents
- KYC verification mismatch
- Fraud or AML concerns
- Credit Bureau unavailability
- Low credit score
- Insufficient income or high debt-to-income ratio
- Borderline or high-value applications requiring escalation
- Collateral valuation or title issues
- Loan offer expiry
- Applicant withdrawal
- E-signature failure
- Disbursement failure

## BPMN Concepts Used

The process demonstrates several BPMN 2.0 constructs, including:

- User Tasks
- Service Tasks
- Business Rule Tasks
- Exclusive Gateways
- Parallel Gateways
- Inclusive Gateways
- Message Events
- Timer Events
- Error Boundary Events
- Compensation
- Event Sub-processes
- External Participants / Pools

## File

`loan-origination.bpmn` contains the BPMN 2.0 process model and can be
opened using Camunda Modeler.

## Tool

The process was modelled using Camunda Modeler.
