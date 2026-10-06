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
8. Psychology of waiting
9. Response time limits
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
**Evidence** B (Buell and Norton 2011, five experiments in online travel and dating. When sites showed the work being done, people sometimes preferred longer waits to instant results, even with identical results. A plain progress bar did not have the same effect).

**What it says.** Seeing the effort made on your behalf increases perceived value and reciprocity.

**Apply.**
- During longer processes, show what's happening ("Checking 400 airlines", "Comparing 12 quotes", "Scanning your document for key terms").
- Show the steps of complex work (AI generation, analysis, matching) as it happens.
- Summarize the work done ("We checked 34 sources").

**Limits.** Don't add fake delays to instant processes. The effect shows diminishing returns, and users eventually notice. Real speed still wins.

**Audit question.** During any wait, can users see the real work being done for them?

## 8. Psychology of waiting
**Evidence** B (Maister 1985. Widely supported in service operations research).

**What it says.** Unoccupied time feels longer than occupied time. Uncertain and unexplained waits feel longer than known and explained ones. Anxiety makes waits feel longer. Unfair waits feel longer than fair ones.

**Apply.**
- Tell users how long it will take and why.
- Give something useful to do or read during waits (tips, a preview, next steps).
- Reduce anxiety during payments and submissions ("Don't close this window, this takes about 10 seconds").
- Send updates for long processes (email when your export is ready).

**Audit question.** For every wait, do users know how long, why, and that it's working?

## 9. Response time limits
**Evidence** A to B (Miller 1968. Card, Moran and Newell 1983. Nielsen 1993). C for the Doherty threshold of 400 ms as a productivity claim (Doherty and Thadani 1982, an IBM paper).

**What it says.** About 0.1 s feels instant. About 1 s keeps flow of thought but the delay is noticed. About 10 s is the limit of attention, beyond which users switch tasks.

**Apply.**
- Under 100 ms, no indicator needed. Respond visually to every input within 100 ms, even if the work takes longer.
- 1 to 10 s, show a loading state.
- Over 10 s, show determinate progress, allow the user to do other things, and notify on completion.
- Track Core Web Vitals. Google's "good" thresholds are Largest Contentful Paint under 2.5 s, Interaction to Next Paint under 200 ms, and Cumulative Layout Shift under 0.1.

**Real speed matters.** Google and Deloitte's "Milliseconds Make Millions" study (37 brands, 2019 data) found a 0.1 s mobile speed improvement was associated with an 8.4% higher retail conversion rate and 10.1% for travel. It was commissioned by Google and based on natural variation, so treat the exact numbers as grade C and the direction as grade B.

**Audit question.** Does every action produce visible feedback within 100 ms, and do pages meet Core Web Vitals?

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
