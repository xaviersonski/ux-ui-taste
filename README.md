# UX/UI Taste ✦ Research-Backed Design & Audit Skill

> A research-backed library of psychological principles, behavioral economics, and actionable heuristics for designing and auditing user flows, screens, and front ends that convert, satisfy, and feel good to use.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Evidence Graded](https://img.shields.io/badge/Evidence-Graded%20(A--D)-success.svg)](#evidence-grades)
[![Dark Patterns](https://img.shields.io/badge/Dark%20Patterns-Zero%20Tolerance-red.svg)](#ethical-persuasion--legal-guardrails)
[![Standard](https://img.shields.io/badge/AI%20Skill-SKILL.md-purple.svg)](SKILL.md)

---

## Overview

Most UX advice swings between two extremes: dogmatic rules of thumb ("always keep menus to 7 items", "three clicks max") or aggressive growth hacking that relies on manipulative dark patterns.

**UX/UI Taste** takes a third way:
1. **Rooted in empirical science**: Every principle carries an explicit evidence grade (from meta-analyses and replicated field data to debunked myths).
2. **Prioritizes friction removal over trickery**: The biggest conversion lifts come from deleting fields, clarifying copy, and accelerating speed—not deceptive urgency.
3. **Dual-purpose**: Operates both as a human design playbook and as an AI agent skill (compatible with [Antigravity](https://github.com), Claude Code, Claude Desktop, Cursor, and custom agentic frameworks).

---

## The Taste, in Ten Rules

These core heuristics shape every recommendation:

1. **Clarity converts.** A user who instantly understands what this is, why it matters, and what to do next is the single biggest driver of conversion. Cleverness that costs comprehension loses.
2. **Remove before you add.** The biggest wins come from deleting fields, steps, choices, surprise costs, and interruptions. Baymard finds the average checkout shows ~23 form elements when 12–14 suffice.
3. **Earn the ask.** Show real value before asking for an email, payment details, permissions, or commitment. Ask at the exact moment the request makes sense to the user.
4. **Familiar for tasks, novel for moments.** Core tasks (navigation, forms, checkout, search) must follow conventions users already know. Save originality for brand moments, delights, and celebrations.
5. **Design the peak and the end.** People judge an experience largely by its most intense moment and its ending. Fix the worst moment first, then make the ending memorable.
6. **Speed is a feature.** Real speed first (Core Web Vitals), perceived speed second. Every wait over 1 second demands visual feedback.
7. **Honest persuasion only.** Help people make decisions they will be glad about. If a tactic only works when users don't notice it, drop it. Dark patterns are a serious legal and brand liability.
8. **Grade the evidence.** Treat single lab studies as hypotheses to test. Effects shrink at scale (academic nudges average ~8.7% gains; government nudge units at scale average ~1.4%).
9. **Accessible is usable.** Contrast, touch target size, keyboard navigation, clear labels, and reduced motion help everyone and are legally required in major markets.
10. **Context decides.** Every principle has boundary conditions. State them, and recommend an empirical test when uncertainty or stakes are high.

---

## Evidence Grades

Whenever citing a principle or recommending a change, cite its evidence grade:

| Grade | Description | Standard |
|---|---|---|
| **Grade A** | **Robust** | Meta-analyses or multiple independent replications, including scaled field experiments. |
| **Grade B** | **Solid but conditional** | Replicated or supported by large-scale industry benchmarks (Baymard, NN/g), with known boundary conditions or modest effect sizes. |
| **Grade C** | **Promising but thin** | Single lab study, small sample, commissioned/correlational data, or widely used practitioner heuristic. Treat as a hypothesis to test. |
| **Grade D** | **Myth or debunked** | Failed replication, misinterpreted statistic, or urban legend. Never present as fact; gently correct when cited. |

*See [`references/08-evidence-myths-measurement.md`](references/08-evidence-myths-measurement.md) for full replication status and effect-size calibration.*

---

## The Twenty Taste Maxims & UX Laws

Every interaction recommendation in this library is anchored by twenty rapid-reference maxims grounded in empirical cognitive psychology and human-computer interaction:

| Maxim | Principle / Scientific Law | Grade | Focus & Application |
|---|---|:---:|---|
| **Reduce choices per screen.** | **Hick's Law** | **A/B** | Minimize fork options; highlight a recommended path to prevent choice overload. ([01](references/01-cognitive-load.md)) |
| **Make targets large.** | **Fitts's Law** | **A** | Expand hit boundaries ($\ge 44\times44\text{ px}$ on touch, full card links). ([02](references/02-perception-attention-visual.md)) |
| **Follow familiar patterns.** | **Jakob's Law** | **B** | Match standard conventions from the rest of the web to leverage existing mental models. ([01](references/01-cognitive-load.md)) |
| **Group-related information.** | **Law of Proximity** | **A** | Internal spacing must be noticeably smaller than external group separation. ([02](references/02-perception-attention-visual.md)) |
| **Break content into chunks.** | **Miller's Law & Chunking** | **A** | Chunk working memory into $4\pm1$ clusters (numbers, steps, forms; not 7-item menus). ([01](references/01-cognitive-load.md)) |
| **Interactions within 400 milliseconds.** | **Doherty Threshold** | **B/C** | Respond under $100\text{ ms}$; resolve state within $400\text{ ms}$ to sustain continuous flow. ([05](references/05-emotion-memory-delight.md)) |
| **Highlight the primary action.** | **Von Restorff Effect** | **A/B** | Establish one visually dominant focal point (CTA) using isolation and contrast. ([02](references/02-perception-attention-visual.md)) |
| **Place key actions nearby.** | **Minimize Target Distance** | **A** | Fitts's corollary: keep controls near cursor/thumb reach; distance destructive actions. ([02](references/02-perception-attention-visual.md)) |
| **Put essentials first.** | **Serial Position Effect & Pareto** | **A/B** | Front-load the vital 20% benefits and primary navigation; leverage primacy and recency. ([01](references/01-cognitive-load.md), [02](references/02-perception-attention-visual.md)) |
| **End flows memorably.** | **Peak-End Rule** | **A** | Fix the worst frustration first; turn confirmation screens into rewarding endings. ([05](references/05-emotion-memory-delight.md)) |
| **Show visible progress.** | **Goal-Gradient & Endowed Progress** | **B** | Effort accelerates near milestones; show progress and reward real early steps. ([04](references/04-motivation-habit-progress.md)) |
| **Simplify complex interfaces.** | **Law of Prägnanz & Occam's Razor** | **A/B** | Resolve layouts into clean geometric harmony; cut gratuitous UI elements. ([01](references/01-cognitive-load.md), [02](references/02-perception-attention-visual.md)) |
| **Use sensible defaults.** | **Default Effect (Status Quo Bias)** | **A** | Answer questions for the majority by default, with effortless opt-outs. ([01](references/01-cognitive-load.md), [03](references/03-decision-persuasion-pricing.md)) |
| **Prevent errors proactively.** | **Error Prevention (Poka-Yoke)** | **B** | Constrain inputs, auto-format fields, and confirm only irreversible operations. ([06](references/06-feedback-control-forms.md)) |
| **Make errors recoverable.** | **Postel's Law & Forgiveness** | **B** | Be liberal in input tolerance; provide instant undo over disruptive modal alerts. ([06](references/06-feedback-control-forms.md)) |
| **Maintain pattern consistency.** | **Consistency & Standards** | **B** | Identical visual appearance must always signify identical function across all screens. ([01](references/01-cognitive-load.md), [06](references/06-feedback-control-forms.md)) |
| **Connect related elements visually.** | **Uniform Connectedness & Similarity** | **A** | Containers, borders, and shared styling visually overrule mere proximity. ([02](references/02-perception-attention-visual.md)) |
| **Reduce task completion time.** | **Parkinson's Law** | **B** | Work expands to fill available time; compact, brisk flows reduce drop-off and fatigue. ([04](references/04-motivation-habit-progress.md)) |
| **Reveal complexity gradually.** | **Progressive Disclosure & Tesler** | **B** | Shift complexity to the system; surface advanced options only upon demand. ([01](references/01-cognitive-load.md)) |
| **Make completion feel closer.** | **Endowed Progress & Ovsiankina** | **B** | Frame tasks as underway; make resuming interrupted workflows effortless. ([04](references/04-motivation-habit-progress.md)) |

---

## Reference Library

The library is organized into nine focused modules in [`references/`](references/):

| Module | Core Topics Covered | When to Read |
|---|---|---|
| [**01. Cognitive Load**](references/01-cognitive-load.md) | Working memory, Hick's law, choice overload, progressive disclosure, recognition over recall, mental models, Jakob's law, Occam's razor, Pareto principle, plain language. | Screens with choices, navigation, dense information, feature prioritization, or unfamiliar concepts. |
| [**02. Perception & Visual**](references/02-perception-attention-visual.md) | Visual hierarchy, Gestalt laws (proximity, similarity, uniform connectedness, Prägnanz), scanning patterns, the fold, Fitts's law & target distance, touch targets, first impressions, typography, contrast, motion. | Layout, visual hierarchy, responsive & mobile UI, landing pages. |
| [**03. Decision, Persuasion & Pricing**](references/03-decision-persuasion-pricing.md) | Defaults, anchoring, decoys, framing, loss aversion, zero price effect, cost transparency, social proof, reviews, trust cues, risk reversal. | Pricing pages, paywalls, product detail pages, signup flows, CTAs. |
| [**04. Motivation & Progress**](references/04-motivation-habit-progress.md) | Fogg Behavior Model, time-to-value, goal gradient, endowed progress, progress indicators, Parkinson's law, IKEA effect, flow, habits, reactance. | Onboarding, activation, retention, multi-step flows, task completion, gamification. |
| [**05. Emotion, Memory & Delight**](references/05-emotion-memory-delight.md) | Peak-end rule, Kano model, microinteractions, labor illusion, psychology of waiting, Doherty threshold & response times, error tone, voice, celebrations. | Loading states, latency budgets, confirmations, micro-delighters, service recovery. |
| [**06. Feedback, Control & Forms**](references/06-feedback-control-forms.md) | Nielsen heuristics, visibility of status, undo vs. confirm, error prevention, Postel's law, inline validation, form & checkout essentials, modals. | Forms, checkouts, settings, account creation, mobile interactions. |
| [**07. Ethics, Dark Patterns & Law**](references/07-ethics-dark-patterns-law.md) | Dark pattern taxonomy with fair alternatives, evidence on harm, US FTC regulations, EU Digital Services Act (DSA), UK DMCC Act. | Any persuasion, subscriptions, consent, cancellation, or pricing flows. |
| [**08. Evidence, Myths & Measurement**](references/08-evidence-myths-measurement.md) | Evidence grading criteria, effect-size reality check, comprehensive replication table, debunked UX myths, metrics, A/B testing hygiene, qualitative methods. | When citing numbers, evaluating "laws", or planning experiments. |
| [**09. Audit Checklist & Template**](references/09-audit-checklist.md) | Comprehensive checklist across all categories, 0–4 severity scale, structured markdown audit report template. | Auditing any existing page, app, screenshot, or user flow. |

---

## Flow Quick Index

Most UX requests center around a specific user flow. Use this index to jump directly to the right reference files:

```
┌──────────────────────────────────────┬────────────────────────────────────────────┐
│ Flow                                 │ Key Reference Guides                       │
├──────────────────────────────────────┼────────────────────────────────────────────┤
│ Landing or Home Page                 │ 02 (Hierarchy, Fold) ✦ 01 (Clarity, Scent) │
│                                      │ 03 (Social Proof, Trust)                   │
├──────────────────────────────────────┼────────────────────────────────────────────┤
│ Signup & Onboarding                  │ 04 (Time to Value, Endowed Progress)       │
│                                      │ 01 (Progressive Disclosure) ✦ 06 (Forms)   │
│                                      │ 05 (First "Aha" Moment)                    │
├──────────────────────────────────────┼────────────────────────────────────────────┤
│ Pricing Page & Paywall               │ 03 (Anchoring, Decoys, Framing, Risk)      │
│                                      │ 07 (Honest Pricing, Subscription Law)      │
├──────────────────────────────────────┼────────────────────────────────────────────┤
│ Product / Detail Page (PDP)          │ 03 (Reviews, Social Proof, Trust)          │
│                                      │ 02 (Hierarchy, Imagery) ✦ 01 (Choice)      │
├──────────────────────────────────────┼────────────────────────────────────────────┤
│ Cart & Checkout                      │ 06 (Forms, Guest Checkout, Validation)     │
│                                      │ 03 (Total Cost Transparency, Trust)        │
│                                      │ 05 (Confirmations) ✦ 07 (Drip Pricing)     │
├──────────────────────────────────────┼────────────────────────────────────────────┤
│ Search & Browse                      │ 01 (Information Scent, Scannability)       │
│                                      │ 06 (Search UX, Filters, Zero Results)      │
├──────────────────────────────────────┼────────────────────────────────────────────┤
│ Dashboards & Data-Heavy UI           │ 01 (Cognitive Load, Defaults)              │
│                                      │ 02 (Visual Hierarchy, Density)             │
├──────────────────────────────────────┼────────────────────────────────────────────┤
│ Empty, Loading & Error States        │ 05 (Psychology of Waiting, Voice & Tone)   │
│                                      │ 06 (System Feedback, Error Prevention)     │
├──────────────────────────────────────┼────────────────────────────────────────────┤
│ Notifications & Re-engagement        │ 04 (Prompts, Habits, Reactance)            │
│                                      │ 07 (Nagging & Dark Patterns)               │
├──────────────────────────────────────┼────────────────────────────────────────────┤
│ Cancellation & Downgrade             │ 07 (Symmetry Test, Legal Requirements)     │
│                                      │ 05 (Respectful Endings)                    │
└──────────────────────────────────────┴────────────────────────────────────────────┘
```

---

## Operating Modes

### Mode 1: Designing a Flow or Screen
1. **Frame the job**: Identify the user persona, their job-to-be-done, context (device, urgency, emotion), business objective, and primary success metric.
2. **Map the steps**: For each step, define the user's primary question ("What is this?"), their anxiety ("Is this safe?"), and the single primary action. Cut unnecessary steps.
3. **Apply the principles**: Walk through cognitive load, perception, decision-making, motivation, emotion, and feedback. Favor Grade A and B principles.
4. **Specify every state**: Default, empty, loading, partial, error, success, and edge cases (long text, zero results, slow network, accessibility).
5. **Design the peak and the end**: Pinpoint the moment of value ("aha") early, and design a reassuring confirmation ending.
6. **Run the ethics check**: Apply the Transparency, Regret, and Symmetry tests from [`07`](references/07-ethics-dark-patterns-law.md).
7. **Formulate test hypotheses**: Define primary metrics and guardrail metrics (cancellations, refund requests, support tickets).

### Mode 2: Auditing an Existing Flow
1. **Understand goals**: Clarify user intent and business conversion goals.
2. **First impressions check**: Evaluate the first 50 milliseconds (gut impression) and the first 5 seconds (clarity & purpose).
3. **Execute the checklist**: Walk through [`references/09-audit-checklist.md`](references/09-audit-checklist.md).
4. **Score findings by severity**:
   - `4 Critical`: Blocks task, risks data/money loss, or creates legal exposure.
   - `3 Major`: Causes abandonment or severe friction.
   - `2 Minor`: Slows users down or causes confusion.
   - `1 Cosmetic`: Visual or copy polish.
5. **Credit strengths**: Identify working patterns so redesigns do not regress them.
6. **Flag dark patterns & legal risks**: Highlight regulatory exposure (FTC, DSA, DMCC).
7. **Deliver structured report**: Use the output template in [`09`](references/09-audit-checklist.md).

---

## The 20 Highest-Leverage UX Moves

When time is limited, verify these twenty moves first—they offer the highest demonstrated return on investment:

1. **One primary action per screen**, visually dominant and unambiguous.
2. **A 5-second headline** stating clearly what the product is and who it is for.
3. **Upfront total pricing** (fees, taxes, shipping) shown before checkout starts.
4. **Guest checkout enabled**, offering account creation *after* payment completion.
5. **Radically fewer form fields**, with autofill attributes and smart defaults.
6. **Inline validation on blur** with kind, specific, blame-free error guidance.
7. **Fast real performance** (LCP < 2.5s, INP < 200ms) plus honest feedback for waits > 1s.
8. **Specific, verifiable social proof** placed adjacent to high-anxiety decisions.
9. **Visual trust cues** displayed right at the point of risk (payment, personal data).
10. **Immediate time-to-value**, deferring non-essential configuration.
11. **Clear progress indicators** in multi-step flows with an endowed head start when honest.
12. **Reward-driven confirmation screens** that bridge seamlessly to the next logical step.
13. **Instant Undo** instead of disruptive "Are you sure?" confirmation dialogs for reversible actions.
14. **User-serving defaults** that make opting out frictionless.
15. **Conventional design patterns** for core navigation, search, and transactional workflows.
16. **WCAG contrast compliance** ($\ge 4.5:1$ body) and touch targets $\ge 44\times44\text{ px}$.
17. **Plain language** written at approximately an 8th-grade reading level.
18. **Support for `prefers-reduced-motion`** and full keyboard accessibility.
19. **Symmetrical cancellation** (canceling must be as easy and quick as subscribing).
20. **Guardrail metrics** (refunds, complaints, churn) tracked alongside conversion.

---

## Common UX Myths Debunked

Don't cite these popular design myths as facts:

- ❌ *"Miller's Law (7±2) means menus can only have 7 items."*  
  Working memory limits apply to unassisted recall, not visible navigation that users scan visually.
- ❌ *"The 3-Click Rule."*  
  Click count does not correlate with task success or user satisfaction. Users gladly make more clicks if each click gives high information scent.
- ❌ *"Users don't scroll."*  
  Users scroll readily, provided there is no "false bottom" and the page offers progressive interest.
- ❌ *"Humans have an 8-second attention span (shorter than a goldfish)."*  
  An urban legend with zero basis in cognitive science or peer-reviewed literature.
- ❌ *"The Zeigarnik Effect means incomplete tasks are remembered better."*  
  Failed modern replications. What holds true is the *Ovsiankina effect* (the motivational urge to resume interrupted tasks).
- ❌ *"Red buttons convert better."*  
  No single color has an inherent universal conversion advantage. What matters is visual contrast against surrounding elements.
- ❌ *"93% of communication is nonverbal."*  
  Mehrabian's classic finding applied only to ambiguous single-word expressions of emotion, not general communication.
- ❌ *"Aesthetics equal usability."*  
  The aesthetic-usability effect holds for first impressions, but severe functional usability failures rapidly destroy perceived beauty once interacted with.

---

## Ethical Persuasion & Legal Guardrails

Psychology should help users make decisions they remain glad about. If a tactic relies on deception, confusion, or exhaustion, it is unacceptable.

### The 3 Ethical Tests
- **The Transparency Test**: Would this design pattern still achieve its goal if the user were explicitly told why it was designed that way?
- **The Regret Test**: Does the user feel satisfied with their decision 24 hours, 7 days, and 30 days later?
- **The Symmetry Test**: Is refusing or canceling as simple, fast, and visible as agreeing or subscribing?

### Regulatory Compliance Highlights
- **US FTC ("Click-to-Cancel" Rule & Section 5)**: Requires cancellation mechanisms to be as easy to find and execute as signup, forbids hidden recurring charges and deceptive fee partitioning.
- **EU Digital Services Act (DSA Article 25)**: Explicitly bans deceptive UI choices, unequal button styling ("accept" vs "reject"), and nagging.
- **UK Digital Markets, Competition and Consumers Act (DMCC)**: Prohibits drip pricing, fake scarcity countdowns, and fabricated consumer reviews.

*Detailed taxonomy and compliant alternatives in [`references/07-ethics-dark-patterns-law.md`](references/07-ethics-dark-patterns-law.md).*

---

## How to Use

### 1. In AI Coding Assistants & Agents
This repository is packaged as an agent skill via [`SKILL.md`](SKILL.md).

- **Google Antigravity**: Place or symlink the folder into your project's workspace or agent skill directory (`builtin/skills/ux-ui-taste` or `.gemini/skills/ux-ui-taste`).
- **Claude Code / Desktop**: Add this repository to your skills directory or Claude project knowledge files.
- **Cursor / Windsurf**: Add a `.cursorrules` or system prompt pointer referencing `SKILL.md` and `references/`.
- **Custom Agent Prompt**:
  ```text
  You have access to the UX/UI Taste library in `references/`.
  When asked to design, review, or code interfaces, adhere to the 10 Taste Rules,
  read the relevant reference files, cite principles with evidence grades (A–D),
  and ensure zero dark patterns.
  ```

### 2. For Design, Engineering & Product Teams
- **Design Critiques**: Use the 0–4 severity scale and checklist in `references/09-audit-checklist.md` during design reviews.
- **Pull Request Reviews**: Check front-end code against accessibility, form validation, error states, and responsive touch targets in `references/06-feedback-control-forms.md`.
- **PRD & Product Specs**: Reference the *Flow Quick Index* when writing functional requirements to guarantee all states (empty, loading, edge, error) are accounted for upfront.

---

## Repository Structure

```
ux-ui-taste/
├── .gitattributes                          # Git normalization rules (LF, text handling)
├── .gitignore                              # Clean ignore rules (OS, AppleDouble, IDE)
├── LICENSE                                 # MIT Open Source License
├── README.md                               # Repository guide and overview (this file)
├── SKILL.md                                # AI skill definition and agent instructions
└── references/                             # In-depth evidence-backed modules
    ├── 01-cognitive-load.md                # Working memory, Hick's law, progressive disclosure
    ├── 02-perception-attention-visual.md   # Hierarchy, Gestalt, scanning patterns, Fitts's law
    ├── 03-decision-persuasion-pricing.md   # Defaults, anchoring, social proof, pricing psychology
    ├── 04-motivation-habit-progress.md     # Fogg model, goal gradient, IKEA effect, habits
    ├── 05-emotion-memory-delight.md        # Peak-end rule, Kano model, perceived speed, waiting
    ├── 06-feedback-control-forms.md        # Heuristics, form design, validation, checkout UX
    ├── 07-ethics-dark-patterns-law.md      # Dark patterns catalog, alternatives, FTC/DSA law
    ├── 08-evidence-myths-measurement.md    # Evidence grades, debunked myths, A/B testing
    └── 09-audit-checklist.md               # 0–4 severity checklist and markdown audit template
```

---

## Contributing

Contributions backed by sound empirical evidence are warmly welcomed:
- **Adding Studies**: Include replication status, sample sizes, and whether the study was conducted in a laboratory or scaled in the field.
- **Updating Legal References**: As consumer protection laws evolve across jurisdictions, updates to `07-ethics-dark-patterns-law.md` are appreciated.
- **Refining Principles**: Propose refinements via pull requests following the standard schema: *What it says*, *Evidence grade*, *How to apply*, *Limits & boundary conditions*, and *Audit question*.

---

## License

This project is open-source under the [MIT License](LICENSE).
