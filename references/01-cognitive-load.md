# 01. Cognitive Load and Comprehension

How much thinking a screen demands, and how to reduce the thinking that doesn't help the user.

## Contents
1. Cognitive load theory
2. Working memory limits (and the 7 plus or minus 2 myth)
3. Recognition over recall
4. Chunking
5. Hick-Hyman law
6. Choice overload (and when it actually happens)
7. Progressive disclosure
8. Tesler's law (conservation of complexity)
9. Satisficing and scanning
10. Information scent and foraging
11. Mental models and Jakob's law
12. Prototypicality and convention
13. Consistency and standards
14. Split attention and redundancy
15. Help at the point of need
16. Plain language
17. Interruption and resumption
18. Smart defaults as load reducers

---

## 1. Cognitive load theory
**Evidence** A (Sweller 1988 onward, large instructional design literature).

**What it says.** Working memory is small. Load comes from the task itself (intrinsic), from how it is presented (extraneous), and from building understanding (germane). Designers can rarely change intrinsic load but can almost always cut extraneous load.

**Apply.**
- Strip anything that doesn't help the current decision, such as decorative copy, duplicate links, unnecessary options and jargon.
- One primary task per screen. Split genuinely complex tasks into steps.
- Keep related information together so users don't have to hold it in memory while looking elsewhere.
- Use visual structure (headings, grouping, whitespace) so parsing the page costs less.

**Limits.** Experts tolerate and often prefer dense screens. Over-splitting creates its own load (more navigation, lost context).

**Audit question.** Is there anything on this screen the user must process that doesn't help them complete this step?

## 2. Working memory limits
**Evidence** A for the limit itself (Cowan 2001 suggests about 4 chunks). D for "menus need 7 items or fewer."

**What it says.** People can hold only a few chunks of information in mind at once. Miller's 1956 "seven plus or minus two" is widely misapplied to visible interfaces. Users don't need to memorize a menu they can see.

**Apply.**
- Never make users carry information from one screen to the next. Repeat the key facts (plan chosen, price, dates) where they are needed.
- Show order summaries in checkout, the selected filters on results, and the item being edited in forms.
- Keep codes, OTPs and reference numbers copyable and visible when they are needed.

**Limits.** The limit matters for things users must remember, much less for things they can see.

**Audit question.** Does the user ever have to remember something from a previous screen to act on this one?

## 3. Recognition over recall
**Evidence** A (memory research shows recognition is easier than recall), B as a usability heuristic (Nielsen 1994).

**What it says.** Seeing options is easier than remembering them.

**Apply.**
- Visible navigation over hidden menus for key destinations on desktop. On mobile, a bottom tab bar for the top three to five destinations.
- Autocomplete, recent searches, recently viewed items, and saved addresses.
- Icons with text labels. Unlabeled icons force recall of meaning.
- Show examples and format hints next to inputs.

**Audit question.** Where does the user have to remember a command, a name, a code or a location instead of picking it?

## 4. Chunking
**Evidence** A.

**What it says.** Grouping items into meaningful units lets people process more.

**Apply.**
- Format numbers (card numbers in groups of four, phone numbers by local convention).
- Group form fields into labeled sections (contact, delivery, payment).
- Break long content into short sections with descriptive headings.

**Audit question.** Are long lists, numbers or forms broken into meaningful groups?

## 5. Hick-Hyman law
**Evidence** A in lab reaction time tasks. B to C for complex UI decisions.

**What it says.** Decision time rises with the logarithm of the number of equally likely choices. In real interfaces, scanning, familiarity and how options are organized matter more than raw count.

**Apply.**
- Reduce choices at moments of decision (plan selection, primary CTAs). One primary action, at most one or two secondary actions.
- Organize large sets (categories, search, filters) instead of hiding them.
- Highlight a recommended option when users lack expertise.

**Limits.** Splitting one menu of 20 into four nested menus of 5 often makes things slower because of extra navigation. Breadth with good grouping usually beats depth.

**Audit question.** At the key decision point, how many options compete for the click, and is the recommended one obvious?

## 6. Choice overload
**Evidence** B, conditional. The famous jam study (Iyengar and Lepper 2000) found fewer purchases from a 24-jam display than a 6-jam one. A 2010 meta-analysis (Scheibehenne, Greifeneder and Todd) found a mean effect near zero. A 2015 meta-analysis (Chernev, Böckenholt and Goodman, 99 observations) found the effect is real when four moderators are present.

**What it says.** Large assortments hurt choice when the choice set is complex, the task is difficult, preferences are uncertain, and the person wants to minimize effort. Otherwise more choice can help.

**Apply.**
- Large catalogs are fine if users can filter, sort and compare. Provide those tools.
- When users are novices or the options are hard to compare (insurance, SaaS plans, mattresses), reduce the set, recommend one, or offer a quiz or guided selector.
- Make options easy to compare with aligned attributes in a table.

**Limits.** Experts and people with clear preferences often want breadth. Don't cut range to fix what is really a navigation problem.

**Audit question.** Are users facing many hard-to-compare options with no recommendation, filter or comparison aid?

## 7. Progressive disclosure
**Evidence** B (NN/g, long practitioner use).

**What it says.** Show what most people need first and reveal advanced options on request. It reduces load for novices without removing power for experts.

**Apply.**
- Basic and advanced settings, with advanced collapsed.
- Ask for the minimum at signup, gather the rest when it becomes relevant.
- Use expandable details, "show more" and tooltips for secondary information.
- Staged disclosure in wizards for genuinely sequential tasks.

**Limits.** Hide only what is rarely needed. Hiding something important (fees, terms, cancellation) is a dark pattern. Use at most two levels of disclosure, as deeper nesting gets lost.

**Audit question.** Is the default view focused on what most users need, with everything else one clear click away?

## 8. Tesler's law (conservation of complexity)
**Evidence** C (practitioner principle, widely accepted).

**What it says.** Every task has irreducible complexity. Someone has to deal with it, either the system or the user. Good design moves it to the system.

**Apply.**
- Detect instead of asking (location for country, card type from number, city from postcode).
- Calculate instead of making users calculate (totals, delivery dates, savings).
- Handle formatting in code instead of demanding exact formats.

**Audit question.** What is the user doing that the system could do for them?

## 9. Satisficing and scanning
**Evidence** A for satisficing as a decision strategy (Simon 1956). B for web behavior (Krug, NN/g eyetracking).

**What it says.** Users don't read and optimize. They scan for the first reasonable option and click it. They muddle through without figuring out how things work.

**Apply.**
- Front-load headings, links and buttons with the most informative words.
- Make the right choice the obvious first candidate.
- Write button labels that say what happens ("Start free trial", "Pay £42.00") instead of "Submit" or "Continue".
- Expect users to skip instructions. Build the guidance into the interface itself.

**Audit question.** If a user clicked the first plausible thing on this screen, would it be the right thing?

## 10. Information scent and foraging
**Evidence** B (Pirolli and Card 1999, information foraging theory, plus extensive NN/g research).

**What it says.** Users follow cues (link text, labels, images) that predict whether a path leads to their goal. Weak scent causes backtracking and abandonment.

**Apply.**
- Use the user's words in navigation and links, found through search logs, support tickets and card sorting.
- Specific labels ("Pricing", "Track my order") over clever or vague ones ("Solutions", "Explore").
- Show previews on category and result pages (thumbnails, counts, key attributes).
- Make sure the destination confirms the scent with a matching heading.

**Audit question.** Does each link and label clearly predict what's behind it, using words the user would use?

## 11. Mental models and Jakob's law
**Evidence** B (Nielsen, NN/g, Norman).

**What it says.** Users bring expectations from everything else they use. Jakob's law says users spend most of their time on other sites, so they prefer yours to work the same way.

**Apply.**
- Logo top left links home, cart top right, search with a magnifier, underlined or clearly styled links, standard form controls.
- Use platform conventions on mobile (iOS and Android patterns differ).
- When changing a familiar design, let users adapt (preview, opt in, explain changes).

**Limits.** Convention can be broken when the gain is large and the new pattern is quickly learnable. Test it.

**Audit question.** Does anything behave differently from how the same element works on the major sites this audience uses?

## 12. Prototypicality and convention
**Evidence** B (Tuch et al. 2012, Google and University of Basel).

**What it says.** Users judge sites that look typical for their category as more appealing, within 17 to 50 milliseconds. Low visual complexity combined with high prototypicality scored best.

**Apply.**
- Make the site look like a member of its category (a bank should look like a bank) and differentiate through brand, voice and quality.
- Keep the first screen visually simple.

**Audit question.** Would a user instantly recognize what kind of product this is from a glance?

## 13. Consistency and standards
**Evidence** B (Nielsen heuristic 4).

**What it says.** The same thing should look and behave the same way everywhere. Different things should look different.

**Apply.**
- Use a design system with one style per role (one primary button style, one link style, one error style).
- Keep terminology stable. Don't call it "workspace" on one screen and "project" on another.
- Keep placement consistent for repeated actions (save, next, close).

**Audit question.** Is anything named, styled or placed inconsistently across screens?

## 14. Split attention and redundancy
**Evidence** A (cognitive load theory in instructional design).

**What it says.** When people must integrate two separate sources (a diagram and its distant legend, a form and a help panel elsewhere), load rises. Saying the same thing twice in different forms can also add load.

**Apply.**
- Put labels directly on charts instead of in separate legends.
- Place help text next to the field it explains.
- Don't narrate on-screen text word for word in onboarding videos.

**Audit question.** Does the user have to look in two places to understand one thing?

## 15. Help at the point of need
**Evidence** B (NN/g on onboarding tutorials and contextual help).

**What it says.** Upfront tutorials are often skipped and quickly forgotten. Help delivered at the moment it's relevant is more effective.

**Apply.**
- Prefer contextual tips, empty-state guidance and inline hints over long upfront tours.
- If you use a tour, keep it short, skippable and tied to doing a real action.
- Make help retrievable later.

**Audit question.** Is guidance delivered when the user needs it, or front-loaded before they care?

## 16. Plain language
**Evidence** B (GOV.UK, plainlanguage.gov, NN/g research showing even experts prefer plain text).

**What it says.** Short sentences, common words and active voice are faster to read for everyone, including specialists.

**Apply.**
- Aim for around a grade 8 reading level for general consumer products.
- Lead with the point. One idea per sentence.
- Replace jargon with the user's words. Define unavoidable terms inline.
- Write numbers as numerals and use specific values ("Arrives Thursday 9 October" instead of "3 to 5 business days" when you can).

**Audit question.** Could a tired person on a phone understand every sentence on the first read?

## 17. Interruption and resumption
**Evidence** B for the urge to resume unfinished tasks (Ovsiankina effect, confirmed by Ghibellini and Meier 2025 meta-analysis). D for the claim that unfinished tasks are remembered better (Zeigarnik memory effect, not replicated in the same meta-analysis).

**What it says.** People tend to return to tasks they started. They don't reliably remember them better.

**Apply.**
- Save progress automatically in long flows and forms. Let people return to where they left off.
- Show "continue where you left off" on return.
- Remind of unfinished tasks with useful, infrequent, easy-to-dismiss prompts (abandoned cart email, incomplete profile).

**Limits.** Excessive reminders become nagging (see 07).

**Audit question.** If a user leaves mid-flow, is their work saved and easy to resume?

## 18. Smart defaults as load reducers
**Evidence** A for defaults changing behavior (see 03). B for defaults as a usability tool.

**What it says.** Most users keep defaults. A good default answers the question for the majority so they can skip it.

**Apply.**
- Preselect the most common, user-beneficial option (standard shipping, user's country, current date).
- Prefill from what you already know (billing same as shipping, checked by default).
- Make defaults easy to see and change.

**Limits.** Defaults that serve the business at the user's expense (pre-ticked add-ons, opt-in marketing) are dark patterns and in many places illegal.

**Audit question.** Does each question have a sensible default that most users would choose anyway?
