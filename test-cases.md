# Home Credit LAP Voice Agent — Test Cases

## Purpose

These test cases evaluate whether the Retell AI voice agent follows the Loan Against Property (LAP) screening rules, handles customer responses correctly, and avoids unsupported promises.

## Test Environment

- Platform: Retell AI
- Agent: Home Credit LAP Voice Agent
- Testing method: Simulated or manual conversations
- Status convention: Not Run, Pass, or Fail

## Test Case 1: Potentially Eligible Customer

**Customer input:** The customer verifies their identity and provides the following answers:

- Property type: Residential
- Ownership: Sole
- Original documents: Available
- Requested loan amount: ₹40 lakh
- Occupation: Salaried
- Relevant income: Received through a bank
- Property market value: ₹80 lakh
- Requested tenure: 10 years

**Expected behavior:** The agent records all seven answers, completes preliminary screening, and explains that the customer may proceed to the next assessment step. It must not guarantee loan approval.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 2: Agricultural Property

**Customer input:** "The property I want to use is agricultural land."

**Expected behavior:** The agent politely explains that agricultural property does not meet the screening criteria and ends the normal qualification process.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 3: Original Documents Unavailable

**Customer input:** "I only have photocopies. I don't have the original property documents."

**Expected behavior:** The agent identifies the document requirement as unmet, politely explains the outcome, and ends the screening.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 4: Entirely Cash-Based Relevant Income

**Customer input:** "All the income I want to use for this application is received in cash."

**Expected behavior:** The agent identifies the income-source disqualification and ends the normal qualification process.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 5: Requested Loan Amount Above the Limit

**Customer input:** "I need ₹90 lakh."

**Expected behavior:** The agent explains that the potential offer is capped at ₹75 lakh and asks whether the customer would consider that amount.

**Follow-up A:** Customer accepts ₹75 lakh.

**Expected behavior:** The agent records the accepted amount and continues screening.

**Follow-up B:** Customer rejects ₹75 lakh.

**Expected behavior:** The agent politely ends the screening without continuing the checklist.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 6: Tenure Outside the Permitted Range

**Customer input:** "I want the loan for 2 years."

**Expected behavior:** The agent explains that the permitted tenure is 3–15 years and asks whether the customer would accept a tenure in that range.

**Follow-up:** Customer refuses to change the requested tenure.

**Expected behavior:** The agent politely ends the screening.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 7: Joint Ownership

**Customer input:** "The property is jointly owned by me and my spouse."

**Expected behavior:** The agent accepts joint ownership for the preliminary screening and continues with any unanswered questions.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 8: Existing Property Loan

**Customer input:** "I already have a loan against this property."

**Expected behavior:** The agent acknowledges the situation, indicates that specialist assistance is appropriate, and ends normal qualification. It does not continue the ordinary checklist or falsely claim a transfer has occurred.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 9: Customer Wants to Reduce Existing EMI

**Customer input:** "I want to reduce the EMI on my existing property loan."

**Expected behavior:** The agent identifies the specialist-referral condition and ends normal qualification politely.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 10: Customer Is Busy

**Customer input:** "I'm busy right now. Can you call me later?"

**Expected behavior:** The agent asks for a suitable callback time, acknowledges the response, and ends the call. It does not claim a callback has been scheduled unless the system supports it.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 11: Answers Provided Out of Order

**Customer input:** The customer gives the property value and occupation before answering the property-type question.

**Expected behavior:** The agent remembers the clear answers, does not ask for them again, and returns to the earliest unanswered checklist item.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 12: Unclear Document Availability

**Customer input:** "I think I can arrange the papers."

**Expected behavior:** The agent asks whether the original property documents are currently available for verification. It does not assume that the requirement is satisfied.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 13: Customer Asks for an Interest Rate

**Customer input:** "What is the interest rate?"

**Expected behavior:** The agent does not invent a rate. It explains that the rate has not been confirmed in the information available and directs the customer to the appropriate representative or next step.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 14: Customer Corrects an Earlier Answer

**Customer input:** The customer first says they have original documents, then corrects themselves and says they only have copies.

**Expected behavior:** The agent uses the latest clear answer, applies the document rule, and ends the screening politely.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Case 15: Customer Has Not Answered Every Question

**Customer input:** The customer answers six checklist items but has not provided the approximate property market value.

**Expected behavior:** The agent asks for the missing property market value and does not declare preliminary screening complete until all seven checklist items are answered.

**Actual result:** To be recorded after testing.

**Status:** Not Run

## Test Summary

Update this table after running the tests.

| Test | Description | Status |
|---|---|---|
| 1 | Potentially eligible customer | Not Run |
| 2 | Agricultural property | Not Run |
| 3 | Original documents unavailable | Not Run |
| 4 | Entirely cash-based income | Not Run |
| 5 | Loan amount above ₹75 lakh | Not Run |
| 6 | Tenure outside 3–15 years | Not Run |
| 7 | Joint ownership | Not Run |
| 8 | Existing property loan | Not Run |
| 9 | Existing EMI reduction | Not Run |
| 10 | Customer busy | Not Run |
| 11 | Out-of-order answers | Not Run |
| 12 | Unclear document availability | Not Run |
| 13 | Interest-rate question | Not Run |
| 14 | Correction to earlier answer | Not Run |
| 15 | Missing checklist item | Not Run |
