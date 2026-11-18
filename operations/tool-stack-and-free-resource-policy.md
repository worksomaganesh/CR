# CR Tool Stack and Free-Resource Policy

**Decision date:** 18 November 2026  
**Status:** Accepted with conditions  
**Review cadence:** Monthly and whenever a provider changes pricing, limits, terms or model availability.

## 1. Decision

CR follows a **free-first, value-first** tool strategy:

- Use existing subscriptions and genuinely free tiers as much as they produce useful, verifiable work.
- Pay only when a tool removes a real bottleneck that free resources cannot reasonably handle.
- Use free resources within provider limits, terms, privacy settings and eligibility rules.
- Do not create extra accounts, rotate emails, repeatedly claim trials or otherwise evade quotas.
- Do not spend a quota merely to exhaust it. Optimize accepted work and business value per rupee—not raw prompts, tokens, agent steps or lines of code.
- Keep the stack small enough to operate, review and secure.

The objective is not "zero spending forever". It is **minimum justified cost while maintaining quality, security and delivery reliability**.

## 2. Current tool register

| Tool / entitlement | Status | Best CR use | Limits / conditions |
|---|---|---|---|
| Codex on ChatGPT Free | Existing free entitlement | Scoped code changes, tests, documentation, small debugging tasks and code review assistance | Codex is included on Free, with limited usage. OpenAI's current model table lists GPT-5.6 Terra for Codex on Free/Go; GPT-5.6 Luna is the default ChatGPT Free model, not the Codex Free model in that table. Codex Cloud is not included on Free/Go. Verify the account's model selector and allowance. |
| Google AI Pro through Jio | Existing partner entitlement, if previously claimed and still eligible | Gemini app reasoning, Deep Research, writing, Flow, NotebookLM and the included Google developer tools | New claims have ended. Existing successful claimants can continue the 18-month benefit while continuously maintaining an eligible unlimited 5G plan of ₹349 or more. Model and feature availability are product-surface-specific. |
| Gemini Argon 4 in Gemini app | Use when visibly available in the user's account | Deep research, architecture critique, complex reasoning and adversarial review | Treat the account's current UI as the model-availability check. Do not assume this model is available in Antigravity, Gemini CLI or Gemini API. |
| Gemini Code Assist / Gemini CLI | Included higher daily limits where activated under the Jio benefit | Coding assistance and terminal tasks | Check actual account activation, model availability and quotas. |
| Gemini API / Google AI Studio Free | Free tier for eligible models | Small experiments, synthetic-data prototypes, evaluation and low-risk integrations | Only selected models are free. Argon is not an API Free-tier model. Google says Free-tier content may be used to improve products. Never send confidential/customer data on the Free tier. |
| GitHub Student Developer Pack / Copilot Student | Student offer; apply and verify | Coding assistance, GitHub Pro, Codespaces and relevant partner tools | Requires active student verification; partner terms and offer periods differ. Offers cannot be redeemed multiple times or reset by creating extra accounts. |
| Cloudflare Workers Free | Free tier | Lightweight APIs, webhooks and small scheduled jobs | Current published Free limits include 100,000 requests/day and 10 ms CPU time per request. Check limits and data terms before production use. |
| Supabase Free | Free tier | Prototypes, demos and non-critical experiments | Current published limits include two active projects, 500 MB database per project and 5 GB egress; projects can pause after one week of inactivity. No automatic backups on Free. Not a sole datastore for critical customer workloads without a recovery plan. |
| Vercel Hobby | Free personal/non-commercial tier | Personal portfolio and non-commercial prototypes | Its terms restrict Hobby to personal or non-commercial use. Do not use it for CR paid client deployments. |
| Grok Bot Premium | Conditional paid one-month test; not yet activated | Delegated multi-step browser/computer tasks, recurring internal routines and bounded operational work | Official Grok Bot page lists Premium at USD $30/month, Super at $100/month and Ultra at $200/month. Start with Premium only after 18+ eligibility, local checkout verification, privacy/security review and a concrete test plan. Usage is limited; verify the exact allowance and billing controls in the account. |

The register is a planning baseline, not proof that every offer is enabled. Verify each actual entitlement before assigning critical work.

## 3. Codex Free: correct use

Use the Free allowance for bounded tasks where the available Codex model and context are sufficient:
- Documentation, tests, scripts, boilerplate and routine code edits.
- Small implementation issues with clear acceptance criteria.
- Explaining unfamiliar code and preparing change plans.
- Generating test cases and inspecting narrow diffs.

For larger or risky tasks:
1. Ask a stronger available reasoning model to critique the plan and identify risks.
2. Break implementation into small tasks.
3. Use Codex Free for suitable implementation work.
4. Run actual tests and request an independent review.
5. Require human approval before merge, production deployment or destructive changes.

Do not dismiss the model only because it is included in Free; judge it against the task's acceptance criteria. Do not assume generated code is tested because the agent says it is.

### Account and usage rule

OpenAI's Terms prohibit circumventing rate limits or restrictions. Do not switch to another email/account to reset Codex Free usage. Do not automate account creation or trial cycling. Wait for the official reset, use another legitimately available benefit, or propose a budgeted paid option.

## 4. Google AI Pro via Jio

Keep an already claimed Jio Google AI Pro entitlement active while useful and eligible. Jio states that the offer is no longer open to new claims; existing successful claimants can continue the 18-month benefit provided they continuously maintain an eligible unlimited 5G plan of ₹349 or more.

Use Gemini app models that the account actually displays. Keep these surfaces separate:
- Gemini consumer app: use Argon 4 if it is visibly available in the current account.
- Gemini Code Assist / CLI: use the higher daily limits actually activated on the account.
- Antigravity: do not assume the Jio partner promotion grants every premium model there; verify the model selector and current eligibility.
- Gemini API / AI Studio: API billing and free-tier availability are separate from the consumer AI Pro subscription. Argon 4 is not on the API Free tier. Free-tier content may be used to improve Google's products, so use only public or synthetic data.

## 5. Grok Bot purchase decision

**Decision:** Conditionally approve a one-month test of Grok Bot Premium; do not buy a higher tier initially.

The official Grok Bot product page currently lists:
- Premium — USD $30/month; includes its own computer, sign-in to tools, scheduled routines, desktop/mobile access and a weekly usage allowance.
- Super — USD $100/month; 3.5× Premium usage.
- Ultra — USD $200/month; 12× Premium usage.

Other eligible subscriptions may bundle Grok Bot; do not assume an X/Grok app subscription and a Grok Bot plan are interchangeable. Verify the exact checkout offer, billing owner, weekly allowance, included model use and any separate Cursor/on-demand charges in the account.

### Purchase gates

Do not use or buy Grok Bot for the founder's own access until:
1. The user meets Grok Bot's minimum age requirement: 18 or the higher local age of majority.
2. The official purchase route and actual Indian checkout price/taxes are verified.
3. A one-month test has at least three specific workflows and measurable acceptance criteria.
4. Cloud-computer data handling, shared-account behaviour and approval settings have been reviewed.

Start with Premium only, monthly. No annual billing, Super/Ultra tier or top-up credits are approved initially. Renew only if accepted work creates measurable value beyond the cost.

### Usage and spend controls

- Leave Auto Top-up off.
- Set the monthly additional-usage/spending cap to zero or the lowest acceptable amount.
- Check weekly usage before long-running tasks.
- Split work into small bounded tasks; one large run may consume substantial allowance.
- Review actual usage and accepted outputs weekly.
- Cancel/decline renewal if it does not outperform the existing free stack on useful tasks.

### Privacy and security controls

Grok Bot uses a persistent cloud computer. All Bots under the same user account share its files, browser sessions and command-line credentials. The product requires data storage and does not support Legacy Privacy Mode.

For the initial test:
- Use a dedicated work environment/account with minimum necessary logins.
- Do not connect personal banking, payment, password-manager or unrelated personal accounts.
- Do not provide customer documents, personal data, confidential leads, private correspondence, production secrets or customer credentials before reviewing data terms and receiving explicit founder approval.
- Use public/sanitized CR documents and synthetic examples for initial tests.
- Keep local-computer access at Ask-every-time or Never unless a specific task requires it.
- Add narrow Ask-first rules for external email/DMs, publishing, prospect outreach, purchases, payments, file deletion, permissions/security changes, GitHub merges, production releases and database migrations.
- Avoid broad "Always allow" rules.
- Never paste passwords, one-time codes or API keys into normal chat; use provider-supported secure secret flows where appropriate.

Auto Review is a safeguard, not a substitute for checking the exact action, target, data and consequences.

## 6. Student benefits

Apply for the GitHub Student Developer Pack using genuine student status and institution-issued proof. If verified, activate eligible benefits such as Copilot Student, Codespaces and relevant partner offers.

GitHub's Pack includes many changing third-party offers. Each partner may impose different age restrictions, expiry, usage caps, renewal conditions and data policies. GitHub requires active student verification, says benefits cannot be redeemed multiple times, and prohibits creating another account to reset a time-limited offer.

Claim only resources that solve an active CR need. Do not connect every offered service.

## 7. Resource-selection checklist

For each new free tool or credit:
1. Name the exact CR workflow it solves.
2. Check whether an existing tool already does it adequately.
3. Verify official Free/Student/Trial terms, geography and account eligibility.
4. Check data use, retention, training, security and deletion terms.
5. Record hard quotas, expiry, pause behaviour and automatic overage billing.
6. Classify the data as public, synthetic, internal or confidential.
7. Set billing alerts/caps before enabling paid usage.
8. Record a reset/expiry date and review whether the benefit remains useful.

Do not add a payment method or enable API billing unless the founder approves the budget and spending limit. Keep API keys in environment variables/secret storage, never Git.

## 8. Initial task routing

| Task | Primary route | Fallback / review |
|---|---|---|
| Deep market research | Gemini Argon in consumer app, if available | Gemini Deep Research / other permitted sources; independent source audit |
| Quick code change | Codex Free | Gemini Code Assist/CLI if enabled; tests and diff review |
| Complex implementation plan | Argon in Gemini app | Codex planning/review; human acceptance |
| Routine documentation | Codex Free | ChatGPT Free |
| Multi-step browser/computer task | Grok Bot after eligibility and purchase | Human-operated browser or scoped manual workflow |
| Website/social draft | Foundable or existing tools | Founder review and manual publication |
| Prototype API/backend | Cloudflare Workers / Supabase Free where appropriate | Local mock or another compliant free tier |
| Student developer tooling | GitHub Student Developer Pack | Existing GitHub Free tools |
| Customer-facing/production workload | Select based on customer SLA, privacy, reliability and cost | Do not assume a Hobby/free tier is suitable |

## 9. Resource ledger

For each tool, record provider/product, account entitlement, intended workflow, plan type, quota/reset/expiry, permitted data class, auto-billing status/spend cap, accepted outputs, fallback tool, review date and keep/pause/cancel/upgrade decision.

## 10. Review criteria

Review monthly:
- Which tools produced accepted CR outputs?
- What useful work was completed per rupee?
- Which limits were reached naturally while completing valuable work?
- Did any tool cause rework, privacy risk or operational dependency?
- Did Grok Bot complete work that the free stack could not reasonably do?
- Can any unused subscription be cancelled?

The goal is not maximum tool usage. It is a lean, reliable and compliant AI-native company operating system.

## Official references checked on 18 November 2026

- OpenAI Codex availability and model selection: https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan and https://help.openai.com/en/articles/20001354-gpt-6-and-other-models-in-chatgpt
- OpenAI Terms of Use: https://openai.com/policies/terms-of-use/
- Grok Bot product/pricing: https://x.ai/bot
- Grok Bot terms: https://x.ai/legal/grok-bot-terms
- Grok Bot approvals/security/privacy: https://docs.x.ai/grok-bot/approvals-security-and-privacy
- Grok Bot computer and shared-account behaviour: https://docs.x.ai/grok-bot/computer-and-apps
- Grok Bot usage and top-ups: https://docs.x.ai/x-subscription/extra-usage and https://docs.x.ai/x-subscription/spending-caps
- Jio Google AI Pro offer: https://www.jio.com/help/faq/mobile/offers/google-gemini-offer/
- Gemini API pricing/data use: https://ai.google.dev/gemini-api/docs/pricing
- GitHub Student Developer Pack: https://education.github.com/pack/ and https://docs.github.com/en/education/about-github-education/github-terms-and-conditions-for-the-student-developer-pack
- Cloudflare Workers limits: https://developers.cloudflare.com/workers/platform/limits/
- Supabase pricing: https://supabase.com/pricing
- Vercel terms: https://vercel.com/legal/terms
