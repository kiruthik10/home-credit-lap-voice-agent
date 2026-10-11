# home-credit-lap-voice-agent
etell AI voice agent for Home Credit Loan Against Property pre-qualification
# Home Credit LAP Voice Agent

## Project Overview

This project implements an AI-powered voice agent using Retell AI for the Home Credit Loan Against Property (LAP) pre-qualification process.

The agent conducts an initial conversation with customers, verifies their identity, explains the potential loan offer, and collects information needed for preliminary eligibility screening.

## Objectives

- Verify the intended customer before discussing the offer.
- Explain the potential Loan Against Property offer of up to ₹75 lakh without promising approval.
- Collect and assess the required eligibility information.
- Identify disqualifying responses and specialist-referral cases.
- Avoid repeating questions when the customer has already provided clear answers.
- Direct potentially eligible customers to the next step for further assessment.

## Technology Used

- Retell AI — voice agent creation and testing.
- Large Language Model (LLM) — conversational understanding and response generation.

## Eligibility Checks

The agent collects information about:

1. Property type.
2. Property ownership.
3. Availability of original property documents.
4. Requested loan amount.
5. Occupation and income source.
6. Approximate property market value.
7. Requested loan tenure.

The agent performs preliminary screening only. Final loan approval is subject to further assessment.

## Repository Contents

- `README.md` — project overview and documentation.
- `agent-prompt.md` — final agent instructions.
- `test-cases.md` — test scenarios and expected outcomes.

## Live Demo

Retell AI published agent: [Insert your published Retell agent URL here]

## Testing

The agent should be tested with eligible, ineligible, ambiguous, and specialist-referral scenarios before submission.
