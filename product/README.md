# Product and solution delivery

The [CR service catalogue](../docs/service-catalogue.md) records the intended capability portfolio: AI marketing, knowledge systems, sales/customer operations, websites/integrations, reporting/analytics, and custom technical solutions. These are not all launched products; each offer needs its own validated buyer, problem, scope, acceptance criteria and economics.

No final first-product commitment has been made. This folder records product hypotheses and, only after validation, requirements, design, architecture, implementation notes, tests and release evidence.

## Current hypothesis (unvalidated)
A seller-side GeM post-award execution assistant. Proposed workflow:
1. Upload a permitted order/contract document.
2. Extract obligations and link each field to source evidence.
3. Require human confirmation of critical facts.
4. Generate a checklist and deadlines.
5. Track fulfilment and document evidence.
6. Prepare draft follow-up correspondence for human approval.

## Non-goals for the first test
- Replacing GeM.
- Guaranteeing compliance or preventing suspension.
- Automatically accepting contracts or submitting documents.
- Building generic tender discovery, generic invoice OCR or generic AI calling.
- Connecting to private accounts without a clear permission and security model.

## Product selection rule

Do not choose an idea merely because it is easy to demo with AI or uses an interesting architecture. Compare the hypothesis with alternatives and existing competitors; speak to relevant buyers; define a small paid-pilot scope; and proceed only when the evidence supports the problem and delivery path. A service-assisted pilot may be appropriate before standalone SaaS. The broad catalogue must not be treated as permission to build every service at once.

## Quality bar
Traceability, correction workflow, clear uncertainty, safe data handling, and reproducible tests are more important than adding features.
