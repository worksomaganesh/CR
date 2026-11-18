# Decision — Free-First Tooling and Conditional Grok Bot Purchase

**Date:** 18 November 2026  
**Status:** Accepted with conditions  
**Owner:** Founder  
**Review date:** 18 December 2026, then monthly

## Context

The founder wants CR to maximise the useful capacity of legitimately available free tools and existing subscriptions, while paying selectively for Grok Bot because its persistent computer and agent workflows may enable useful delegation.

Current stated baseline: Codex on ChatGPT Free and Google AI Pro through a Jio offer. Grok Bot is the proposed paid tool. CR must keep starting costs low and avoid overlapping subscriptions.

## Decision

Adopt a **free-first, value-first** tooling strategy, with Grok Bot approved only as a conditional one-month Premium test after eligibility and security gates are satisfied.

### 1. Existing tools

- **Codex Free:** Use included limits for scoped coding, tests, documentation, small bug fixes and review assistance. OpenAI currently says Codex is included in Free; its model table lists GPT-5.6 Terra for Codex on Free/Go. GPT-5.6 Luna is the default ChatGPT Free model, not the Codex Free model listed in that table. Codex Cloud is not included on Free/Go. Verify the actual account UI.
- **Google AI Pro via Jio:** Retain the existing valid entitlement. Use Argon 4 in the Gemini consumer app when it is visibly available for the account. Do not assume identical entitlement in Antigravity, Gemini CLI or API.
- **Gemini Code Assist / CLI:** Use only where the existing Jio entitlement is activated and model/rate limits are visible.
- **Gemini API / AI Studio Free:** Use eligible free-tier models for experiments with public or synthetic data. Argon 4 is not on the API Free tier; Google says Free-tier content may be used to improve products.
- **GitHub Student Developer Pack:** Apply using genuine student status and redeem useful benefits only once under provider terms.
- **Other free infrastructure:** Evaluate Cloudflare Workers Free and Supabase Free when they fit a specific prototype. Vercel Hobby is personal/non-commercial and must not host CR paid client deployments.

### 2. Do not circumvent free-tier limits

Do not use additional email accounts to reset Codex Free or other provider quotas. Do not cycle trials, duplicate student redemptions or otherwise bypass provider restrictions. OpenAI Terms prohibit circumventing rate limits/restrictions. Use official resets, another legitimately available entitlement or an approved paid option.

"Use the full free potential" means completing valuable work within the allowance, not sending unnecessary prompts just to exhaust a quota.

### 3. Conditionally approve Grok Bot Premium

The official Grok Bot page currently lists Premium at USD $30/month, Super at $100/month and Ultra at $200/month. Premium includes the Bot's own computer, tool sign-ins, scheduled routines, desktop/mobile access and a weekly usage allowance. Higher tiers are not approved for initial use.

Approve only:
- One monthly Premium test, through the official provider channel.
- Confirm the actual Indian checkout price, GST/taxes, subscription owner and exact usage allowance before purchase.
- No annual billing, Super/Ultra tier, top-up credits or auto-top-up initially.
- Review the usage dashboard weekly and renew only if accepted work proves value beyond the cost.

**Eligibility gate:** The Grok Bot Terms require each user to be at least 18 years old (or the higher local age of majority). The founder must not access or use Grok Bot before meeting this requirement. Payment by another person does not remove the age restriction.

### 4. Data and action controls

Grok Bot's persistent cloud computer is shared among all Bots on the same user account: browser sessions, files and command-line credentials are available across that Bot roster. Grok Bot requires data storage and does not support Legacy Privacy Mode.

For the first test:
- Use a dedicated work environment with minimum necessary accounts and permissions.
- Use public/sanitized documents and synthetic datasets.
- Do not connect customer-sensitive files, private leads, production secrets, personal banking or unrelated personal accounts before reviewing data terms and approving access.
- Keep local computer access Ask-every-time or Never unless a specific task requires it.
- Require Ask-first approval for messages, publishing, prospect outreach, purchases, payments, file deletion, permission changes, GitHub merges, production deployments and database migrations.
- Never paste passwords, one-time codes or API keys into ordinary chat.

### 5. Free-resource register

Maintain an operating register of legitimate offers, quota/reset dates, expiry, privacy/data terms, auto-billing status, accepted outputs and fallback tools. Candidate resources include GitHub Student Developer Pack, Gemini API/AI Studio Free tier (eligible models only, public/synthetic data), Cloudflare Workers Free and Supabase Free. Verify each provider's limits and terms at the time of use.

## Alternatives considered

- **Pay for several AI tools immediately:** rejected due to cost and overlap.
- **Buy Grok Bot Super/Ultra immediately:** rejected until Premium shows a real usage bottleneck.
- **Rotate email accounts after Codex limits:** rejected because that attempts to bypass provider restrictions.
- **Use only free tools forever:** rejected; justified spending may improve reliability, speed or delivery after a real bottleneck is measured.
- **Exhaust every free allowance regardless of value:** rejected as wasteful and potentially inconsistent with provider terms.

## Consequences

- CR measures accepted work and cost/value, not usage volume.
- Tool choice can vary by task; no single model is a single point of failure.
- Grok Bot is not assumed to automate "half the business". Its value is measured through a controlled test.
- Jio AI Pro entitlement is retained while valid; model availability differs by product surface.
- Provider plans, pricing, limits and terms must be rechecked monthly.

## Success criteria for the Grok Bot test

After the founder becomes eligible and activates the one-month test, evaluate at least three internal workflows:
1. Source-linked market/competitor research preparation.
2. A multi-step browser/computer task using only approved services.
3. Internal operations/documentation coordination.

Measure task completion, accuracy, verification effort, time saved, usage consumed, cost and founder interventions. No external prospect outreach, public publishing, payments or production changes without exact founder approval.

## Reversal criteria

Do not start or renew if:
- Eligibility or checkout conditions are not met.
- Actual local cost is not justified.
- Usage is consumed too quickly.
- Quality/rework outweigh time saved.
- Privacy settings or permissions are unacceptable.
- The tool does not outperform the existing free stack on useful tasks.

Consider a higher tier only after two consecutive monthly reviews show that more included usage is consistently necessary and economically justified.
