# 05. Emotion, Memory and Delight

How experiences feel in the moment and how they are remembered afterwards. Satisfaction, word of mouth and return visits come from the remembered experience.

## Contents
1. Peak-end rule
2. Duration neglect
3. Norman's three levels of emotional design
4. Kano model
5. Delight that lasts
6. Microinteractions
7. Labor illusion and operational transparency
8. Psychology of waiting, chronoperception and occupied time
9. Response time limits and the Doherty threshold
10. Perceived performance techniques
11. Skeleton screens and spinners
12. Optimistic UI
13. Error messages and tone
14. Forgiveness and undo
15. Celebration moments
16. Voice and tone
17. Humor
18. Endings and confirmation screens
19. Service recovery
20. Mere exposure and familiarity
21. Hedonic adaptation

---

## 1. Peak-end rule
**Evidence** A. Kahneman et al. 1993 (cold water study) and Redelmeier and Kahneman 1996 (colonoscopy). Alaybek et al. 2022 meta-analysis of 174 effect sizes found a large, robust peak-end effect (around r = .57), comparable to the overall average experience, with duration mattering very little.

**What it says.** People remember experiences mainly by the most intense moment and the end.

**Apply.**
- Find the worst moment in a flow (a confusing form, a surprise fee, a slow step) and fix it first. A bad peak dominates memory.
- Create a genuine positive peak (the moment of value, a clear win, a well-crafted reveal).
- End well. The confirmation screen, the last step of onboarding, the cancellation flow, and the support ticket closure all shape memory.
- Put mandatory unpleasant steps early and finish with something pleasant or reassuring.

**Limits.** The overall average still matters, as the meta-analysis found. The peak-end rule is no excuse for a mediocre middle.

**Audit question.** What is the most negative moment in this flow, and how does it end?

## 2. Duration neglect
**Evidence** A (Fredrickson and Kahneman 1993. Supported in Alaybek et al. 2022).

**What it says.** How long an experience lasted barely affects how it's remembered.

**Apply.**
- A slightly longer flow that feels smooth can be remembered better than a short one with a painful step.
- Don't cut steps that reduce anxiety (a review step before payment) just to make the flow shorter.

**Audit question.** Have we made the flow shorter at the cost of making it feel worse?

## 3. Norman's three levels of emotional design
**Evidence** Framework (Norman 2004).

**What it says.** Products are experienced at three levels. Visceral (instant look and feel), behavioral (how it works in use), and reflective (what it means to me, how it makes me look and feel about myself).

**Apply.**
- Visceral. Polish, beautiful defaults, satisfying feedback.
- Behavioral. Speed, reliability, control, few errors. This level carries most satisfaction.
- Reflective. Brand story, identity, the feeling of being smart or good for using it, shareable outcomes.

**Audit question.** Does the product deliver at all three levels, with behavioral quality first?

## 4. Kano model
**Evidence** B as a framework (Kano 1984. Widely used in product management).

**What it says.** Features fall into basics (absence causes anger, presence goes unnoticed), performance (more is better) and delighters (unexpected, cause joy). Delighters become basics over time.

**Apply.**
- Fix basics first. No delighter compensates for a missing basic (working search, saved cart, reliable sync).
- Invest in the performance attributes users care most about (speed, accuracy, price).
- Add a few delighters, and expect to keep raising the bar.

**Audit question.** Are all the basics flawless before we spend effort on delight?

## 5. Delight that lasts
**Evidence** B (NN/g and Aarron Walter's hierarchy of user needs, which runs from functional to reliable to usable to pleasurable).

**What it says.** Surface delight (animations, playful copy) only lands on a product that already works. Deep delight comes from a product that anticipates needs and removes effort.

**Apply.**
- Anticipate (prefill, remember preferences, suggest the next step).
- Remove effort in surprising ways (auto-detect, one-tap reorder, smart defaults).
- Add surface delight in low-stakes, frequent moments, and keep it brief.

**Audit question.** Where could the product save the user effort they expected to spend?

## 6. Microinteractions
**Evidence** Framework (Saffer 2013).

**What it says.** Single-purpose moments (toggling, liking, pulling to refresh, saving) consist of a trigger, rules, feedback, and loops and modes. They carry much of a product's feel.

**Apply.**
- Every interactive element needs clear states (default, hover, focus, active, disabled, loading, success, error).
- Give instant, proportionate feedback (a subtle check on save, a button that shows progress during submit).
- Make feedback consistent across the product.
- Small haptic feedback on mobile for confirmations, used sparingly.

**Audit question.** Does every interactive element respond instantly and clearly in every state?

## 7. Labor illusion and operational transparency
**Evidence** B (Buell and Norton 2011, Harvard Business School, *Management Science*; five experiments in online travel and dating. When websites showed the computational work being performed, users rated outcomes as more valuable and reported higher satisfaction with longer waits than with instantaneous results or blank progress bars).

**What it says.** Seeing the effort, rigor, or computation exerted on your behalf increases perceived quality, trust, and reciprocity. If a system completes an extraordinarily complex task instantaneously behind a blank screen, users often discount its thoroughness. Conversely, showing real-time operational transparency justifies the wait and elevates perceived craft.

**Apply.**
- **Operational transparency:** During processes exceeding 1.5 seconds, display a running stream of genuine sub-tasks ("Scanning 42 airline databases...", "Verifying SSL certificate...", "Checking DNS propagation...", "Comparing 18 pricing tiers...").
- **AI thought and task streaming:** Expose the model's reasoning stages or pipeline milestones (e.g., *"Analyzing schema $\to$ Generating unit tests $\to$ Linting output"*).
- **Summary of labor on completion:** Close the loop by explicitly stating the work done: *"Scanned 14,200 records across 4 regions in 1.4 seconds."*

**Limits & Anti-patterns.** Never inject artificial, fake `sleep()` delays into instant operations to fake effort. Users and developers quickly detect phony spinners, destroying trust. Operational transparency is for *communicating real work*, not fabricating synthetic toil.

**Audit question.** During any wait over 1.5 seconds, can users see the real work, milestones, and computational effort being executed for them?

## 8. Psychology of waiting, chronoperception and occupied time
**Evidence** B (David Maister 1985, *The Psychology of Waiting Lines*; Christopher Hsee, Adelle Yang, and Liangyan Wang 2010, *Psychological Science*; Chris Harrison et al. 2007 ACM UIST & 2010 ACM CHI; Richard Oliver 1980, *Expectation Disconfirmation Theory*).

**What it says.** The subjective experience of time (**chronoperception**) rarely matches clock time. How a user *feels* about a delay is driven far more by cognitive occupation, anxiety, and perceived equity than by actual millisecond duration.

### Classic Lateral Case Studies
- **The Elevator Mirror Paradox:** In mid-20th-century New York high-rises, building managers faced intense tenant complaints regarding slow elevators. Mechanical engineers proposed expensive new motors and extra elevator shafts costing hundreds of thousands of dollars. A psychologist suggested installing full-length mirrors in lobbies and elevator cabs. Waiting tenants adjusted their ties, fixed their hair, and observed others. **Occupied time replaced unoccupied time.** Complaints dropped to near zero without altering elevator speed by a single millisecond.
- **The Houston Airport Baggage Claim:** Passengers arrived at gates, walked 1 minute to baggage claim, and stood for 7 minutes waiting for carousels to turn, producing heavy complaints. The airport spent millions optimizing ground crews, shaving wait times to 6 minutes—yet complaints persisted. The airport reframed the problem: walking is *occupied time*; standing stagnant is *unoccupied time*. They moved arrival gates to the farthest concourse. Passengers now walked for 6 minutes and waited 1 minute. Complaints dropped to zero.

### Maister's Core Principles of Waiting Lines (1985)
1. **Occupied time feels shorter than unoccupied time.** Mental engagement distracts attention from the passage of time.
2. **People want to get started.** Preprocess waits feel longer than in-process waits. Letting a user begin entering metadata, customizing options, or viewing a preview while background setup occurs eliminates the perceived start delay.
3. **Uncertain waits feel longer than known, finite waits.** A known 45-second countdown feels shorter and far calmer than an indefinite spinning circle that could take 5 seconds or 5 minutes.
4. **Unexplained waits feel longer than explained waits.** Users tolerate delays when they understand the cause ("Compiling 48 assets..."), but grow anxious when the system gives no rationale.
5. **Anxiety makes waits feel longer.** Fear of double-charging, lost drafts, or broken forms amplifies perceived duration. Reassurance (*"Your spot is reserved. Please do not refresh"*) compresses perceived time.
6. **Unfair waits feel longer than equitable waits.** Violations of First-In-First-Out (FIFO) or perceived queue jumping trigger intense user reactance.
7. **The more valuable the service, the longer users tolerate waiting.**
8. **Solo waits feel longer than group or socially validated waits.**

### Idleness Aversion & Justifiable Busyness (Hsee et al. 2010)
Humans naturally dread idleness, but require a minimal justification to be busy. When interfaces provide users with a light, justifiable task during a backend operation (e.g. answering a quick preference question, reading a relevant tip, or tweaking an optional setting), user mood and reported satisfaction increase dramatically compared to forcing them to sit idle.

### Progress Bar Chronoperception (Harrison et al. 2007, 2010)
- **Accelerating Progress Bars:** A progress bar that starts with steady, predictable movement and accelerates toward 100% is perceived as up to **11% faster** than a bar that fills at a constant mathematical rate.
- **Backward Optical Flow (Visual Doppler Effect):** Progress bars with animated backward-moving ripples or pulsing bands (moving leftwards while the bar fills rightwards) reduce perceived wait time by **12%**.
- **The 99% Freeze Trap:** Pauses at the beginning of a wait are readily forgiven; pausing or freezing at 99% triggers severe anxiety, destroys trust, and ruins the remembered experience (violating the **Peak-End Rule**). If a long tail is unavoidable, keep the bar at 90% while cycling active status micro-copy rather than stalling at 99%.

### Pipelined Interleaved Waiting (Active vs. Passive Sequencing)
Convert sequential blocking steps into parallel active tasks:
- *Anti-Pattern (Serial Blocking):* Select video $\to$ wait 90s for upload to finish $\to$ enter title and tags $\to$ submit.
- *Lateral Pattern (Pipelining):* Select video $\to$ upload begins immediately in the background while the user fills title, description, thumbnail, and tags. By the time the user finishes typing, upload is complete. **Perceived wait time: 0 seconds.**

### Expectation Disconfirmation (Oliver 1980)
$\text{Satisfaction} = \text{Perceived Experience} - \text{Expectation}$.
Always under-promise and over-deliver on estimated durations. Stating *"This operation takes approximately 60 seconds"* when it reliably takes 35 seconds produces **positive disconfirmation** (delight). Stating *"Just a moment..."* when it takes 20 seconds produces **negative disconfirmation** (frustration).

**Audit question.** For every wait exceeding 1 second: Is unoccupied time transformed into occupied or transparent time? Is the wait finite and explained? Are subsequent tasks pipelined to run during background processing?

## 9. Response time limits and the Doherty threshold
**Evidence** A for sensory reaction time (Miller 1968; Card, Moran and Newell 1983; Nielsen 1993). B for user productivity and flow preservation under 400 ms (Doherty and Thadani 1982 IBM research report; Google Core Web Vitals data).

**What it says.** Computer response time dictates the cognitive rhythm of human interaction. When computer response time drops below 400 ms, user interaction rate and productivity increase non-linearly because neither party is forced to wait for the other, keeping the user in a continuous cognitive flow state.
- **$\le 100\text{ ms}$ (Instantaneous):** The user feels direct, physical manipulation. Required for button presses, hover states, input typing, and toggle switches.
- **$\le 400\text{ ms}$ (Doherty Threshold):** **Interactions within 400 milliseconds.** The upper boundary for keeping user-system dialogue seamless and preventing the user's mind from wandering to secondary thoughts. UI state updates, dropdown opens, and client filtering should resolve within this window.
- **$1.0\text{ s}$ (Flow Limit):** The user notices a delay, but their train of thought remains intact. A subtle inline loader or progress indicator is required.
- **$10\text{ s}$ (Attention Limit):** The absolute boundary of single-task attention. Beyond 10 seconds, users switch tabs, multitask, or abandon. Demands determinate progress bars and background notifications.

**Apply.**
- **Interactions within 400 milliseconds.** Ensure client-side interactions, modal appearances, and view filtering complete within 400 ms.
- Provide immediate sensory feedback within 100 ms (pressed states, skeleton shells, instant checkbox ticks).
- For asynchronous requests exceeding 400 ms, employ **Optimistic UI** (render the predicted success state immediately in the client and roll back gracefully on error).
- Target Google Core Web Vitals benchmarks: Largest Contentful Paint (LCP) under 2.5 s, Interaction to Next Paint (INP) under 200 ms, and Cumulative Layout Shift (CLS) under 0.1.

**Real speed matters.** Google and Deloitte's "Milliseconds Make Millions" study found a 0.1 s mobile speed improvement yielded an 8.4% lift in retail conversions and 10.1% in travel. Treat exact magnitudes as Grade C (correlational) and the directional impact as Grade B.

**Audit question.** Does every user action produce visible feedback within 100 ms, and do transitions and feedback complete within the 400 ms Doherty threshold?

## 10. Perceived performance techniques
**Evidence** B to C.

**Apply.**
- Render the page frame and content progressively. Show text before images.
- Preload likely next pages (hover intent, prefetching the next step).
- Lazy-load below-the-fold media.
- Reserve space for images and ads to prevent layout shift.
- Move work out of the critical path (send analytics later, process uploads in the background).

**Audit question.** What can the user see and do while the rest loads?

## 11. Skeleton screens and spinners
**Evidence** C, mixed. Viget's 2017 test (136 participants) found the skeleton screen produced the longest perceived wait, longer than a spinner or a blank screen. Other studies report the opposite. Results likely depend on duration and how closely the skeleton matches the final layout.

**Apply.**
- For waits under about 300 ms, show nothing (a flash of loading state looks glitchy).
- For short waits with known layout, a skeleton that closely matches the final content is reasonable.
- For unknown layouts or in-place actions, a spinner or button-level progress is fine.
- For long waits, use determinate progress and the labor illusion.
- Test perceived speed with your own users if loading is a major part of the experience.

**Audit question.** Is the loading pattern appropriate to the wait length, and does it avoid flicker?

## 12. Optimistic UI
**Evidence** B (common practice in high-quality apps).

**What it says.** Show the result of an action immediately, assuming success, and reconcile with the server in the background.

**Apply.**
- Likes, saves, toggles, reordering, sending messages.
- Roll back clearly if the action fails, with a retry option.

**Limits.** Not for payments, deletions of important data, or anything where a false success would harm the user.

**Audit question.** Are low-risk actions instant from the user's point of view?

## 13. Error messages and tone
**Evidence** B (NN/g error message guidelines. Baymard checkout research).

**What it says.** Errors are peak negative moments. A good error message says what happened, why, and exactly how to fix it, without blaming the user.

**Apply.**
- Specific ("Card number is missing 2 digits") beats generic ("Invalid input").
- Place the message next to the problem, in plain language, with a visible color and icon.
- Preserve everything the user entered. Never clear a form on error.
- Avoid blame ("You entered an invalid...") and avoid jokes in serious errors.
- For system errors, apologize briefly, explain what's being done, and offer a path (retry, contact, save for later).

**Audit question.** For each error, does the user know what went wrong and how to fix it, with their work intact?

## 14. Forgiveness and undo
**Evidence** B (Raskin 2000. Nielsen heuristic 3. Gmail's "Undo send" is a classic example).

**What it says.** Confirmation dialogs get clicked through by habit. Undo protects users without slowing them down.

**Apply.**
- Offer undo for reversible actions (delete, archive, send, move) via a toast with an Undo button for several seconds.
- Use soft delete (trash with recovery period).
- Reserve confirmation dialogs for irreversible, high-stakes actions, and make the confirm button name the action ("Delete 14 files").
- For very destructive actions, require typing a name or similar deliberate friction.

**Audit question.** Can users recover from mistakes easily, without being nagged by confirmations for everyday actions?

## 15. Celebration moments
**Evidence** C (industry practice, consistent with competence and peak-end research).

**Apply.**
- Celebrate meaningful milestones (first project shipped, first sale, course completed). Leave routine actions with simple feedback.
- Keep celebrations short and skippable. Respect reduced-motion preferences.
- Pair celebration with the next step ("Your store is live. Share it with your first customer").

**Limits.** Celebrating trivial actions feels patronizing, and frequent celebrations lose effect.

**Audit question.** Is there a well-earned celebration at the user's first real success?

## 16. Voice and tone
**Evidence** B (NN/g 2016 tone-of-voice study found tone measurably affected perceptions of friendliness, trustworthiness and desirability. Casual and conversational tones generally performed well. Irreverent tones were riskier, especially in serious domains).

**Apply.**
- Define a consistent voice and adapt tone to context (lighter in success, plain and calm in errors, serious in money, health and security).
- Write as a helpful person would speak. Use "you", short sentences, and active voice.
- Make microcopy do work (button labels that state the outcome, helper text that prevents errors).

**Audit question.** Does the tone fit the emotional context of each moment?

## 17. Humor
**Evidence** C (context dependent).

**Apply.**
- Small, light humor in low-stakes places (empty states, 404 pages, loading tips) can build affection.
- Never in errors involving money, data loss, health, or when the user is frustrated.
- Humor rarely translates well. Be careful in localized products.

**Audit question.** Would this joke still land for a user having a bad day?

## 18. Endings and confirmation screens
**Evidence** B (peak-end research. Baymard order confirmation research).

**Apply.**
- Confirm clearly what happened, with key details (order number, what, when, where, total).
- Say what happens next and when ("We'll email you when it ships, usually within 24 hours").
- Offer useful next actions (track order, invite teammates, start the first task). Light cross-sell is fine if relevant.
- Send a matching confirmation email immediately.
- Offer account creation here for guest buyers, with details prefilled.

**Audit question.** Does the final screen leave the user confident, informed and feeling good?

## 19. Service recovery
**Evidence** B. A meta-analysis by de Matos, Henrique and Rossi 2007 found a service recovery paradox for satisfaction (excellent recovery can leave customers more satisfied than if nothing had gone wrong) but not reliably for loyalty or repurchase.

**Apply.**
- When things go wrong (outage, late delivery, billing mistake), acknowledge fast, explain honestly, fix it, and compensate proportionately.
- Proactive notification of problems beats users discovering them.
- Never design failures on purpose to trigger the paradox. It's unreliable.

**Audit question.** When something fails, does the product tell users first and make it right?

## 20. Mere exposure and familiarity
**Evidence** A (Zajonc 1968. Bornstein 1989 meta-analysis).

**What it says.** Repeated exposure increases liking, up to a point.

**Apply.**
- Consistent brand and UI patterns across touchpoints (site, app, email, packaging).
- Gradual changes over sudden redesigns for established products.

**Audit question.** Is the experience consistent across every channel the user sees?

## 21. Hedonic adaptation
**Evidence** A (Brickman and Campbell 1971 and later work).

**What it says.** People adapt to pleasures and improvements. Delight fades.

**Apply.**
- Vary surface delight occasionally, and keep investing in deep value.
- Show cumulative value periodically (year in review, time saved this month) to remind users of benefits they've adapted to.

**Audit question.** Do we remind users of the value they've stopped noticing?
