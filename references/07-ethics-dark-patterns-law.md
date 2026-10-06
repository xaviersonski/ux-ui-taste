# 07. Ethics, Dark Patterns and the Law

Persuasion helps people decide. Manipulation decides for them against their interest. This file draws the line, gives a fair alternative for every common dark pattern, and summarizes the legal landscape as of October 2026. It is general information and should not be treated as legal advice. Recommend that users confirm current rules with counsel for their markets.

## Contents
1. Three tests for any persuasive tactic
2. What the evidence says about dark patterns
3. Dark pattern catalog with fair alternatives
4. Sludge
5. Vulnerable users and children
6. Legal landscape (US, UK, EU)
7. How to raise ethics in an audit

---

## 1. Three tests for any persuasive tactic

Apply all three before recommending a tactic.

1. **Transparency test.** Would the tactic still work if the user knew exactly how and why it was used? Honest social proof passes. A fake countdown fails.
2. **Regret test.** Will users who acted on it be glad later? Look at refunds, cancellations, complaints and support contacts. Rising guardrail metrics mean the tactic is borrowing from the future.
3. **Symmetry test.** Is saying no as easy as saying yes? Is cancelling as easy as subscribing? Is "Reject all" as easy as "Accept all"?

If a tactic fails any test, replace it with the fair alternative below.

## 2. What the evidence says

- **Dark patterns work in the short term.** Luguri and Strahilevitz 2021 found mild dark patterns more than doubled sign-ups for a dubious service, and aggressive ones nearly quadrupled them. Aggressive patterns caused a strong backlash. Mild ones did not, which makes them both profitable and especially concerning. Less educated participants were more susceptible.
- **They are common.** Mathur et al. 2019 crawled about 11,000 shopping sites and found 1,818 dark pattern instances on 1,254 of them (about 11%), many of them deceptive.
- **They are now expensive.** The FTC's September 2025 settlement with Amazon over Prime enrollment and cancellation flows totaled $2.5 billion ($1 billion civil penalty and $1.5 billion in refunds), and required a clear decline button and a simpler cancellation. Epic Games paid $245 million in 2023 over dark patterns that led to unwanted purchases.
- **Short-term lift hides long-term cost.** Trust damage, chargebacks, churn, reviews, regulator attention and brand harm don't show up in a two-week A/B test. Always pair conversion metrics with guardrails.

## 3. Dark pattern catalog with fair alternatives

Terms follow Brignull's deceptive.design taxonomy and Mathur et al. 2019.

| Dark pattern | What it looks like | Fair alternative |
|---|---|---|
| Hidden costs / drip pricing | Fees, taxes or shipping appear only at the last step | Show the total including mandatory fees from the first price display |
| Sneak into basket | Items or insurance added without the user choosing | Offer add-ons as unticked options with clear prices |
| Preselection | Pre-ticked boxes for marketing, extras or data sharing | Unticked boxes, with a clear benefit statement |
| Hidden subscription | A one-off purchase silently enrolls the user in recurring billing | Explicit subscription choice, with price, frequency and renewal date stated next to the button |
| Roach motel / hard to cancel | Easy to join, hard to leave (phone-only cancel, many screens) | Cancel online in the same channel and with similar effort as signup. One optional retention offer at most |
| Confirmshaming | "No thanks, I don't like saving money" | Neutral decline ("No thanks") |
| Trick questions | Double negatives, confusing checkbox wording | Plain, positively worded choices |
| Visual interference / asymmetric choice | "Accept" as a bright button, "Decline" as faint grey text | Equal visual weight for yes and no in consent and enrollment choices |
| Fake urgency | Countdown timers that reset, "offer ends soon" with no end | Real deadlines, the same for everyone |
| Fake scarcity | "Only 2 left!" when not true | Real stock data, or nothing |
| Fake social proof | Invented reviews, fake "Sarah from Leeds just bought" pop-ups | Real reviews and real, verifiable activity |
| Nagging | Repeated prompts after the user said no | Respect "no" for a reasonable period. Offer "don't ask again" |
| Forced action / forced registration | Account required before seeing prices or to buy | Guest access. Offer an account when it benefits the user |
| Obstruction | Making comparison, data export or privacy settings hard | Easy export, clear privacy controls, transparent comparisons |
| Disguised ads | Ads styled as content or as navigation | Clear labeling of sponsored content |
| Bait and switch | Advertised price or feature unavailable when the user arrives | Honest availability and pricing |
| Privacy zuckering | Defaults that over-share data | Privacy-protective defaults, opt-in for sharing |
| Free trial trap | No reminder before conversion, card charged silently | Reminder a few days before the trial ends, with a one-click cancel link |

## 4. Sludge

**What it is.** Sunstein's term for excessive friction that makes it hard to do something in your own interest (claim a refund, cancel, opt out, access a benefit). It is the mirror image of a helpful nudge.

**Apply.**
- Audit flows users want to complete but the business might not want them to (cancellation, refund, downgrade, data deletion). Count the steps and compare with signup.
- Remove unnecessary verification, phone calls, and repeated confirmations.

**Audit question.** For every action that benefits the user but not the business, is the effort comparable to the reverse?

## 5. Vulnerable users and children

- Luguri and Strahilevitz found less educated users more susceptible to mild dark patterns. Older users, users in financial stress, and people with cognitive disabilities are often more affected.
- Products likely to be used by children face specific rules (UK Age Appropriate Design Code, EU DSA protections for minors, US COPPA). Avoid engagement-maximizing mechanics, nudges toward weaker privacy, and in-app purchase pressure.
- The EU's planned Digital Fairness Act specifically targets addictive design and gamification aimed at minors.

## 6. Legal landscape (status as of October 2026)

Laws change fast. Treat this as orientation and recommend checking current status.

**United States**
- **FTC Act Section 5** prohibits unfair or deceptive practices, and the FTC applies it to dark patterns (see its 2022 staff report "Bringing Dark Patterns to Light").
- **ROSCA** (Restore Online Shoppers' Confidence Act) requires clear disclosure of material terms, express informed consent before charging, and simple cancellation for online negative-option subscriptions. The Amazon settlement above was brought under ROSCA and the FTC Act.
- The FTC's broader 2024 "click-to-cancel" rule was vacated by the Eighth Circuit in July 2025, but ROSCA enforcement continues and many states have their own auto-renewal laws (California's was strengthened in 2025 to require online cancellation).
- **FTC rule on fake reviews and testimonials** (effective October 2024) bans fake reviews, buying reviews and fake social media indicators.
- **FTC rule on unfair or deceptive fees** (effective May 2025) requires upfront total pricing for live-event tickets and short-term lodging.

**United Kingdom**
- **Digital Markets, Competition and Consumers Act 2024 (DMCCA).** Since April 2025 the CMA can directly fine firms up to 10% of global turnover for consumer law breaches. Drip pricing and fake reviews are banned outright. New subscription contract rules (clear pre-contract information, reminders, easy exit) are expected to follow secondary legislation, with commencement expected after autumn 2026.
- **UK GDPR and PECR** govern consent, cookies and marketing.

**European Union**
- **Unfair Commercial Practices Directive** covers misleading and aggressive practices. Commission guidance (2021) applies it to dark patterns.
- **Digital Services Act Article 25** prohibits online platforms from designing interfaces that deceive, manipulate or impair users' free choice.
- **GDPR** requires freely given, specific, informed, unambiguous consent. Pre-ticked boxes are invalid (Planet49, 2019).
- **Consumer Rights Directive amendments** (Directive 2023/2673) require a clearly labeled withdrawal function for online contracts from 19 June 2026.
- **Digital Fairness Act.** The Commission's legislative proposal is expected in late 2026, targeting dark patterns, addictive design, unfair personalization, subscription traps and influencer marketing. Formal adoption is unlikely before 2027.
- **European Accessibility Act** has applied since 28 June 2025 to e-commerce and other covered services (see 06).

## 7. How to raise ethics in an audit

- List ethical and legal risks in their own section, separate from usability findings, so they can't be traded away for conversion.
- Name the pattern, the likely legal exposure in plain terms, and the fair alternative.
- Show the business case for the fair version (trust, lower refunds and chargebacks, reviews, regulatory risk avoided, retention of willing customers).
- Suggest guardrail metrics so the team can see hidden costs.
- Stay matter-of-fact. Many dark patterns are inherited or accidental.
