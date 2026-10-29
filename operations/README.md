# Operations, privacy and compliance

The [service catalogue](../docs/service-catalogue.md) defines the intended scope across marketing content, AI knowledge systems, sales/customer workflows, websites/integrations, analytics and custom technical solutions. Before any offer goes live, define data access, permissions, review steps, limitations, failure handling, customer acceptance tests and support ownership.

## Data protection
- Collect the minimum data required.
- Prefer synthetic or redacted documents for demos.
- Obtain permission before processing customer documents.
- Review the AI provider's retention, training, region, access and deletion terms before sending confidential information.
- Never commit API keys, passwords, customer invoices, contracts, or personal data to Git.
- Use environment variables/secrets management and least-privilege access.
- Provide a deletion/export path if the product stores customer data.

## AI reliability
- Cite the source page/text for extracted contractual obligations.
- Require human confirmation of critical dates, amounts, specifications and commitments.
- Test missing, ambiguous, conflicting and low-quality documents.
- Do not promise legal compliance or guaranteed prevention of penalties.
- Keep an audit trail for material changes and approvals.

## Outreach and calling
Use legitimate published business contact routes. Before automated or bulk commercial calls, independently verify current TRAI regulations, DLT/TSP requirements, consent/permission rules and vendor terms. A vendor tool does not automatically make a campaign compliant.

## Service-specific safeguards

- **Marketing/reviews:** use genuine business information and real reviews only; do not fabricate reviews, claims, customer outcomes or competitor findings. Respect platform rules, consent, opt-outs and IP rights.
- **WhatsApp, voice and appointments:** verify current provider/API terms, customer consent/permissions, applicable Indian commercial-communication rules, booking permissions and human handoff. An integration vendor does not itself guarantee compliance.
- **Knowledge assistants/PDF chatbots:** enforce document-level access where needed, test unsupported/conflicting sources and prompt injection, show citations where feasible, and define source update/deletion behaviour.
- **Proposal/quote/lead systems:** validate approved facts and price rules; require appropriate human approval before binding commitments or final quotes.
- **Analytics/Power BI:** document source definitions, transformations, KPI logic, refresh failures and access controls. Verify the customer's actual Microsoft licensing and sharing requirements before deployment; a `.pbix` file is not the same as a published managed dashboard.
- **AI-generated software/content:** use independent review, representative tests and actual environment checks. Do not report generated work as verified without evidence.

## Security baseline before a real pilot
- Threat model and data-flow diagram
- Authentication and access controls
- Encryption in transit and at rest where applicable
- Logs that avoid exposing secrets or unnecessary customer data
- Backups and deletion policy
- Dependency and secret scanning
- Tested export and recovery procedure
- Clear incident contact and response plan
