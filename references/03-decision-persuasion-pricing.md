# 03. Decision-Making, Persuasion, Trust and Pricing

How people choose, and how to help them choose well and confidently. Read `07-ethics-dark-patterns-law.md` alongside this file. Every tactic here has a manipulative version, and the line is covered there.

## Contents
1. Defaults
2. Anchoring
3. Decoy (asymmetric dominance) effect
4. Compromise and center-stage effects
5. Framing
6. Loss aversion
7. Zero price effect
8. Pain of paying
9. Total cost transparency, partitioned and drip pricing
10. Charm pricing and left-digit bias
11. Temporal reframing (pennies a day)
12. Annual vs monthly plans
13. Social proof
14. Reviews and ratings
15. Credibility and trust signals
16. Trust at the moment of payment
17. Scarcity
18. Urgency and deadlines
19. Reciprocity
20. Commitment and consistency (foot in the door)
21. Risk reversal (trials, guarantees, returns)
22. Endowment effect and ownership
23. Status quo bias and switching costs
24. Comparison and decision aids
25. Personalization and recommendations
26. Consent and opt-in

---

## 1. Defaults
**Evidence** A. Jachimowicz, Duncan, Weber and Johnson 2019 meta-analysis of 58 studies (n 73,675) found d = 0.68 with large variation between studies. Defaults work best when seen as an endorsement (what the designer recommends) or as the status quo. Classic field examples are pension auto-enrollment (Madrian and Shea 2001) and organ donation (Johnson and Goldstein 2003).

**Apply.**
- Preselect the option that is best for most users (recommended plan size, standard delivery, sensible privacy settings).
- Label it as recommended and say why ("Most teams of your size choose this").
- Make alternatives visible and one click away.
- Use defaults for things that help users later (autosave, backups, security features on).

**Limits.** Defaults that benefit the business at the user's cost (pre-ticked insurance, add-ons, marketing consent, auto-renew hidden in small print) are dark patterns and frequently unlawful. Defaults change choices more reliably than long-term outcomes.

**Audit question.** Would most users, fully informed, pick each default themselves?

## 2. Anchoring
**Evidence** A (Tversky and Kahneman 1974, replicated in Many Labs).

**What it says.** The first number people see shapes how they judge later numbers.

**Apply.**
- On pricing pages, ordering plans from high to low price can make the middle and lower tiers feel more reasonable. Test it, since effects vary.
- Show a real reference price (genuine previous price, the cost of the problem, the price of alternatives such as hiring someone).
- Show savings against a real comparison ("£96 a year, save £24 against monthly").

**Limits.** Fake "was" prices and inflated reference prices are illegal in the UK, EU and US.

**Audit question.** What is the first number the user sees, and is it a fair reference?

## 3. Decoy (asymmetric dominance) effect
**Evidence** B to C. Huber, Payne and Puto 1982 established it. Frederick, Lee and Baskin 2014 found it weakens or disappears with realistic, visually presented options. Effects in real product pages are smaller and less reliable than textbook examples suggest.

**What it says.** Adding an option that is clearly worse than one target option (but not another) can push choice toward the target.

**Apply.**
- Design tiers so each has a clear reason to exist, and the recommended tier is plainly the best value for most users.
- If testing a decoy tier, check that it is a real product someone could sensibly buy.

**Limits.** Fake tiers meant only to steer are manipulative and erode trust once noticed.

**Audit question.** Does every plan serve a real customer segment?

## 4. Compromise and center-stage effects
**Evidence** B (Simonson 1989 compromise effect. Valenzuela and Raghubir 2009 center-stage effect).

**What it says.** People lean toward middle options when uncertain, and toward items in the center of a display.

**Apply.**
- Put the recommended plan in the middle with a single highlight.
- In three-tier pricing, the middle plan is a natural default for uncertain buyers.

**Audit question.** Is the plan most users should pick placed and highlighted where uncertain users naturally look?

## 5. Framing
**Evidence** A in lab settings (Tversky and Kahneman 1981). B in marketing contexts.

**What it says.** The same fact presented as a gain or a loss, or in different units, changes choices.

**Apply.**
- Frame benefits in terms users care about (time saved per week, money saved per year).
- "95% fat free" feels different from "5% fat". Choose the frame that helps understanding, then check it isn't misleading.
- Frame the next step as small and concrete ("Takes 2 minutes").

**Limits.** Framing that hides material facts is deceptive.

**Audit question.** Is each claim framed in the user's terms, and is the frame honest?

## 6. Loss aversion
**Evidence** B. Classic prospect theory (Kahneman and Tversky 1979) puts losses at about twice the weight of gains. Gal and Rucker 2018 argue the effect is less general than claimed, and it varies by context and stakes.

**Apply.**
- Show what users keep or would lose in honest terms when relevant (saved work, unused credit, data that will be deleted on downgrade).
- In trials, remind users what they built during the trial before it ends.

**Limits.** Guilt-tripping on cancellation ("You'll lose everything!" when they won't) is confirmshaming. Keep loss framing factual.

**Audit question.** Are any loss messages exaggerated or used to shame?

## 7. Zero price effect
**Evidence** B (Shampanier, Mazar and Ariely 2007).

**What it says.** People overvalue free items relative to even very cheap ones. A price of zero changes how the choice feels.

**Apply.**
- Free shipping often outperforms an equivalent price cut. A free shipping threshold can raise basket size.
- Free tiers and free trials lower the barrier to starting.
- "Free" must be truly free. Hidden conditions destroy trust and may be illegal.

**Audit question.** Is there a natural place to offer something genuinely free that removes the biggest barrier?

## 8. Pain of paying
**Evidence** B (Prelec and Loewenstein 1998. Prelec and Simester 2001 found willingness to pay rises with credit cards over cash).

**What it says.** Paying feels like a loss. Separating the payment from the consumption, or making it less salient, reduces the pain.

**Apply.**
- Saved payment methods and wallets (Apple Pay, Google Pay, PayPal) reduce effort and pain at checkout.
- Bundle where it genuinely simplifies (one price for everything).
- Charge after value is delivered where the model allows.

**Limits.** Don't obscure that a charge will happen. Automatic renewal must be clear and agreed to.

**Audit question.** How many steps and how much effort does paying take, and is a one-tap option available?

## 9. Total cost transparency, partitioned and drip pricing
**Evidence** B. Baymard's surveys of US shoppers rank "extra costs too high (shipping, tax, fees)" as the top fixable reason for abandonment, cited by 40% of those who abandoned (excluding the just-browsing group), and 12% cite being unable to see the total cost up front. Blake et al. 2021 (StubHub field experiment) showed hiding fees until checkout raises spending, which is exactly why regulators now ban it.

**What it says.** Surprise costs late in the flow feel like a betrayal and drive abandonment. Drip pricing can raise short-term revenue but now carries legal risk (UK DMCC Act, US FTC rule on junk fees for live events and lodging, EU consumer law).

**Apply.**
- Show the full price including mandatory fees from the first price display.
- Show shipping cost or a shipping calculator on the product page and in the cart.
- Show delivery dates early (slow delivery is the second biggest reason at 20% in Baymard data).

**Audit question.** Does the price the user first sees equal what they pay, apart from optional extras they chose?

## 10. Charm pricing and left-digit bias
**Evidence** B (Thomas and Morwitz 2005. Field evidence on left-digit bias in used car prices and retail).

**What it says.** £9.99 is perceived as closer to £9 than to £10.

**Apply.**
- Charm prices can help in value-oriented markets. Round prices signal quality and simplicity in premium positioning and are easier to process.
- Be consistent within a product.

**Audit question.** Does the pricing format match the brand's position?

## 11. Temporal reframing
**Evidence** B (Gourville 1998, pennies-a-day framing).

**What it says.** Expressing a cost in small, frequent units can make it feel smaller.

**Apply.**
- "£8 a month" or "less than a coffee a week" can help justify subscriptions when the underlying price is clear.
- Always show the actual billed amount and frequency next to the reframe.

**Audit question.** Is the real billed amount always visible next to any reframed price?

## 12. Annual vs monthly plans
**Evidence** C (widely used, outcomes vary by product).

**Apply.**
- Show the annual saving clearly ("2 months free"). Defaulting the toggle to annual can raise annual uptake. Test it, and be clear about the upfront charge.
- Let users switch between views without losing their place.

**Audit question.** Is it obvious what will be charged today and when the next charge will occur?

## 13. Social proof
**Evidence** B. Cialdini's work and Goldstein, Cialdini and Griskevicius 2008 (hotel towel reuse with descriptive norms). Norm-based nudges at scale produce real but modest effects (Allcott 2011 found about 2% energy reduction from home energy reports).

**What it says.** People look to others' behavior when unsure.

**Apply.**
- Specific beats vague. "4,200 accounting firms use this" beats "Trusted by thousands".
- Similar others work best. Show customers like the visitor (same industry, size, role).
- Place proof near the decision (testimonial next to the pricing CTA, rating next to add-to-cart).
- Use logos, case studies with numbers, ratings, and user counts when they are true.

**Limits.** Fake reviews, fake counters and fake "X people are viewing this" notices are illegal in the UK (DMCC Act), banned by the FTC's 2024 rule on fake reviews, and erode trust. Social proof highlighting that many people do the wrong thing can backfire ("most people don't pay on time").

**Audit question.** Is the social proof specific, real, relevant to this visitor and placed at the point of decision?

## 14. Reviews and ratings
**Evidence** B (Northwestern Spiegel Research Center with PowerReviews. Purchase likelihood for a product with five reviews was about 270% higher than with none. Purchase likelihood peaked at average ratings of 4.2 to 4.5 and fell toward 5.0, as perfect scores looked too good to be true. Effects were larger for higher-priced products).

**Apply.**
- Get products to at least a handful of reviews quickly (post-purchase prompts, sampling programs with disclosure).
- Show the rating distribution, not just the average. Let users filter to negative reviews.
- Show verified-buyer badges, review dates and reviewer context (size worn, use case).
- Don't suppress negative reviews. A few honest negatives raise credibility.
- Respond publicly to criticism.

**Audit question.** Can users see enough real, recent and varied reviews to trust the rating?

## 15. Credibility and trust signals
**Evidence** B (Fogg et al. 2003, Stanford web credibility research, found design look was the most commonly cited credibility factor. Baymard trust research).

**Apply.**
- Professional, consistent, error-free design. Typos and broken elements undermine trust fast.
- Real contact details, physical address, company info, and easy-to-find policies (returns, privacy, terms).
- Clear "who we are" and real team or founder presence where relevant.
- Third-party validation (press, certifications, awards, security audits) when real.
- Keep content current. Outdated copyright years and stale blog posts signal neglect.

**Audit question.** Would a skeptical first-time visitor find enough evidence that this is a real, competent and accountable company?

## 16. Trust at the moment of payment
**Evidence** B (Baymard. 19% of US shoppers who abandoned cited not trusting the site with card details).

**Apply.**
- Visually reinforce the payment area (a bordered section, lock icon, "secure payment" wording, recognized payment logos). Users judge security by how the page looks.
- Keep the checkout visually consistent with the rest of the site. Unexpected redirects or styling changes raise suspicion.
- Show recognizable payment options and trust seals near card fields.
- Explain why you need sensitive data (phone number "for delivery updates only").

**Audit question.** Does the payment step look and feel at least as secure as the rest of the site?

## 17. Scarcity
**Evidence** B (Worchel, Lee and Adewole 1975 cookie jar study. Real scarcity raises perceived value).

**Apply.**
- Show real stock levels when low ("3 left in your size") because it helps users decide.
- Limited editions and capacity limits, only when genuine.

**Limits.** Fake or perpetual scarcity is deceptive and illegal in many jurisdictions. Mathur et al. 2019 found many fake scarcity and urgency messages on shopping sites.

**Audit question.** Is every scarcity message true and tied to real data?

## 18. Urgency and deadlines
**Evidence** B to C (deadlines prompt action, Ariely and Wertenbroch 2002 on self-imposed deadlines. Fake countdowns are a common dark pattern).

**Apply.**
- Real deadlines (sale ends, order by 2pm for next-day delivery) are helpful information.
- "Order within 2 hrs 14 mins for delivery tomorrow" is honest urgency that serves the user.

**Limits.** Countdown timers that reset are illegal deception.

**Audit question.** Is every deadline real and the same for every user?

## 19. Reciprocity
**Evidence** B (Regan 1971. Cialdini).

**What it says.** People feel inclined to return favors.

**Apply.**
- Give real value before asking (useful free tools, free content, a free tier, a genuinely helpful onboarding).
- Ask for a review or referral right after delivering a success moment.

**Limits.** Gifts with hidden strings feel manipulative. Keep the value real and the ask light.

**Audit question.** Have we given the user something useful before asking for something?

## 20. Commitment and consistency (foot in the door)
**Evidence** B, small effects (Freedman and Fraser 1966. Burger 1999 meta-analysis found a small but reliable effect).

**What it says.** A small first commitment makes a larger related one more likely.

**Apply.**
- Start flows with an easy, engaging first question (goal, use case) before asking for personal details.
- Micro-commitments in onboarding (pick topics, set a goal) that also personalize the product.
- Let users save or favorite before requiring an account.

**Audit question.** Does the flow start with the easiest, most engaging step?

## 21. Risk reversal (trials, guarantees, returns)
**Evidence** B (Baymard. 13% of abandoners cite an unsatisfactory returns policy. Return policy leniency research, Janakiraman et al. 2016 meta-analysis, found lenient policies raise purchases more than returns).

**Apply.**
- Free trials, money-back guarantees and free returns where the economics allow.
- State the policy near the CTA in plain language ("Cancel anytime in two clicks", "Free returns for 30 days").
- No-card trials lower the barrier. Card-required trials raise intent but lower starts. Choose deliberately and test.
- Remind before a trial converts to paid.

**Audit question.** What does the user risk by saying yes, and have we reduced and stated it?

## 22. Endowment effect and ownership
**Evidence** A for the effect (Kahneman, Knetsch and Thaler 1990), with debate about mechanisms.

**What it says.** People value what they own or feel they own more highly.

**Apply.**
- Let users build, customize or personalize early (name the workspace, upload a photo, configure a product). It creates ownership and investment.
- Full-feature trials let users experience owning the premium version.

**Audit question.** Do users create or personalize something of their own early in the flow?

## 23. Status quo bias and switching costs
**Evidence** A (Samuelson and Zeckhauser 1988).

**What it says.** People stick with what they have. Switching needs a strong reason and a low cost.

**Apply.**
- For acquisition from competitors, reduce switching costs with importers, migration help and concierge onboarding.
- Make the first step of switching tiny.

**Audit question.** What does it cost a user to switch to us, and how have we reduced it?

## 24. Comparison and decision aids
**Evidence** B (Baymard on comparison tools and product lists. Choice overload moderators in 01).

**Apply.**
- Plan comparison tables with aligned rows, the differences highlighted, and the recommended plan marked.
- Product comparison for complex purchases.
- Guided selectors and quizzes for novices.
- Filters that match how users think about the product (use case, not just specs).

**Audit question.** Can users compare their top options side by side without opening multiple tabs?

## 25. Personalization and recommendations
**Evidence** C (results vary widely. Perceived creepiness reduces trust when data use is unexpected).

**Apply.**
- Personalize from data users knowingly gave (stated goals, history) and explain why ("Because you bought X").
- Let users correct or reset recommendations.

**Audit question.** Would users understand and welcome why they are seeing this personalized content?

## 26. Consent and opt-in
**Evidence** Law. Under EU and UK GDPR, consent must be freely given, specific, informed and unambiguous. The CJEU's Planet49 ruling (2019) held pre-ticked boxes are not valid consent for cookies.

**Apply.**
- Unticked marketing checkboxes, with a clear benefit statement.
- Cookie banners with "Reject all" as easy as "Accept all".
- Ask for permissions in context, after explaining the benefit (see 06).

**Audit question.** Is every consent an active, informed choice with an equally easy no?
