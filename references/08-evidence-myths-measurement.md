# 08. Evidence, Myths and Measurement

How strong is the evidence, which popular "laws" are myths, and how to measure whether a change actually helped.

## Contents
1. Evidence grades in detail
2. Calibrating expectations (effect sizes shrink at scale)
3. Replication status table
4. Popular myths and what to say instead
5. Reading industry statistics critically
6. What to measure
7. A/B testing hygiene
8. Qualitative methods that catch what numbers miss

---

## 1. Evidence grades in detail

- **A, robust.** Supported by meta-analyses or many independent replications, ideally including field data. Examples include defaults, anchoring, the peak-end rule, Fitts's law, implementation intentions, and processing fluency.
- **B, solid but conditional.** Replicated or backed by large-scale industry research, with known moderators or modest effects. Examples include choice overload (only under specific conditions), social proof, goal gradient, endowed progress, the labor illusion, and Baymard's checkout findings.
- **C, promising but thin.** Single studies, small samples, commissioned research, correlational data, or practitioner heuristics. Examples include the Doherty threshold, skeleton screens, decoy pricing in real interfaces, and the Hook model. Recommend testing.
- **D, myth or failed replication.** Don't present as fact.

When an effect is graded A in the lab but untested in product contexts, say so (for example "A for the psychology, B for this use").

## 2. Calibrating expectations

- **Published effects are inflated.** DellaVigna and Linos 2022 compared 126 trials by two US government nudge units (covering 23 million people) with nudge trials published in academic journals. Academic nudges averaged an 8.7 percentage point increase in take-up. Nudge unit trials averaged 1.4 points (still significant, an 8% relative increase). About 70% of the gap was explained by selective publication and low statistical power.
- **Publication bias is severe in parts of the field.** Mertens et al. 2022 meta-analysis of 447 nudge effect sizes reported d = 0.43. Maier et al. 2022 reanalyzed it with corrections for publication bias and found no remaining evidence of an average effect. Later commentary clarified that some nudges clearly work (defaults among them), but the average is not a reliable guide.
- **Practical rule.** Expect single tactics to produce small, real gains when they work. Expect larger gains from removing real friction (errors, hidden costs, slow pages, forced accounts). Always test claims with large promised lifts.

## 3. Replication status table

| Finding | Status | Grade | Note |
|---|---|---|---|
| Default effect | Robust, heterogeneous | A | Jachimowicz et al. 2019, d = 0.68 |
| Anchoring | Robust | A | Replicated in Many Labs |
| Peak-end rule | Robust | A | Alaybek et al. 2022, 174 effect sizes |
| Fitts's law & target distance | Robust | A | Decades of HCI replication; Fitts 1954 |
| Law of Proximity (Gestalt) | Robust | A | Wertheimer 1923, foundational perceptual psychology |
| Law of Similarity (Gestalt) | Robust | A | Wertheimer 1923, visual grouping |
| Law of Uniform Connectedness | Robust | A | Palmer and Rock 1994, overrides proximity |
| Law of Prägnanz (Simplicity) | Robust | A | Wertheimer 1923, Köhler 1929 |
| Von Restorff (isolation) effect | Robust | A | von Restorff 1933, perceptual salience |
| Serial position effect (primacy/recency) | Robust | A | Ebbinghaus 1885, Murdock 1962 |
| Working memory chunking (4±1) | Robust | A | Cowan 2001 (revising Miller 1956) |
| Implementation intentions | Robust | A | Gollwitzer and Sheeran 2006, d = 0.65 |
| Processing fluency | Robust | A | Reber et al. 2004 |
| Hick's law | Robust in RT, conditional in UI | A to B | Hick 1952, Hyman 1953; breaks on complex trade-offs |
| Jakob's law | Supported heuristic | B | Nielsen 2000; schema theory |
| Tesler's law (complexity conservation) | Supported heuristic | B | Tesler 1984, Xerox PARC |
| Postel's law (robustness principle) | Supported standard | B | Postel 1980, RFC 760/793 |
| Occam's razor (parsimony in UI) | Foundational heuristic | B | Maeda 2006, Lidwell et al. 2010 |
| Pareto principle (80/20 usage) | Supported telemetry | B | Telemetry power-law distributions; Juran 1941 |
| Parkinson's law (task time expansion) | Supported | B | Parkinson 1955; behavioral economics |
| Choice overload | Conditional | B | Near-zero mean (Scheibehenne 2010), real under four moderators (Chernev 2015) |
| Loss aversion | Real, magnitude debated | B | Gal and Rucker 2018 |
| Goal gradient | Supported | B | Kivetz et al. 2006 |
| Endowed progress | Supported, few replications | B | Nunes and Drèze 2006 |
| Labor illusion | Supported | B | Buell and Norton 2011 |
| IKEA effect | Supported | B | Norton et al. 2012 |
| Social norms nudges | Real, modest at scale | B | Allcott 2011 about 2% |
| Aesthetic-usability effect | Mixed, can reverse after use | B | Tuch et al. 2012 |
| Doherty threshold 400 ms | Supported for flow | B to C | Doherty and Thadani 1982, Google CWV |
| Inline validation gains | Small sample | B to C | Wroblewski and Etre 2009, n = 22 |
| Decoy effect | Weakens with realistic stimuli | C | Frederick et al. 2014 |
| Skeleton screens feel faster | Mixed | C | Viget 2017 found the opposite |
| Ovsiankina resumption effect | Supported | B | Ghibellini and Meier 2025 meta-analysis |
| Zeigarnik memory effect | Failed to replicate | D | Ghibellini and Meier 2025 |
| Miller's law (7±2) for menus | Failed / Myth | D | Menus rely on visual recognition, not recall |
| Ego depletion | Failed large replications | D | Hagger et al. 2016 registered replication |
| Social priming (e.g. elderly-walking) | Failed replications | D | Doyen et al. 2012 |

## 4. Popular myths and what to say instead

- **"Seven plus or minus two items."** Miller's paper concerns working memory for things people must hold in mind. Menus are visible, so the rule doesn't apply. Say instead that menus should be well grouped and labeled, and that users shouldn't have to remember things across screens.
- **"The three-click rule."** Studies (including Porter 2003 at UIE) found no link between the number of clicks and success or satisfaction. Say instead that each click must clearly move users closer to their goal.
- **"Users don't scroll."** They do. NN/g 2018 found about 57% of viewing time above the fold and the rest below it. Say instead that attention drops sharply below the first screen, so put the essentials first and invite scrolling.
- **"Eight-second attention span, shorter than a goldfish."** Traced to an unsourced statistic. Attention depends on motivation and content.
- **"Users decide in 50 ms whether to stay."** The research measured aesthetic ratings at 50 ms. Say instead that first impressions of appeal form almost instantly and color later judgments.
- **"Red (or orange, or green) buttons convert best."** Famous button-color tests reflect contrast with the specific page. Say instead that the primary action should be the highest-contrast element.
- **"93% of communication is nonverbal."** Mehrabian studied single words with ambiguous emotional tone. Irrelevant to interface copy.
- **"People remember unfinished tasks better."** Not supported (Zeigarnik). People do tend to resume unfinished tasks (Ovsiankina).
- **"Hick's law means always cut options."** Organization and familiarity matter more than raw count for complex choices.
- **"Beautiful products are more usable."** First impressions, yes. After use, usability drives perceived beauty.
- **"Carousels increase engagement."** Industry data consistently shows low interaction beyond the first slide. Lead with the single most important message.
- **"Long-form landing pages always win" (or "short always wins").** It depends on the price, complexity and awareness level of the audience. Test.

## 5. Reading industry statistics critically

When citing a number, ask these questions.
- **Who funded it?** Vendor-commissioned studies (for example Google and Deloitte on site speed) can be useful, but give them grade C for exact magnitudes.
- **Is it causal?** Correlations between speed and conversion or between activation and retention don't prove that changing one changes the other.
- **What's the sample?** Baymard's abandonment reasons come from surveys of US adults. They capture stated reasons, which only approximate causes.
- **Is the base rate stated?** "270% more likely" relative to near-zero is very different from an absolute lift.
- **Is it current?** Behavior shifts (mobile share, wallet adoption, AI search). Prefer recent data for fast-moving topics.

## 6. What to measure

**Behavioral metrics**
- Conversion rate per funnel step, with drop-off between steps.
- Task success rate, time on task, error rate (from usability testing and analytics).
- Time to value and activation rate (share of new users reaching the key action).
- Retention cohorts (day 1, day 7, day 30, or week and month for B2B).
- Feature adoption and frequency.

**Attitudinal metrics**
- **SUS** (System Usability Scale). Ten items. The average across many studies is about 68. Above 80 is excellent.
- **SEQ** (Single Ease Question) after each task. Seven-point scale.
- **CES** (Customer Effort Score) for support and service flows.
- **CSAT** for specific interactions.
- **NPS** is widely used but a weak diagnostic. Pair it with the open-text "why".

**Frameworks**
- **Google's HEART.** Happiness, Engagement, Adoption, Retention, Task success, each mapped to goals, signals and metrics.

**Guardrail metrics** (always pair with conversion tests)
- Refunds, returns, chargebacks, cancellations within 30 days, support contacts, complaints, unsubscribe and notification opt-out rates, app uninstalls, negative reviews.

## 7. A/B testing hygiene

**Evidence** B (Kohavi, Tang and Xu 2020, "Trustworthy Online Controlled Experiments").

- Pre-register one primary metric, guardrails, minimum detectable effect and run time before starting.
- Calculate sample size and run for full weekly cycles. Don't stop early when it looks significant (peeking inflates false positives).
- Check for sample ratio mismatch (unequal group sizes signal a bug).
- Be wary of novelty effects. Check whether the lift holds after the first week or two.
- Twyman's law. Any result that looks surprisingly good is probably a bug. Investigate before celebrating.
- Most ideas fail. At large companies, a majority of experiments show no improvement. A low win rate is normal.
- Use long-term holdouts for changes that might trade future retention for present conversion.
- Low-traffic products should rely more on qualitative research and large, high-confidence changes than on testing small tweaks.

## 8. Qualitative methods that catch what numbers miss

- **Moderated usability testing.** Five users per round find most major issues in a flow (Nielsen and Landauer 1993). Run several small rounds rather than one large one.
- **Five-second test** for first impressions and clarity of value proposition.
- **First-click testing** for navigation and information scent.
- **Card sorting and tree testing** for information architecture.
- **Session recordings and heatmaps** to find rage clicks, dead clicks and confusion.
- **Exit and on-page surveys** ("What stopped you from completing your purchase today?").
- **Support tickets and sales call notes** as a free source of real user language and pain points.
