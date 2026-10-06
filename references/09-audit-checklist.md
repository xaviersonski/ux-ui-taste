# 09. Audit Checklist and Output Template

Use this in audit mode. Work through the sections that apply. Each line names the principle and the file with more detail. Log every "no" as a finding.

## Severity scale

- **4 Critical.** Blocks the task, causes data or money loss, or creates legal exposure. Fix before anything else.
- **3 Major.** Causes frequent failure, abandonment or serious frustration.
- **2 Minor.** Slows users down or causes occasional confusion.
- **1 Cosmetic.** Polish. Fix when convenient.

Prioritize by severity, then by reach (how many users hit it), then by effort.

## A. First impression and clarity (01, 02)
- [ ] In 5 seconds, can a new user say what this is, who it's for and what to do next? (clarity, five-second test)
- [ ] Does the first screen look calm, credible and typical of its category? (first impressions, prototypicality)
- [ ] Is there one visually dominant primary action? (hierarchy, Von Restorff)
- [ ] Does the headline use the user's language and lead with the benefit? (information scent, plain language)
- [ ] Is there a cue to scroll, with no false bottom? (the fold)

## B. Cognitive load (01)
- [ ] Is anything on screen irrelevant to the current step? (cognitive load)
- [ ] Does the user ever have to remember information from a previous screen? (working memory)
- [ ] At key decisions, are choices limited, organized and is one recommended? (Hick, choice overload)
- [ ] Are advanced options tucked away but easy to reach? (progressive disclosure)
- [ ] Could this interface achieve the exact same user outcome with fewer elements, concepts or steps? (Occam's razor)
- [ ] Are the vital 20% of core tasks dominant, rather than cluttering the screen with the 80% rare actions? (Pareto principle)
- [ ] Does the system do work the user is currently doing (detecting, calculating, formatting)? (Tesler)
- [ ] Do conventions match what users know from other products? (Jakob's law)
- [ ] Is terminology consistent across screens? (consistency)
- [ ] Is the copy plain enough for a tired person on a phone? (plain language)

## C. Visual and interaction design (02, 06)
- [ ] Does spacing (proximity) and containers/connectors (uniform connectedness) make it clear what belongs together? (Gestalt proximity, uniform connectedness)
- [ ] Do elements with identical functions share identical styling, and are non-clickable elements distinct? (Law of similarity)
- [ ] Does the visual layout resolve into clean, symmetrical, and regular geometric structures without visual clutter? (Law of Prägnanz)
- [ ] Can users get the gist from headings and first words? (scanning)
- [ ] Is it obvious what's clickable? (signifiers)
- [ ] Do icons have labels? (icon usability)
- [ ] Are targets at least 24 px, primary touch targets 44 to 48 px, and placed near the user's thumb or focus? (Fitts's law, target distance)
- [ ] Do text and controls meet contrast minimums, and does meaning survive without color? (contrast)
- [ ] Is body text at least 16 px with comfortable line length and height? (typography)
- [ ] Are animations fast, purposeful and disabled for reduced motion? (motion)
- [ ] Does feedback appear where the user is looking? (change blindness)

## D. Feedback, control and errors (05, 06)
- [ ] Does every action give feedback within about 100 ms? (system status)
- [ ] Do waits over 1 s show progress, and waits over 10 s show determinate progress or notify on completion? (response time limits)
- [ ] Can users go back, cancel and undo without losing work? (user control, forgiveness)
- [ ] Are confirmations reserved for irreversible actions, with the action named on the button? (undo over confirm)
- [ ] Are error messages specific, placed at the problem, blame-free, and is entered data kept? (error tone)
- [ ] Are likely mistakes prevented by constraints and defaults? (error prevention)
- [ ] Is work saved automatically and easy to resume? (Ovsiankina)

## E. Forms and checkout (06, 03)
- [ ] Has every field been justified, and could any be inferred, deferred or dropped? (form length)
- [ ] Single column, labels above, no placeholder-only labels? (form layout)
- [ ] Correct input types and autocomplete attributes? (mobile, autofill)
- [ ] Format-tolerant inputs? (Postel)
- [ ] Inline validation on blur? (inline validation)
- [ ] Guest checkout, with account creation offered after purchase? (forced registration)
- [ ] Total cost, delivery date and returns policy visible before checkout? (cost transparency)
- [ ] Express wallets available? (pain of paying)
- [ ] Payment step visually reinforced and consistent with the rest of the site? (trust at payment)
- [ ] Coupon field present but not prominent? (checkout)

## F. Decision, persuasion and trust (03)
- [ ] Do defaults serve the user, with alternatives easy to choose? (defaults)
- [ ] Is the recommended option placed and highlighted where uncertain users look? (center stage)
- [ ] Is the first number shown a fair reference? (anchoring)
- [ ] Is social proof specific, real, relevant and near the decision? (social proof)
- [ ] Are reviews numerous, recent, varied and filterable? (reviews)
- [ ] Is there enough evidence that this is a real, accountable company? (credibility)
- [ ] Is the user's risk reduced and stated near the CTA (trial, guarantee, returns, cancel anytime)? (risk reversal)
- [ ] Do CTAs state the outcome ("Start free trial")? (satisficing)

## G. Motivation and progress (04)
- [ ] How quickly does a new user reach first value, and could setup be deferred? (time to value)
- [ ] Do multi-step flows show named steps and progress, with fast early steps? (progress indicators)
- [ ] Is progress already made visible? (endowed progress)
- [ ] Can users see how close the next meaningful milestone is? (goal gradient)
- [ ] Does the flow compress unnecessary steps and prime brisk, focused completion without artificial panic? (Parkinson's law)
- [ ] Do users create or personalize something early? (IKEA, endowment)
- [ ] Are permissions requested in context with a clear benefit? (permission timing)
- [ ] Does any copy feel coercive? (reactance)
- [ ] Does the experience support autonomy, competence and relatedness? (SDT)

## H. Emotion and memory (05)
- [ ] What is the worst moment in this flow, and can it be fixed or softened? (peak-end)
- [ ] Is there a genuine positive peak? (peak-end, delight)
- [ ] Does the final screen confirm, inform and point to what's next? (endings)
- [ ] During waits, can users see real work happening? (labor illusion)
- [ ] Are all the basics flawless before any delighters? (Kano)
- [ ] Is the tone right for each emotional moment? (voice and tone)
- [ ] Are empty states helpful and action-oriented? (empty states)

## I. Accessibility (02, 06)
- [ ] Can the core flow be completed with a keyboard alone, with visible focus that isn't obscured?
- [ ] Do all inputs have programmatic labels, and are errors announced?
- [ ] Does the core flow work with a screen reader?
- [ ] Do drag interactions have a single-pointer alternative?
- [ ] Is redundant entry avoided, and is authentication free of memory tests?

## J. Performance and waiting (05)
- [ ] Does every action give visible feedback within 100 ms and complete transitions within the 400 ms Doherty threshold? (Doherty threshold, response times)
- [ ] LCP under 2.5 s, INP under 200 ms, CLS under 0.1 on mobile?
- [ ] No layout shift during load?
- [ ] Is the loading pattern suited to the wait length, without flicker?
- [ ] For waits over 1 second, is unoccupied time converted into occupied or transparent time (operational transparency, pipelined tasks, or engaging micro-interactions)? (Maister's laws, labor illusion, elevator mirror effect)

## K. Ethics and legal risk (07)
- [ ] Transparency test. Would each tactic still work if users understood it?
- [ ] Regret test. Are refunds, cancellations and complaints tracked as guardrails?
- [ ] Symmetry test. Is no as easy as yes, and cancel as easy as signup?
- [ ] No hidden costs, pre-ticked boxes, fake urgency, fake scarcity, fake reviews, confirmshaming or nagging?
- [ ] Are subscription terms (price, frequency, renewal, how to cancel) stated next to the purchase button?
- [ ] Is consent freely given with an equally easy reject option?

---

## Output template

Use this structure for audit reports. Keep it scannable. Adjust depth to the request (a quick review might only need the summary and top fixes).

```markdown
# UX audit. [Product / flow name]

**Scope.** [Screens or flow reviewed, device, user type assumed]
**Goal assumed.** [Primary business and user goal, and the key metric]

## Summary
[Two to four sentences on the overall state and the biggest opportunity.]

## Top three fixes
1. **[Fix]**. [Why, in one or two sentences, citing principle and grade.] Severity [n]. Effort [low / medium / high].
2. ...
3. ...

## What's working
- [Strength worth keeping, and why]

## Findings by step
### [Step or screen name]
| Issue | Friction type | Principle (grade) | Severity | Structural recommendation | Disqualified obvious fix |
|---|---|---|---|---|---|
| [What user experiences] | [Comprehension / Anxiety / Motor / Timing / Reactance] | [e.g. Hidden costs (B)] | 3 | [Structural change] | [Why tooltip/modal/etc. rejected] |

## Top bottleneck: Three structural solution angles
For the single highest-severity issue, provide three distinct directions (see `references/10-problem-solving-lateral-ux.md`):
- **Angle A (Subtractive / System):** [Eliminate the step, infer data, smart defaults]
- **Angle B (Cognitive / Risk Reversal):** [Dissolve anxiety, plain language, transparent guarantees]
- **Angle C (Structural / Timing Shift):** [Move ask post-value, reverse onboarding, inline controls]
- **Disqualified vanilla idea:** [Explicitly name the superficial band-aid and why it fails]

## Ethics and legal risk
[Each issue with the pattern name, the risk, and the fair alternative. Write "None found" if clean.]

## What to test
| Hypothesis | Primary metric | Guardrail |
|---|---|---|
| [Change X will improve Y because Z] | [Metric] | [Metric] |
```
