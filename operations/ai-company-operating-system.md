# CR AI Company Operating System

**Status:** Proposed operating model; adoption begins with controlled internal workflows  
**Recorded:** 18 November 2026  
**Inspiration:** [Grok Bot Galaxy case study](../research/2026-11-18-grok-bot-galaxy-case-study.md)

## 1. Purpose

Turn CR into a well-organised AI-native technical-solutions business by treating AI tools as bounded specialist workers inside a repeatable company workflow.

This is an operating model, not a promise of fully autonomous agents or a new software platform. Start with existing tools, documents and human approvals. Automate a workflow only after it is understood, repeatable and safe.

## 2. Operating architecture

### Human founder — CEO / final accountable owner

The founder owns:
- Company direction, niche and offer choices.
- Interpretation of customer evidence and go/no-go decisions.
- Customer discovery, relationship-building and final communications.
- Pricing, proposals, scope, contracts and commitments.
- Security, privacy, legal/compliance checks and data access approvals.
- Final acceptance of deliverables, production releases and money movement.

AI workers can prepare recommendations and artifacts, but cannot assume these responsibilities.

### Chief of Staff — workflow coordinator

The coordinator is the single entry point for turning a goal into a sequence of tasks. It should:
- Read the current CR source-of-truth documents.
- Break a goal into bounded work packets.
- Assign each packet to an appropriate specialist role/tool.
- Track owner, status, dependencies, due date and blockers.
- Gather deliverables and evidence.
- Identify contradictions, missing information and decisions requiring the founder.
- Update the relevant documentation/log after approval.

It must not quietly approve its own recommendations, create commercial commitments, contact prospects, merge code or deploy production changes.

### Specialist workers

Specialists work on one function with one clear output contract. Their roles and authority limits are defined in [agent-role-catalogue.md](agent-role-catalogue.md).

## 3. CR source of truth and tools

| Layer | CR choice | Rule |
|---|---|---|
| Company knowledge and decision record | This CR GitHub repository | Dated research, decisions, workflows, templates and logs live here |
| Task tracking | GitHub Issues/Projects or a simple documented task board | Each task links to its brief, owner, status and evidence |
| Research | Gemini Argon 4 Task Mode or another approved research tool | Return source URLs, dates, evidence labels and contradictions |
| Planning and review | ChatGPT / Chief of Staff role | Convert research into decisions, plans, task packets and review questions |
| Software implementation | Codex or the selected coding agent | Work from a scoped issue/spec; do not deploy without gates |
| Brand execution | Foundable, if adopted | Draft website/social assets from approved content; publishing requires founder approval |
| Source control and release evidence | GitHub | Branches, commits, tests, PRs, releases and deployment records |
| Private customer records | A separately approved private system | Never store customer PII, contracts, credentials or raw private files in this public CR repository |

Tool availability and subscription entitlements must be checked in the actual account before a workflow depends on them. Do not purchase additional subscriptions or infrastructure until a measured bottleneck justifies the cost.

CR's public repository may contain sanitized summaries, templates, public-source links and decision records. Detailed prospect records, interview notes, customer documents, pricing negotiated for a named customer, credentials and other confidential material belong in a properly secured private system.

## 4. Initial role map

Start with a small bench and reuse roles rather than creating a separate bot for every tiny task.

| Role | Main responsibility | Preferred current tool/route | Output |
|---|---|---|---|
| Chief of Staff | Coordinate and maintain task flow | ChatGPT / founder-supervised coordinator | Task plan, status, blockers, decision requests |
| Market Intelligence Researcher | Market, niche and competitor research | Gemini Argon 4 Task Mode | Source-linked research pack |
| Opportunity / Product Analyst | Evaluate pain, ICP, alternatives, scope and validation | ChatGPT with research evidence | Opportunity brief, interview plan, go/no-go recommendation |
| Solution Architect | Define the smallest reliable technical approach | ChatGPT or Codex planning mode | Architecture note, data flow, risks and acceptance tests |
| Engineer | Implement scoped code and tests | Codex | Branch/PR, code, test results and setup notes |
| Independent QA / Security Reviewer | Challenge the implementation and inspect proof | Separate review pass/tool/session | Findings, reproduction steps, risk and release recommendation |
| Sales Researcher / SDR assistant | Qualify business leads and draft personalised outreach | Argon/research workflow plus founder review | Verified lead brief and unsent draft |
| Customer Success / Support assistant | Prepare onboarding, FAQ, support triage and follow-up | ChatGPT using approved private customer context | Draft response, resolution checklist and escalation |
| Brand / Marketing operator | Turn verified work into content and maintain the portfolio | Foundable + founder approval | Draft posts, site copy, campaign plan and analytics summary |
| Finance / Operations analyst | Track costs, quotes, delivery capacity and operating metrics | Spreadsheet + review assistant | Cost sheet, cash-flow update and exception report |

Roles may initially be performed by the same tool in separate sessions. What matters is clear task scope and an independent review step—not the number of bots or model subscriptions.

## 5. Workflow lifecycle and status

Use consistent statuses across research and delivery tasks:

1. **Backlog** — idea recorded, no work started.
2. **Ready** — scope, owner, input and acceptance criteria are clear.
3. **In progress** — assigned worker is executing.
4. **Agent complete** — a draft artifact exists; not yet accepted.
5. **Review required** — evidence and output await a human or independent reviewer.
6. **Blocked** — dependency, access, ambiguity or risk prevents safe progress.
7. **Accepted** — the accountable human confirms the output meets criteria.
8. **Released / Published** — the approved result is live; record a URL or release identifier.
9. **Closed / Rejected** — task ended with outcome and rationale documented.

"Agent complete" is deliberately different from "Accepted". A generated artifact, passing unit test, merged pull request and verified customer outcome are different states.

## 6. The six operating loops

### A. Opportunity research and validation

**Flow:** question/hypothesis → source research → competitor/substitute comparison → problem brief → ICP → interview preparation → customer discovery → decision.

Required gates:
- Evidence must distinguish fact, vendor claim, assumption and unknown.
- Desk research cannot prove willingness to pay.
- Do not build a full product merely because the research agent recommends it.
- A founder approves any change to the active hypothesis or selected offer.
- Preserve rejected ideas and reasons to stop.

### B. Product and solution delivery

**Flow:** validated workflow → scoped requirements → acceptance tests → architecture → small implementation tasks → code/test → independent review → staging/preview → founder/customer acceptance → deployment → monitoring/support.

Engineering gates:
- Use a feature branch and pull request for meaningful changes.
- Run tests and relevant security checks.
- Do not allow an implementing agent to approve its own work.
- Verify UI behaviour in a real preview when relevant.
- Require human approval for schema migrations, secrets, permissions, production deployment, destructive operations and customer data changes.
- Keep a rollback or recovery path for consequential releases.

Do not copy an event-specific "ship directly to main" shortcut. CR's standard is reliable delivery, not maximum agent throughput.

### C. Sales and lead acquisition

**Flow:** define ICP → identify public business sources → verify relevance → qualify → prepare account context → draft a personalised message → founder approves and sends → record response → discovery → proposal → paid pilot.

Rules:
- No fabricated pain points or contact details.
- No scraped private personal numbers or indiscriminate bulk outreach.
- Treat all generated messages as drafts.
- The founder approves each external message and controls follow-up frequency.
- Store detailed private lead information outside the public CR repo.
- Record the difference between a lead, a reply, a discovery call, a proposal, a committed pilot and a cleared payment.

### D. Founder brand and marketing

**Flow:** verified project/research evidence → content brief → platform-specific draft → fact/privacy/IP review → founder approval → publish → record live URL → analyse.

Rules:
- Use the [brand module](../brand/README.md).
- Foundable can help prepare assets and publishing workflows; it is not a source of truth.
- Do not auto-publish or auto-reply by default.
- Never expose raw customer/lead data or unapproved claims.

### E. Customer onboarding and success

**Flow:** accepted scope → onboarding checklist → access/data permissions → delivery milestones → support/FAQ → issue triage → resolution → customer feedback → renewal/retention review.

Rules:
- Use only approved customer context and minimum necessary data.
- Follow customer-agreed policies for refunds, service credits and escalation.
- AI can draft support responses but cannot approve refunds, alter contracts or promise delivery dates.
- Escalate safety, security, billing, privacy, legal and high-impact issues to the founder.

### F. Operations and finance

**Flow:** task/cost capture → weekly review → exceptions → human decision → log/decision record.

Track:
- Time and API/tool costs per task or delivery.
- Lead-to-discovery, discovery-to-proposal and proposal-to-paid-pilot conversion.
- Delivery scope, rework, defects and support load.
- Revenue actually collected, expenses, refunds, taxes, margin and cash.
- Customer satisfaction/retention only when measured using a defined method.

Do not optimize agent count, prompt count, tokens or lines of code as business outcomes.

## 7. Task contract for every agent assignment

Use [agent-task-template.md](../templates/agent-task-template.md). Every task must state:
- One outcome and named role/owner.
- Context and authoritative files.
- Inputs and permitted tools/data.
- In-scope and explicitly out-of-scope work.
- Output format and acceptance criteria.
- Evidence required and sources to preserve.
- Data classification and allowed actions.
- Approval gates, escalation conditions and cost constraints.

No open-ended instruction such as "run the whole company" is a valid task.

## 8. Reusable playbooks and memory

When the same task is performed repeatedly:
1. Observe the human/agent workflow.
2. Record the steps, failure cases and evidence standard.
3. Ask a reviewer to challenge the playbook.
4. Save the approved procedure in the appropriate CR folder.
5. Update it when tools, providers or policies change.

Durable memory should be explicit:
- Business facts and decisions → CR docs.
- Current work and blockers → task board/issues.
- Reusable procedures → playbooks/templates.
- Customer-specific private context → approved private system.
- Temporary reasoning → task artifact or log, not assumed long-term memory.

## 9. Human approval and permission matrix

| Action | AI may prepare | AI may execute without per-action approval? |
|---|---|---|
| Public-source research | Yes | Yes, within scope and source rules |
| Internal draft and plan | Yes | Yes, in a draft/work branch |
| Modify a draft documentation file | Yes | Only in an authorised branch/task |
| Edit application code | Yes | Within scoped branch and test environment |
| Merge to main | Recommend | No, unless a narrowly defined repository policy explicitly authorises it |
| Production deploy / database migration | Prepare and verify plan | No |
| Send email, DM, call or sales follow-up | Draft and qualify | No |
| Publish post or website content | Draft and preview | No |
| Quote, contract or customer commitment | Prepare draft | No |
| Refund, payment, purchase or money movement | Analyse and recommend | No |
| Access customer/private data | Only with approved scope | No new access without founder approval |

Use least-privilege access. Do not grant a tool broader credentials than the current task requires.

## 10. Monitoring, escalation and stop conditions

- Every active task has one owner and a next checkpoint.
- "Urgent" must include impact, deadline and why it cannot wait.
- Stop and escalate when sources conflict, data is missing, permissions are insufficient, a task exceeds budget/scope, sensitive data appears, or the agent's output cannot be verified.
- Limit delegation depth; do not let agents spawn unlimited sub-agents or circular review chains.
- Use scheduled reviews that fit the work cadence. Do not create noisy checks that generate activity without decisions.
- For every production issue, preserve reproduction steps, impact, timeline, fix, tests and prevention action.

## 11. CR adoption roadmap

The dates below preserve CR's current commercial execution target of 1 February 2027. They are an internal preparation plan, not a new customer-launch promise.

### Phase 0 — Establish the operating rules (18–24 November 2026)
- Approve role ownership and task status definitions.
- Keep GitHub/CR as canonical documentation and use only sanitized public-repository records.
- Add the task brief and review templates.
- Identify what information must remain in a private system.
- Confirm which current tools are actually available and what permissions they have.

**Exit condition:** A task can be assigned, returned with proof, reviewed and recorded without relying on chat memory.

### Phase 1 — Run controlled research workflows (25 November–15 December 2026)
- Run one complete market/competitor research task using the researcher role.
- Run an independent challenge/review pass.
- Update the dated report, source register and decision record.
- Measure source verification, contradictions, missing evidence and reviewer rework.

**Exit condition:** Research outputs are traceable, falsifiable and useful for a founder decision.

### Phase 2 — Build repeatable internal routines (16 December 2026–10 January 2027)
- Create approved SOPs for research, planning, project implementation, QA and content drafting.
- Use a small number of reusable roles rather than a large bot fleet.
- Dry-run the delivery lifecycle using a non-customer project or safe prototype.
- Record tool usage and costs.

**Exit condition:** Work passes from brief to accepted artifact with clear ownership and no unauthorised external action.

### Phase 3 — Pre-execution readiness (11–31 January 2027)
- Review the commercial discovery plan and first target segment.
- Prepare private customer-data handling and lead-management arrangements.
- Rehearse proposal, pilot scope, onboarding, support and finance workflows.
- Confirm access, account ownership, payment and legal/compliance requirements using current reliable sources.

**Exit condition:** The founder can start the planned commercial execution with a defined workflow, not a collection of disconnected prompts.

### Phase 4 — Commercial operation (target: from 1 February 2027)
- Begin focused customer discovery.
- Select only an evidence-supported offer.
- Deliver a tightly scoped paid pilot before productising.
- Add SDR/customer-success/marketing automations only where actual repeated work justifies them.
- Review the system weekly and adapt from outcomes.

**Exit condition:** Repeatable, verified customer value and sustainable delivery economics—not merely a working demo.

## 12. Measures of success

| Function | Measure useful for CR | Vanity measure to avoid |
|---|---|---|
| Research | Verified source quality, hypotheses invalidated, time to a clear decision | Number of pages or prompts generated |
| Product | Evidence of buyer pain, completed discovery, paid pilot commitment | Number of feature ideas |
| Engineering | Acceptance-test pass rate, escaped defects, delivery reliability, rework | Lines of code or raw PR count |
| Sales | Qualified conversations, proposals, paid pilots, collected revenue | Raw lead volume or unsent email count |
| Marketing | Relevant audience conversations, portfolio visits, qualified referrals | Impressions alone |
| Customer success | Resolution quality, time to resolution, repeated issues, retention | Number of bot replies |
| Operations | On-time accepted work, blocker age, task cost and clear ownership | Number of autonomous runs |

## 13. Immediate next action

Use the role catalogue and task template to run one controlled internal task: independently re-evaluate the existing CR candidate opportunities and service lines, identify the strongest buyer/problem evidence still missing, and recommend the next discovery test. This must not silently select a product or begin external outreach.
