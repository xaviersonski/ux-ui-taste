---
name: ux-ui-taste
description: Research-backed UX and UI taste for designing and auditing user flows, screens and front ends that convert, satisfy and feel good to use. Use this skill whenever the user asks to design, plan, sketch, critique, review, audit or improve any user flow, onboarding, signup, checkout, pricing page, paywall, form, landing page, dashboard, search, empty, error or loading state, settings page, notification, or cancellation flow. Also use it for questions about conversion rate, activation, retention, friction, delight, microinteractions, trust, persuasion, behavioral psychology, UX laws or dark patterns, and when reviewing a screenshot, mockup, wireframe, Figma description or front end code for usability, even if the user never says "UX".
---

# UX/UI Taste

This skill gives Claude a library of psychological principles, studies and tactics for building products that people find easy, trustworthy and pleasant, and that convert because of it. It is organized by psychological principle. Every principle carries an evidence grade so Claude can tell a robust finding from a popular myth.

Use it in two modes. **Design mode** creates new flows and screens. **Audit mode** critiques existing ones. Both draw on the same principle library in `references/`.

## The taste, in ten rules

These are the defaults that shape every recommendation. The reference files explain the research behind each.

1. **Clarity converts.** A user who instantly understands what this is, why it matters and what to do next is the single biggest driver of conversion. Cleverness that costs comprehension loses.
2. **Remove before you add.** The biggest wins usually come from deleting things (fields, steps, choices, surprise costs, interruptions) before adding persuasion. Baymard finds the average checkout shows about 23 form elements when 12 to 14 would do.
3. **Earn the ask.** Show value before asking for an email, a card, a permission or a commitment. Ask at the moment the request makes sense to the user.
4. **Familiar for tasks, novel for moments.** Core tasks (navigation, forms, checkout) should look and behave like the conventions users already know. Save originality for brand moments and celebrations.
5. **Design the peak and the end.** People judge an experience largely by its most intense moment and its ending. Fix the worst moment first, then make the ending good.
6. **Speed is a feature.** Real speed first, perceived speed second. Every wait needs feedback.
7. **Honest persuasion only.** Use psychology to help people make decisions they will be glad about. If a tactic only works when users don't notice it, drop it. Dark patterns are now a serious legal liability in the US, UK and EU.
8. **Grade the evidence.** Treat a single lab study as a hypothesis to test. Effects shrink at scale. Say how strong the evidence is.
9. **Accessible is usable.** Contrast, target size, keyboard access, clear labels and reduced motion help everyone and are legally required in many markets.
10. **Context decides.** Every principle has boundary conditions. State them, and recommend a test when the stakes or uncertainty are high.

## Evidence grades

Use these grades whenever citing a principle, in both modes.

- **A, robust.** Meta-analyses or many independent replications, including field data.
- **B, solid but conditional.** Replicated or backed by large-scale industry research (Baymard, NN/g), with known boundary conditions or modest effect sizes.
- **C, promising but thin.** A single study, small samples, commissioned or correlational data, or a widely used practitioner heuristic. Treat as a hypothesis to test.
- **D, myth or failed replication.** Do not present as fact. If the user cites one, correct it kindly and offer what the evidence does support.

Detail on effect sizes, replication status and common myths is in `references/08-evidence-myths-measurement.md`. A key calibration point is that nudges published in academic journals averaged an 8.7 percentage point effect, while the same kinds of nudges run at scale by government nudge units averaged 1.4 points (DellaVigna and Linos 2022). Expect small, real gains from single tactics, and larger gains from removing genuine friction.

## Principle library

Read only the files relevant to the task. Each principle entry has the same shape, which is what it says, the evidence grade, how to apply it, its limits, and an audit question.

| File | Covers | Read when |
|---|---|---|
| `references/01-cognitive-load.md` | Working memory, Hick's law, choice overload, progressive disclosure, recognition over recall, mental models, Jakob's law, information scent, plain language | Any screen with choices, navigation, dense information or new concepts |
| `references/02-perception-attention-visual.md` | Visual hierarchy, Gestalt, scanning patterns, the fold, Fitts's law, target sizes, first impressions, aesthetics, typography, color, contrast, motion | Layout, visual design, mobile, landing pages, anything visual |
| `references/03-decision-persuasion-pricing.md` | Defaults, anchoring, decoys, framing, loss aversion, pricing psychology, social proof, reviews, trust, scarcity, urgency, reciprocity, risk reversal | Pricing pages, paywalls, product pages, signup, plan selection, CTAs |
| `references/04-motivation-habit-progress.md` | Fogg model, goal gradient, endowed progress, progress bars, IKEA effect, self-determination theory, flow, habits, rewards, implementation intentions, reactance | Onboarding, activation, retention, gamification, multi-step flows |
| `references/05-emotion-memory-delight.md` | Peak-end rule, Kano, delight, microinteractions, labor illusion, psychology of waiting, perceived performance, error tone, voice, celebrations, service recovery | Making things feel good, loading states, confirmations, brand moments |
| `references/06-feedback-control-forms.md` | Nielsen heuristics, feedback, undo, error prevention, inline validation, form and checkout design, search, empty states, modals, permissions, accessibility in interaction | Forms, checkout, settings, errors, mobile interaction, search |
| `references/07-ethics-dark-patterns-law.md` | Dark pattern taxonomy with fair alternatives, evidence on their effects, current US, UK and EU law | Any persuasion, subscription, cancellation, consent or pricing work. Always skim before recommending urgency, scarcity, defaults or retention tactics |
| `references/08-evidence-myths-measurement.md` | Replication status, myths, how to read industry stats, metrics, A/B testing hygiene | When citing numbers, when the user cites a "law", when proposing tests |
| `references/09-audit-checklist.md` | Full audit checklist by principle, severity scale, output template | Audit mode, always |

### Flow quick index

The library is organized by principle, but most requests arrive as a flow. Use this to find the right files fast.

- **Landing or home page.** 02 (first impressions, hierarchy, fold), 01 (clarity, scent), 03 (social proof, trust).
- **Signup and onboarding.** 04 (time to value, endowed progress, goal gradient), 01 (progressive disclosure), 06 (forms), 05 (first success moment).
- **Pricing page and paywall.** 03 (anchoring, decoys, center stage, framing, risk reversal), 07 (honest urgency, subscriptions law).
- **Product or detail page.** 03 (reviews, trust), 02 (hierarchy, imagery), 01 (choice overload).
- **Cart and checkout.** 06 (forms, guest checkout, validation), 03 (total cost transparency, trust at payment), 05 (confirmation as the ending), 07 (drip pricing).
- **Search and browse.** 01 (information scent), 06 (search UX, filters, no results).
- **Dashboards and data-heavy tools.** 01 (cognitive load, defaults), 02 (hierarchy, density).
- **Errors, empty and loading states.** 05 (waiting, tone, recovery), 06 (feedback, prevention).
- **Notifications and re-engagement.** 04 (prompts, habits, reactance), 07 (nagging).
- **Cancellation and downgrade.** 07 first, then 05 (endings).

## Mode 1. Designing a flow or screen

1. **Frame the job.** Identify who the user is, what job they are hiring the product for, their context (device, urgency, expertise, emotional state), the business goal, and one success metric. If key facts are missing, make a reasonable assumption and state it.
2. **Map the flow as steps.** For each step write the user's question ("what is this?", "is it safe?", "how much?"), their likely anxiety, the one primary action, and what they need to know to take it. Cut any step that answers no user question.
3. **Walk the principle families.** For each step, check cognitive load, perception, decision, motivation, emotion, feedback and ethics using the reference files. Apply the strongest relevant principles, favoring grade A and B.
4. **Specify every state.** Default, empty, loading, partial, error, success, and edge cases (long text, zero results, slow network, returning user, screen reader). Most products feel bad in the states nobody designed.
5. **Design the peak and the end.** Name the moment of value (the "aha") and make sure it arrives early and lands well. Make the last screen of the flow clear, reassuring and forward-looking.
6. **Run the ethics check.** Apply the three tests in `07`. Replace any manipulative tactic with its fair alternative.
7. **Decide what to test.** List the two or three riskiest assumptions and how to test them, with a primary metric and a guardrail metric.

**Design output format.** Unless the user asks for something else, deliver the flow outline (steps and their purpose), a per-screen spec (layout priority, copy direction, primary and secondary actions, states), the rationale for key decisions citing the principle and its grade in a short parenthetical, and a short test plan. When the user wants front end code, apply the same principles in the build and note the reasoning in brief comments or a short summary.

## Mode 2. Auditing an existing flow or screen

1. **Understand the goal and the user.** Ask, or infer and state, who it is for and what success looks like.
2. **Walk it as the user.** Go step by step, narrating what a first-time user sees, thinks and feels, including the first 50 milliseconds (gut impression) and the first 5 seconds (can they say what this is and what to do).
3. **Run the checklist.** Use `references/09-audit-checklist.md`. Log each issue with the violated principle, the evidence grade, a severity score (0 to 4), and a concrete fix.
4. **Prioritize.** Rank by severity, reach (how many users hit it) and effort. Lead with the few changes that matter most.
5. **Credit what works.** Name strengths so they survive the redesign.
6. **Flag ethics and legal risk separately.** Any dark pattern gets called out even if it converts.

**Audit output format.** Use the template at the end of `09-audit-checklist.md`. Keep it scannable, and lead with the top three fixes.

## Highest-leverage moves

When time is short, check these first. They combine strong evidence with large typical impact.

1. One clear primary action per screen, visually dominant.
2. A headline that says what it is and who it's for, readable in five seconds.
3. Show the full price, including fees and shipping, as early as possible. Unexpected extra costs are the top reason shoppers abandon carts in Baymard's surveys.
4. Guest checkout, and account creation offered after purchase.
5. Fewer form fields, with smart defaults, autofill and format-tolerant inputs.
6. Inline validation on blur with specific, kind error messages.
7. Fast real performance (Core Web Vitals), then honest progress feedback for any wait over about one second.
8. Social proof that is specific, real and placed near the decision.
9. Trust cues at the moment of risk (payment, personal data, permissions).
10. Get the user to first value fast, and defer setup that can wait.
11. Show progress in multi-step flows, and give a head start when progress is real.
12. Design the confirmation screen as a reward and a bridge to what's next.
13. Make undo available instead of asking "are you sure?" for reversible actions.
14. Sensible defaults that serve the user, with alternatives easy to pick.
15. Conventional navigation and layouts for core tasks.
16. Contrast of at least 4.5 to 1 for body text, and touch targets of at least 24 by 24 CSS pixels (44 or more for primary actions on touch).
17. Plain language at roughly a grade 8 reading level for consumer products.
18. Respect for `prefers-reduced-motion` and keyboard users.
19. Easy cancellation that mirrors how easy signup was.
20. A test plan with a guardrail metric (refunds, complaints, cancellations, support tickets) so short-term wins don't hide long-term harm.

## Myths to avoid stating as fact

Correct these gently when they come up. Details and sources are in `08`.

- "Seven plus or minus two means menus need seven items or fewer." Working memory research doesn't apply to visible menus users can scan.
- "The three-click rule." Click count doesn't predict success or satisfaction. Users happily click more when each click clearly moves them closer.
- "Users don't scroll." They do, though attention still drops sharply below the first screen.
- "Humans have an eight-second attention span, shorter than a goldfish." No credible source.
- "Unfinished tasks are remembered better" (the Zeigarnik memory effect). It fails to replicate. The urge to resume unfinished tasks (the Ovsiankina effect) does hold.
- "Red buttons convert better" and other fixed color meanings. What matters is contrast with the surroundings.
- "93% of communication is nonverbal." Mehrabian's study was about ambiguous single words expressing feelings.
- "Beautiful means usable." The aesthetic-usability effect is real for first impressions, but poor usability lowers how beautiful people rate a product after they use it.

## Writing style for outputs

Write recommendations plainly and specifically, e.g. "Move the plan comparison above the testimonials so the price question is answered before the trust question." Avoid vague advice like "improve the hierarchy." Cite principles by name with the grade in a short parenthetical, for example "(goal gradient, B)". Keep citations light in casual answers and fuller in formal audits.
