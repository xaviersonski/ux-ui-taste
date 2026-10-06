# 10. Problem Diagnosis, Lateral Thinking and High-Taste Fixes

How to think about diagnosing and solving UX problems without falling into predictable, one-size-fits-all AI recommendations.

---

## Why AI Fails at UX Recommendations: The Vanilla Trap

When asked to "improve conversion", "fix onboarding", or "critique this screen", most AI assistants reflexively reach for the same five superficial band-aids:
1. **The Tooltip Band-aid:** Adding an info icon `(i)` or tooltip instead of rewriting confusing copy or simplifying the layout. If an interface requires a tooltip to be understood, the design has already failed.
2. **The Modal / Banner Hammer:** Slapping a modal dialog, banner, or pop-up over an ignored feature to force attention, creating interruption and banner blindness.
3. **The "Bigger Button" Fallacy:** Making the CTA larger, changing its color to green, or adding pulsing animations when the real bottleneck is that the user isn't convinced or fears the hidden cost.
4. **The Generic Onboarding Checklist:** Forcing new users through a 5-step setup tour instead of delivering immediate, tangible value in the product.
5. **The Fake Urgency Reflex:** Adding countdown timers or artificial scarcity instead of addressing the core value proposition.

These vanilla fixes share one flaw: **they treat symptoms on the glass rather than the human friction behind them.** They ask the user to work harder rather than making the system smarter.

Because every product, audience, and flow has a unique context, an AI must not prescribe generic formulas. It must follow a structured **thinking protocol** to diagnose the root cause and generate genuinely creative, high-taste solutions.

---

## Phase 1: Diagnose the 5 Friction Dimensions

Before proposing any change, identify which fundamental human friction is causing the failure:

```
┌───────────────────────────────────────────────────────────────────────────────┐
│                          THE 5 UX FRICTION TYPES                              │
├───────────────────┬───────────────────────────────────────────────────────────┤
│ 1. Comprehension  │ "I don't understand what this is, what this word means,    │
│    Friction       │ or what clicking this button will actually do."           │
│                   │ (Mental model clash, insider jargon, weak information scent)│
├───────────────────┼───────────────────────────────────────────────────────────┤
│ 2. Anxiety & Risk │ "I know what it does, but I fear the consequence:         │
│    Friction       │ being billed, spam, embarrassment, or losing my work."    │
│                   │ (Loss aversion, missing risk reversal, opacity)           │
├───────────────────┼───────────────────────────────────────────────────────────┤
│ 3. Cognitive &    │ "This demands too much working memory, reading, typing,   │
│    Motor Friction │ hunting, or precise finger gymnastics."                   │
│                   │ (Overload, Fitts's distance, poor grouping, no defaults)  │
├───────────────────┼───────────────────────────────────────────────────────────┤
│ 4. Timing & Value │ "You are asking for my commitment, email, or money before │
│    Asymmetry      │ showing me any real value."                               │
│                   │ (Premature ask, violating 'Earn the ask')                 │
├───────────────────┼───────────────────────────────────────────────────────────┤
│ 5. Autonomy &     │ "I feel forced, manipulated, nagged, or trapped."         │
│    Reactance      │ (Dark patterns, confirmshaming, hard paywalls, no undo)   │
└───────────────────┴───────────────────────────────────────────────────────────┘
```

**Diagnostic Rule:** A solution aimed at the wrong friction dimension always fails. For example, if a user isn't clicking because of *Anxiety Friction* (fear of being billed), making the button bigger (*Motor*) or adding a tooltip (*Comprehension*) will not move the metric. You must eliminate the anxiety (add *"No credit card required. Cancel in 1 click."*).

---

## Phase 2: The Abstraction Climb ("What is this a way of doing?")

Before redesigning a problematic component, climb one rung up the ladder of abstraction (de Bono 1992):

1. **State the current element:** *"We have a 7-field company profile form in onboarding."*
2. **Ask the climb question:** *"What is this a way of doing?"*
   - *Answer:* *"It is a way of getting data to personalize the dashboard."*
3. **Ask again:** *"What is that a way of doing?"*
   - *Answer:* *"It is a way of helping the user see relevant value on their first visit."*

Once you reach the underlying purpose, the current element ceases to look inevitable. You are no longer trapped into "how do we make this 7-field form prettier?" You can now ask: **"What is the fastest, lowest-friction way to show relevant value on first visit?"**

---

## Phase 3: The Eight Lateral Thinking Moves for UX

When generating solutions, run the problem through these eight structural moves:

### 1. Subtractive Solving (The Elimination Move)
- **The Core Question:** What if we didn't improve this step, but deleted it completely?
- **How it works:** Instead of polishing friction, eradicate it. If a form has 6 fields, ask which 3 can be inferred from the IP/browser and which 2 can be dropped entirely. If users struggle with a complex settings toggle, pick the ideal default so the setting disappears.
- **Example:** Instead of redesigning an address verification error dialog, auto-complete address data from postal code lookup.

### 2. Timing & Sequence Shift (Earn the Ask)
- **The Core Question:** What if this ask happened at a completely different moment in the journey?
- **How it works:** Move the request from a point of high friction (before value) to a point of natural motivation (after value).
- **Example:** Instead of requiring account creation before using an AI generator or design canvas, let the user create the asset first. Prompt for an email only when they click *"Save"* or *"Export"*—the moment they have emotional ownership.

### 3. Effort Inversion (Tesler's Shift)
- **The Core Question:** What if the software did the work instead of asking the user to do it?
- **How it works:** Shift the complexity from the user's brain and fingers onto system logic (Tesler's Law).
- **Example:** Instead of asking a user to select their credit card brand, detect Visa/Mastercard from the first digits. Instead of asking a business for their industry and employee count, ask for their website domain and enrich the company profile automatically.

### 4. Contextual Relocation (Proximity / Scent)
- **The Core Question:** Why is this control physically or conceptually separated from the object it changes?
- **How it works:** Move actions from distant toolbars, header menus, or multi-step modal dialogs directly into the user's line of sight or hover context (Fitts's Law & Law of Proximity).
- **Example:** Instead of selecting a row in a table and moving the mouse 800px up to a top action bar, reveal inline actions directly on hover over the row.

### 5. Radical Risk Reversal (The Anxiety Dissolver)
- **The Core Question:** What unspoken fear or skepticism is stopping the user, and how can we neutralize it right next to the trigger?
- **How it works:** Address the exact objection at the micro-moment of decision.
- **Example:** Placing micro-copy directly below a payment CTA: *"7-day free trial. An email reminder is sent 2 days before billing starts. Cancel in 2 clicks from settings."*

### 6. State Reframing (Springboard States)
- **The Core Question:** How can a passive or negative state (empty, loading, error, 404) become an active accelerator?
- **How it works:** Transform dead ends into high-momentum starting points.
- **Example:** Turn an empty dashboard into a starter gallery with 3 one-click templates rather than a blank page with a sad illustration. Turn a long search wait into operational transparency showing live sources checked.

### 7. Progressive Engagement (The Staging Move)
- **The Core Question:** Can we replace an intimidating wall of effort with a 1-second starter commitment?
- **How it works:** Break a daunting task into a trivial micro-step that triggers the endowed progress effect and goal-gradient momentum.
- **Example:** Rather than showing a 20-question financial survey, ask one simple, intriguing question on screen 1: *"What's your primary financial goal this year?"* Once answered, show *"1 of 3 quick stages completed"* and continue smoothly.

### 8. Assumption Inversion (The Opposites Game)
- **The Core Question:** What does the industry assume is mandatory, and what happens if we build the exact opposite?
- **How it works:** List the unstated conventions of competitors and flip one into a defensible opposite.
- **Example:** Competitors in B2B SaaS lock product demos behind a *"Book a 30-minute sales call"* form. Flip it: embed an interactive, fully clickable product sandbox directly on the homepage with zero login required.

---

## Phase 4: Divergence and the Three-Angle Mandate

When generating recommendations, **never provide three variations of the same idea** (e.g. three slightly different button labels or three color tweaks).

Always provide solutions across **three distinct structural angles**:

```markdown
### Proposed Directions

#### Angle A: The Subtractive / System Move (Elimination & Defaults)
[How to eliminate the need for the user to make this effort at all.]
- Mechanism: [e.g. Auto-enrichment, pre-selection, smart defaults]
- Principle: Tesler's Law (B), Occam's Razor (B)

#### Angle B: The Cognitive & Risk Reversal Move (Clarity & Anxiety)
[How to reframe the choice, dissolve fear, and clarify consequences.]
- Mechanism: [e.g. Inline guarantee, plain language comparison, progressive disclosure]
- Principle: Risk Reversal (B), Plain Language (B)

#### Angle C: The Structural / Timing Shift (Sequence & Interaction)
[How to change the journey or interaction paradigm entirely.]
- Mechanism: [e.g. Reverse onboarding, sandbox first, contextual inline trigger]
- Principle: Earn the Ask (Taste Rule 3), Endowed Progress (B)
```

---

## Phase 5: The Disqualification Rule (Honesty Mechanics)

Every high-taste recommendation must include a **Disqualification Check**:
- Explicitly name the obvious "vanilla" fixes that anyone could have proposed.
- State why they are disqualified for this specific situation.

**Example Disqualification Statement:**
> *"Disqualified obvious fix: We considered adding an inline tooltip explaining 'Workspace Namespace' and adding an onboarding modal. Disqualified because user testing shows users don't read tooltips, and the term itself is internal engineering jargon. Adding an explanation to a confusing concept treats the symptom; auto-generating a clean slug from the project name eliminates the problem entirely."*

---

## Phase 6: How to Think About Usability & Metric Scores

When optimizing for usability scores (SUS, SEQ) or conversion rates:
1. **Target Severity First:** Fixing one Severity 4 issue (e.g. hidden total cost at payment) produces a 10x larger gain than polishing ten Severity 1 cosmetic issues.
2. **Prioritize Reach Over Depth:** A 5% friction reduction on the homepage or signup screen impacts 100% of visitors; a 50% improvement on an obscure settings screen impacts <2% of users.
3. **Always Pair with Guardrail Metrics:**
   - If optimizing **Signup Conversion**, guardrail against **Day-7 Activation** and **Spam Rates**.
   - If optimizing **Checkout Speed**, guardrail against **Order Errors** and **Customer Support Tickets**.
   - If optimizing **Retention**, guardrail against **Unsubscribe Rates** and **User Reactance**.
