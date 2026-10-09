# Failure Path Register

| ID | Failure Point | Cause / Trigger | BPMN Solution |
|---|---|---|---|
| F1 | Incomplete documents | Required documents are missing or incomplete | Request missing documents and use a timer-based resubmission loop; application may lapse if not completed |
| F2 | KYC mismatch | Applicant information does not match verification records | Route to manual verification; unresolved mismatch results in rejection |
| F3 | Fraud / AML flag | Fraud or compliance concerns are detected | Send the application for Fraud & Compliance investigation; confirmed issues lead to rejection |
| F4 | Credit Bureau unavailable | External credit verification service is unavailable | Error boundary handling triggers retries; after repeated failure, use manual verification or park the application |
| F5 | Low credit score | Credit assessment falls below the required threshold | Reject the application or generate a counteroffer requiring additional support such as a guarantor or collateral |
| F6 | Insufficient income / high DTI | Applicant does not meet affordability requirements | Adjust loan amount or tenure and re-assess; reject if the application remains unsuitable |
| F7 | Borderline / high-value application | Application requires additional review or exceeds the normal approval threshold | Escalate to senior credit committee with SLA/timer-based handling |
| F8 | Collateral issue | Collateral valuation or ownership/title is unsuitable | Revalue collateral, adjust LTV, and re-underwrite; unresolved title issues result in rejection |
| F9 | Loan offer expires | Applicant does not accept the offer within the allowed period | Timer boundary event marks the offer as expired |
| F10 | Applicant withdrawal | Applicant withdraws during processing | Message-triggered withdrawal handling activates compensation and releases relevant holds |
| F11 | E-signature failure | Applicant is unable to complete the electronic signature | Resend/remind the applicant; repeated failure results in cancellation of the offer |
| F12 | Disbursement failure | Funds cannot be successfully disbursed | Verify account details, retry disbursement, and use compensation/reversal handling where required |
