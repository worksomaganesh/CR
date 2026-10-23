# Operations, privacy and compliance

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

## Security baseline before a real pilot
- Threat model and data-flow diagram
- Authentication and access controls
- Encryption in transit and at rest where applicable
- Logs that avoid exposing secrets or unnecessary customer data
- Backups and deletion policy
- Dependency and secret scanning
- Tested export and recovery procedure
- Clear incident contact and response plan
