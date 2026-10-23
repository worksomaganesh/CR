# Market Gap Validation — Phase 1: Official Rules, Competitors and Discovery Readiness

**Date:** 23 October 2026  
**Status:** Desk research completed; customer validation not yet performed.  
**Related work:** [Gemini Argon report](../../argon/research-task-1.md) · [Independent audit](../../argon/research-task-1-audit.md)

## Executive decision

**Do not build Candidate D yet.** Retain it as the current best interview hypothesis, not as a validated product.

The corrected problem area is not “a Form 3CD Clause 22 generator”. For the upcoming Tax Year 2026–27, the Income Tax Department says the tax audit report uses new Form No. 26 under the Income-tax Rules, 2026. The notified Rules put the MSME-related disclosures in Part D, Clause 33. The older Forms 3CA/3CB/3CD remain relevant for FY 2025–26 / AY 2026–27.

Public competitor research also narrows the possible gap: a free CalcGuru worksheet already covers many legacy FY 2025–26 Section 43B(h) calculations, while Tally supports MSME supplier details, due-date tracking, overdue reports and MSME Form 1 exports. Figment advertises bulk Udyam verification and says it supports Form 26 / Section 37(2)(g). A new tool cannot win by merely calculating dates, identifying Udyam vendors or exporting a spreadsheet.

The only defensible question worth testing is whether CA firms have a recurring, material **cross-client exception-reconciliation / evidence-traceability / working-paper QA workflow** that remains painful while adapting client data and existing tools to the current Form No. 26 reporting format—and that the free Filingo and Charter AI tools, Tally and Figment do not already solve. This is a narrow, lower-confidence assumption. Candidate D should be treated as at risk of being a no-go unless interviews reveal a specific gap.

## 1. Official form and tax-year mapping

The Income Tax Department's form FAQ states:
- FY 2025–26 / AY 2026–27: use the existing Form 3CA / 3CB / 3CD framework under the Income-tax Act, 1961.
- Tax Year 2026–27 under the Income-tax Act, 2025: use Form No. 26 under the Income-tax Rules, 2026.
- The stated tax-audit report due date for Tax Year 2026–27 is 30 September 2027.

Official source: https://www.incometax.gov.in/iec/foportal/help/all-topics/e-filing-services/income-tax-forms?mobile-app=1

The notified Income-tax Rules, 2026 are effective from 1 April 2026. In the official Form No. 26, Part D (“Particulars of expenses”), Clause 33 asks for:
- (a) interest not allowable under Section 23 of the MSMED Act to the extent debited to the profit and loss account;
- (b) amounts debited to the profit and loss account to the extent disallowable under Section 37(2)(g); and
- (c) amounts disallowed under Section 37(2)(g) in a preceding tax year but allowable during the current tax year.

Official notified Rules PDF: https://www.incometax.gov.in/iec/foportal/sites/default/files/2026-03/En-Notified-IT-Rules-2026-20-03-2026.pdf  
PDF location in the official document: Form No. 26, Part D, Clause 33, printed pages 1882–1883 (PDF page index around 349).

**Design implication:** Any product hypothesis for the new tax year must map to the current Form No. 26 schema and the correct statutory mapping. The product must not silently reuse an old Form 3CD / Section 43B(h) template as if it were the current form. Prior-year support should be handled as a separate, explicitly selected tax-year workflow.

**Professional boundary:** This is a source-mapping note, not tax advice. A practising CA must review the rule mapping, treatment of exceptions, input assumptions and expected working papers before a calculation workflow is built or used.

## 2. Current competitor / substitute comparison

| Alternative | Publicly described capability | Consequence for our hypothesis | Evidence type |
|---|---|---|---|
| CalcGuru FY 2025–26 workbook | Free Excel download; supplier master, applicability inputs, Section 15 due dates/ageing, compound-interest ledger, Form 3CD Clause 22 figures and MSME Form 1 extract | A generic legacy-year spreadsheet calculator is already offered free; copying those features is not a gap | Vendor-published offer |
| TallyPrime | Records MSME details and effective dates/history, tracks upcoming and overdue supplier bills, generates MSME reports and Form 1 annexure exports | Basic status capture, ageing and due-date workflows are already served for Tally users | Official vendor documentation |
| Figment MSME Compliance / VenCPC | Bulk Udyam/MSME status verification, vendor master checks, API and a page that expressly describes Form 26 / Section 37(2)(g) coverage | Classification verification and the new statutory mapping already have a commercial supplier; feature depth/pricing/customer evidence still need checking | Vendor-published offer |
| Filingo — MSME 43B(h) & MSME-1 checker | Free browser-based tool accepts a creditor-bill list and checks Section 43B(h), MSMED interest and MSME-1; claims files stay in the browser and offers an Excel working paper | Directly overlaps with the proposed “upload ledger → calculate → export” utility for the legacy regime | Vendor-published offer |
| Charter AI — MSME 45-day payment checker | Free browser-based checker for CA firms; accepts a purchase ledger and outputs late payments, tax disallowance and interest; page says rules reviewed 2 October 2026 | Directly overlaps with the simplest CA-facing ledger-checking MVP | Vendor-published offer |
| Human CA staff / Excel utilities | Manual evidence review, spreadsheets and existing audit working papers | A workflow must save enough time or reduce enough rework to justify changing a trusted process | Substitute hypothesis; validate in interviews |

Sources:
- CalcGuru: https://calcguru.in/excel-downloads/msme-supplier-ageing-43bh-excel/
- Tally MSME payment management (updated 29 September 2026): https://help.tallysolutions.com/managing-payments-to-msme-businesses/
- Tally Udyam setup (updated 29 September 2026): https://help.tallysolutions.com/set-up-udyam-details-msme-suppliers/
- Tally Form 1 annexure / due date workflows: https://help.tallysolutions.com/due-dates-for-payables-to-msme-suppliers/
- Figment MSME compliance: https://www.figmentglobal.com/msme-compliance
- Figment MSME verification API: https://www.figmentglobal.com/msme-verification-api/
- Filingo free checker: https://filingo.in/tools/msme-43bh
- Charter AI free checker: https://www.charterai.in/tools/msme-payment-checker

### Important pricing correction
CalcGuru's page labels its FY 2025–26 workbook “FREE DOWNLOAD”. It already advertises substantial functionality. The earlier Gemini report's repeated ₹999–₹2,500 price assumption for this specific workbook should not be used unless a different, separately priced SKU is verified.

### What this comparison does and does not prove
It shows significant capability overlap in existing products. It does **not** prove that every CA workflow is solved, nor does it prove an unmet niche exists. Vendor claims and feature pages are not independent evidence of accuracy, user satisfaction or purchase intent.

## 3. Refined product hypothesis to test

**Temporary hypothesis:** “CA MSME Exception & Working-Paper QA Assistant for Tax Year 2026–27.”

Potential workflow, only if interviews confirm the problem:
1. Accept a CA-approved, non-sensitive export format (CSV/Excel/XML) and a manifest of supporting records.
2. Compare supplier-status fields, relevant dates, balances, payments and supporting evidence for inconsistencies or missing inputs.
3. Flag only exceptions and missing evidence; show source rows/files for every flag.
4. Produce a reviewer-controlled working-paper draft mapped to the current Form No. 26 Part D, Clause 33, with separate support for prior-year/legacy formats only if customers need them.
5. Require CA review for legal interpretation and final amounts. Do not generate a purported final audit opinion or “audit-ready” guarantee.

This is not yet a product recommendation. Another tool may already do this. The first experiment is interviews and a workflow map, not code.

### What the MVP must not do
- Make autonomous legal decisions about MSME eligibility or a supplier's trader/category treatment.
- Treat a guessed acceptance date, missing Udyam details or ambiguous record as fact.
- Produce a final tax audit opinion or file forms.
- Upload client records to cloud AI services without explicit authorisation and appropriate security review.
- Promise that it prevents penalties or guarantees compliance.

## 4. Primary questions for customer discovery

Start by asking about the respondent's actual most recent workflow:
1. “Could you walk me through how your team prepared MSME payment working papers for a recent audit—from data export to the final reported figures?”
2. “Which accounting system, spreadsheets and existing tax/audit tools did you use?”
3. “Which fields came directly from the system, and which required a person to find or verify evidence elsewhere?”
4. “What was the last discrepancy or missing detail that caused rework?”
5. “How often did that happen, and how much staff time did it take?”
6. “How is your firm adapting its previous working files to Form No. 26 for Tax Year 2026–27?”
7. “What does your current process already do well? What would make you avoid a new utility?”
8. “What would you need to trust an exception report?”
9. “What tools has the firm actually paid for to solve similar workflow problems, and why?”
10. “Would you be willing to review a synthetic example or give feedback on a mock-up, without sharing client information?”

Do not start with “Would you buy our AI software?” or claim that CA firms have this pain. Do not request live client ledgers, Udyam certificates or tax documents during first discovery.

## 5. Validation gate

For the first round:
- Verify and prioritise 10 relevant CA practices using their official public business pages.
- Begin with three personalised research requests, not a blast.
- Aim for 5–8 completed discovery conversations if feasible; this is a practical learning target, not a statistically representative sample.
- Ask for a redacted or synthetic workflow artefact only after trust and permission are established.
- Record negative evidence as carefully as positive evidence.

Proceed to a synthetic-data prototype only if several independent firms describe a common, material workflow gap; existing solutions leave it unresolved; and at least one or two buyers express credible willingness to test a clearly scoped pilot. A paid commitment is stronger evidence than praise.

## 6. Kill / pivot criteria

Pause or abandon this hypothesis if:
- CA firms say Tally + their current Excel/utility already handles the problem with acceptable effort.
- No one can show an actual recurring exception or rework pattern.
- The proposed gap is already included in Figment, a tax-audit tool, or another incumbent at acceptable cost.
- Required information cannot be obtained lawfully or reliably.
- Firms refuse to share even synthetic workflow requirements or to test an anonymised/controlled example.
- No buyer has a budget or the person with the pain cannot influence purchase.
- The legal mapping is too complex to test safely without significant expert involvement.
- Seasonal sales and the small target segment cannot support the business ambition, even if a small utility is useful.

## 7. Current conclusion

**Desk research status:** Very strong evidence of competitor overlap, including two additional free tools directly covering ledger-based checking; no validated market gap yet. The simple MVP is not differentiated and should not be built.

**Best next move:** Before outreach, compare Filingo and Charter AI against the exact proposed workflow and new Form No. 26 needs. Then conduct a small number of neutral CA interviews to determine whether there is a distinct gap beyond free ledger-checkers, Tally and Figment. If interviewees cannot name a recurring unresolved workflow, stop Candidate D and return to wider market research.

**Not completed:** No CA has been contacted, no interview has been conducted, no workflow artefact has been obtained, no prototype has been built, and no payment commitment exists.
