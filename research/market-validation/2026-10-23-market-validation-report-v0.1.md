# Market Validation Report v0.1

**Research date:** 23 October 2026  
**Stage:** Secondary research / hypothesis generation  
**Decision status:** No product-market fit claim; customer interviews and willingness-to-pay tests are still pending.  
**Purpose:** Preserve the first market-research baseline and the assumptions that should be challenged next.

## 1. Executive summary

The current leading hypothesis is a **GeM seller-side post-award execution assistant** for small suppliers. It would help sellers interpret order obligations, track delivery and document deadlines, and organise evidence after an order is accepted.

This is a hypothesis, not a validated gap. The public data confirms a large and active GeM ecosystem, and official suspension data names issues such as incorrect categories/specifications, unreasonable pricing, delivery delays, and refusal to supply after contract placement. It does **not** establish that these problems are frequent among our intended buyer segment, that current tools fail to address them, or that sellers would pay for another product.

Generic invoice-to-cash, payment reminder, and AI calling products look crowded in the initial competitor scan. Do not build a generic version of those categories without new evidence of a narrow unmet need.

**Current decision:** Continue desk research and conduct neutral customer discovery. Do not build the full product yet.

## 2. Candidate opportunity

### Working name
GeM Seller OrderGuard (temporary research label only; not a final brand).

### Target buyer hypothesis
A small GeM supplier with recurring orders, limited dedicated operations staff, and several delivery/documentation/payment obligations to track. The daily user may be the owner, operations coordinator, or accounts employee; the economic buyer may be the owner.

### Problem hypothesis
After an order is placed, the seller may need to coordinate order specifications, delivery dates, documentation, dispatch proof, acceptance status, invoicing and follow-up. A missed requirement or deadline may create operational cost, delay, disputes or platform risk.

### Proposed narrow value
Before committing to fulfil an order, extract key obligations from the order/contract document, flag potential specification/deadline/capacity risks for human review, and generate a traceable checklist. After acceptance, track tasks and evidence.

The product should not replace GeM, promise compliance, submit documents automatically, or claim it can prevent suspension. It must cite the source text/page for extracted obligations and clearly label uncertainty.

## 3. Market signals — facts vs interpretation

### Signal A: Large GeM MSME participation
A Press Information Bureau release dated 11 August 2026 reports 11,75,001 MSMEs registered on GeM as of 30 July 2026, and ₹2,37,235 crore of MSME order value in FY 2025–26.

- **What this supports:** GeM is a substantial ecosystem with many potential businesses.
- **What it does not support:** The number of sellers with the proposed pain, software adoption, addressable segment size, or willingness to pay.

Source: [PIB — GeM Strengthens Participation of MSMEs, Startups, Women Entrepreneurs and SHGs](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2297820&lang=1&reg=48)

### Signal B: Seller execution and compliance incidents
A companion PIB release gives FY 2025–26 figures of 1,81,035 incidents raised and 55,772 seller suspensions. Listed reasons include wrong category/specifications, unreasonable offer pricing, delivery delays, and refusal to supply after contract placement.

- **What this supports:** Operational/compliance failures exist in the ecosystem.
- **What it does not support:** That the proposed software could prevent these incidents, or that these numbers represent preventable post-award workflow mistakes. Some causes are intentional, commercial or unrelated to software.

Source: [PIB — GeM release, English/Hindi language variants](https://www.pib.gov.in/PressReleaseIframePage.aspx?PRID=2297820&lang=2&reg=48)

### Signal C: Existing GeM and service alternatives
GeM has an official seller app and portal workflows. GeM consultants also offer seller management, order/invoice assistance, CRAC and payment follow-up. These are direct substitutes and may already solve the problem for some businesses.

Sources:
- [GeM official website](https://gem.gov.in/)
- [GeM seller app on Google Play](https://play.google.com/store/search?q=GeM%20Seller&c=apps)
- [GemBook](https://gembook.in/)
- [Tech Vantage Consulting](https://techvantageconsulting.in/)

**Research limitation:** Feature availability and current service prices must be re-checked directly before making a buying decision. Vendor pages are not independent evidence of customer outcomes.

## 4. Competitor and substitute scan

| Product / substitute | Publicly described coverage | Implication for our hypothesis | Evidence type |
|---|---|---|---|
| Official GeM portal / seller app | Seller, order and payment-related access | A simple status dashboard is unlikely to differentiate | Official platform source; verify exact current features |
| GemBook | GeM-related seller support and expert services, including order/invoice/CRAC/payment workflows | Human help is an existing alternative | Vendor website |
| Tech Vantage Consulting | GeM management/compliance assistance and order/invoice support | Sellers may pay people to handle the workflow rather than buy software | Vendor website |
| Zoho Books | Accounting, payment reminders, purchase orders; PO matching in its BillPay add-on | Generic invoice, reminder and PO matching features are already served | Official vendor documentation |
| PraecisAI | AI calling/WhatsApp payment recovery, promise tracking and receivables workflow | Generic AI receivables automation is not an obvious gap | Vendor marketing/pricing |
| Rallic | Accounting and invoice-to-cash workflows, reminders and reconciliation | Generic invoice-to-cash automation has direct competition | Vendor website/pricing |
| PaisaBaki | Receivables follow-up and promise/blocker tracking | Basic follow-up queue/reminder concept is not differentiated by itself | Vendor website |

Links:
- [Zoho Books — PO matching](https://www.zoho.com/in/books/help/billpay-addon/po-matching.html)
- [Zoho Books — purchase orders](https://www.zoho.com/in/books/help/purchase-order/)
- [PraecisAI](https://www.praecisai.in/)
- [Rallic](https://rallic.ai/)
- [Rallic pricing](https://rallic.ai/pricing)
- [PaisaBaki](https://paisabaki.com/)

### Pricing signals observed on vendor pages
- Rallic lists ₹399/month for its first company on its published pricing page, with other conditions and GST described there.
- PraecisAI lists a ₹5,000/month platform fee, a one-time setup offer, and usage-based messaging/calling. Pricing can change; re-check before relying on it.

These are **published vendor offers**, not independently verified realised prices, customer counts, or profitability.

## 5. Why not choose generic invoice automation or AI calling first?

1. Invoice capture, PO matching and accounting workflows already exist in established accounting tools.
2. Receivables reminder and AI-calling products already advertise integrations, promise-to-pay tracking, WhatsApp and voice workflows.
3. Generic AI calling adds telephony cost, trust barriers and commercial-communication compliance questions before we have proven our own offer.
4. A student founder with ₹0 should avoid building a broad platform that requires many integrations and high reliability before the first customer.

These categories are not permanently rejected. They can return to the shortlist if customer evidence reveals a narrower, neglected workflow.

## 6. Proposed first product experiment — not yet a build commitment

Manually test one workflow using a redacted sample order document:

1. Extract order number, item/specification, quantity, delivery deadline, required documents and acceptance/invoice milestones.
2. Link each extracted item to its source page/text.
3. Ask the seller to confirm or correct the extraction.
4. Produce a checklist with owner, due date, status and evidence link.
5. Ask whether this would replace a real existing spreadsheet/process, what risk it reduces, and whether they would pay to use it on the next order.

Do not upload confidential buyer/seller documents to third-party AI services without explicit permission and an appropriate data-handling review.

## 7. Customer discovery questions

Ask about past behaviour, not hypothetical enthusiasm:

1. “Walk me through the last GeM order you received, from contract/order placement to delivery and payment.”
2. “Who was responsible for each step?”
3. “Which documents and deadlines did you need to track?”
4. “What tools did you use—GeM, spreadsheets, accounting software, a consultant, WhatsApp, or something else?”
5. “Tell me about the most recent time a requirement, deadline or document was missed or nearly missed.”
6. “What happened, and what did it cost in time or money?”
7. “How often has this happened in the last six months?”
8. “What have you already tried to improve the process?”
9. “What do you pay a consultant or employee to do for this workflow?”
10. “May I see a redacted example of the checklist or document you actually use?”
11. “What would make you refuse to use another tool?”
12. “Would you consider a limited paid pilot for a defined next order? What would need to be true for that to make sense?”

Do not lead with the product idea. Listen first, then show a prototype only if the conversation warrants it.

## 8. Kill criteria / reasons to pivot

Pause or abandon this hypothesis if evidence shows any of the following:

- Sellers already manage the workflow reliably using existing GeM tools, spreadsheets, accounting tools or consultants.
- The problem is infrequent, low-cost or not a priority for the intended segment.
- The proposed user cannot approve purchase and there is no reachable buyer.
- Sellers will discuss the idea but will not share a redacted workflow, test a prototype, or consider a paid pilot.
- Accurate extraction requires expensive integrations or inaccessible data that a zero-capital solo founder cannot support.
- The product cannot reliably cite source evidence and distinguish uncertain extraction from verified obligations.
- Existing products already solve the proposed narrow workflow at a price and quality the target buyer prefers.
- Handling documents creates privacy/security risks that cannot be managed in the initial scope.

## 9. Confidence and next actions

| Claim | Current confidence | Next evidence needed |
|---|---|---|
| GeM is a substantial MSME procurement ecosystem | High, based on official public figures | Keep source/date in research log |
| Execution/compliance incidents exist | High, based on official aggregate figures | Understand which are software-addressable |
| Small suppliers experience this specific workflow pain repeatedly | Low / unvalidated | Interviews and recent workflow examples |
| Current tools leave a meaningful gap | Low / unvalidated | Feature-by-feature competitor and workflow comparison |
| Sellers will pay for a standalone product | Unknown | Paid-pilot discussion and actual payment |
| Codex can help build a lightweight document/checklist MVP | Plausible technical hypothesis | Prototype and accuracy/security tests |
| GeM OrderGuard is the best opportunity | Not established | Compare against alternative niches using the same scoring rubric |

### Immediate next steps
1. Run the adversarial research prompt in Gemini Argon 4 Task Mode.
2. Independently verify sources and competitors; do not accept generated claims without URLs and supporting text.
3. Identify 20 relevant business prospects using public business sources; do not invent contacts or infer a specific pain as fact.
4. Conduct 10–15 neutral discovery conversations if reachable; record actual evidence and anonymise details.
5. Decide build / pivot / stop only after reviewing results.

## 10. Source register

1. PIB, Ministry of Commerce & Industry, “GeM Strengthens Participation of MSMEs, Startups, Women Entrepreneurs and SHGs,” posted 11 Aug 2026: https://www.pib.gov.in/PressReleasePage.aspx?PRID=2297820&lang=1&reg=48
2. PIB, companion language variant containing incident/suspension table and listed reasons: https://www.pib.gov.in/PressReleaseIframePage.aspx?PRID=2297820&lang=2&reg=48
3. GeM official website: https://gem.gov.in/
4. GeM Seller app search page: https://play.google.com/store/search?q=GeM%20Seller&c=apps
5. GemBook: https://gembook.in/
6. Tech Vantage Consulting: https://techvantageconsulting.in/
7. Zoho Books PO matching documentation: https://www.zoho.com/in/books/help/billpay-addon/po-matching.html
8. Zoho Books purchase order documentation: https://www.zoho.com/in/books/help/purchase-order/
9. PraecisAI product and pricing: https://www.praecisai.in/
10. Rallic product: https://rallic.ai/
11. Rallic pricing: https://rallic.ai/pricing
12. PaisaBaki product: https://paisabaki.com/

**Source-quality note:** Official PIB figures are stronger evidence for ecosystem counts and reported incident totals. Vendor websites establish what vendors publicly claim to offer, not independent product efficacy. No customer interviews or payment evidence are included in this v0.1 report.
