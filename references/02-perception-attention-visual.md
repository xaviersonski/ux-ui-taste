# 02. Perception, Attention and Visual Design

How people see a screen, where their eyes and fingers go, and how visual quality shapes trust and feeling.

## Contents
1. First impressions in milliseconds
2. Visual complexity and prototypicality
3. Aesthetic-usability effect (and its reversal)
4. Processing fluency
5. Visual hierarchy
6. Gestalt principles
7. Scanning patterns
8. The fold and scroll depth
9. Left-side bias
10. Banner blindness
11. Von Restorff (isolation) effect
12. Serial position effect
13. Fitts's law
14. Touch target size and the thumb zone
15. Affordances and signifiers
16. Icons and labels
17. Typography and readability
18. Color and contrast
19. Motion and animation
20. Density and whitespace
21. Change blindness and feedback location
22. Imagery and faces

---

## 1. First impressions in milliseconds
**Evidence** B (Lindgaard et al. 2006 found reliable visual appeal judgments after 50 ms. Tuch et al. 2012 found effects at 17 ms).

**What it says.** People form a gut aesthetic judgment almost instantly. That judgment colors later perceptions of credibility and quality.

**Apply.**
- The first screen should be calm, well aligned and clearly typical of its category.
- Avoid clutter, competing focal points and low-quality imagery above the fold.
- Make sure the first paint is stable (no layout shift) so the first impression isn't of something broken.

**Limits.** A good first impression buys attention for a few seconds. Content and usability decide what happens next. The popular claim that users "decide to stay or leave in 50 ms" overstates the research, which measured appeal ratings.

**Audit question.** Shown for half a second, does this screen feel clean, credible and recognizable?

## 2. Visual complexity and prototypicality
**Evidence** B (Tuch et al. 2012. Reinecke et al. 2013 found visual complexity and colorfulness predict appeal, with preferences varying by demographics).

**What it says.** Low complexity plus high prototypicality is judged most appealing. Complexity is processed first.

**Apply.**
- Limit the number of distinct elements, colors and type styles on the first screen.
- Use a recognizable layout for the category, and express brand through color, type, imagery and voice.

**Audit question.** Count the distinct visual elements in the first viewport. Can any be removed?

## 3. Aesthetic-usability effect
**Evidence** B, mixed. Kurosu and Kashimura 1995 and Tractinsky 2000 found attractive interfaces were rated more usable. Tuch, Roth, Hornbæk, Opwis and Bargas-Avila 2012 (80 participants, online shop) found aesthetics did not affect perceived usability, while poor usability lowered post-use aesthetic ratings.

**What it says.** Beauty helps first impressions and goodwill. After real use, usability dominates, and frustration makes products look worse in memory.

**Apply.**
- Invest in visual polish, especially for first impressions and marketing pages.
- Never trade usability for aesthetics on task flows. A beautiful checkout that confuses users will be remembered as ugly.
- Polish the details users touch most (buttons, inputs, transitions).

**Audit question.** Is any visual choice making the task harder (low-contrast text, hidden controls, style over clarity)?

## 4. Processing fluency
**Evidence** A (Reber, Schwarz and Winkielman 2004 and much replication).

**What it says.** Things that are easier to perceive and process feel more true, more likeable, more familiar and less risky. Hard-to-read instructions make a task seem harder.

**Apply.**
- Use legible fonts, good contrast and simple language for anything you want users to trust or attempt.
- Make the steps to start something look simple (short first step, clear typography).
- Use consistent, repeated visual patterns so the interface becomes familiar.

**Limits.** Some studies find disfluency increases careful thinking. Disfluency is rarely worth it in product UI, though for confirming a big risky action a moment of friction can be appropriate.

**Audit question.** Is anything harder to read or parse than it needs to be?

## 5. Visual hierarchy
**Evidence** B (perception research plus extensive practitioner evidence).

**What it says.** Size, weight, contrast, color, position and spacing tell users what matters and in what order.

**Apply.**
- Decide the reading order before designing. Make it visible with a clear size and weight scale (for example a type scale with a ratio around 1.2 to 1.333).
- One dominant element per screen, usually the headline or the primary action.
- Primary buttons high contrast and filled. Secondary buttons outlined or text. Destructive actions distinct and never styled as the primary.
- Use the squint test. Blur the screen and see what stands out.

**Audit question.** With the screen blurred, is the most important element the most visible one?

## 6. Gestalt principles
**Evidence** A for perception. B for application.

**What it says.** People group what is close (proximity), similar (similarity), enclosed together (common region), aligned or flowing (continuity), and complete shapes (closure). They separate figure from ground.

**Apply.**
- Space between groups larger than space within groups. Labels sit closer to their own field than to the previous field.
- Same style for same function.
- Cards and containers to group related content, used sparingly.
- Align to a grid so the eye follows clean lines.

**Audit question.** Does spacing alone make it clear what belongs together?

## 7. Scanning patterns
**Evidence** B (NN/g eyetracking studies 2006 to 2017).

**What it says.** Users scan. The F-pattern (two horizontal sweeps then a vertical scan of the left edge) appears when text lacks formatting, and is a sign of poor structure. Better structured pages produce the layer-cake pattern (scanning headings) or a commitment pattern (reading fully when motivated).

**Apply.**
- Descriptive headings and subheadings that make sense on their own.
- Put key words at the start of headings, bullets and links.
- Short paragraphs, meaningful bold for key terms, and lists where content is genuinely list-like.

**Audit question.** Could a user get the gist by reading only the headings and the first words of each line?

## 8. The fold and scroll depth
**Evidence** B (NN/g 2018 eyetracking. About 57% of viewing time was above the fold and about 74% within the first two screenfuls, down from 80% above the fold in 2010).

**What it says.** Users scroll, but attention drops sharply after the first screen.

**Apply.**
- Put the value proposition, the key visual and the primary action in the first screen.
- Avoid false bottoms (full-height heroes or horizontal lines that look like the end of the page). Let content peek below the fold.
- Order the rest by importance. Expect the long tail to get little attention.
- Repeat the primary CTA after major persuasive sections on long pages.

**Audit question.** Does the first screen answer what this is, who it's for and what to do next, and does something invite scrolling?

## 9. Left-side bias
**Evidence** B (NN/g eyetracking found most viewing time on the left half of pages for left-to-right languages).

**Apply.**
- Left-align body text and most content in LTR languages. Center alignment is fine for short headlines only.
- Put the most important navigation items and labels on the left. Mirror everything for right-to-left languages.

**Audit question.** Is the most important information where readers start (top left in LTR)?

## 10. Banner blindness
**Evidence** B (Benway 1998, NN/g eyetracking 2007 and 2018).

**What it says.** Users ignore anything that looks like an ad, including real content styled like one or placed where ads usually go.

**Apply.**
- Don't style important messages as banners with stock-photo backgrounds or place them in right rails.
- Integrate key announcements into the content flow with native styling.

**Audit question.** Does any important information look like an advertisement?

## 11. Von Restorff (isolation) effect
**Evidence** A for memory (von Restorff 1933). B for UI.

**What it says.** The item that differs from its surroundings is noticed and remembered.

**Apply.**
- Make the primary CTA the only element in its accent color.
- Highlight the recommended plan with a single distinct treatment.
- Use isolation sparingly. If everything is highlighted, nothing is.

**Accessibility.** Don't rely on color alone. Combine it with size, position, labels or icons.

**Audit question.** Is the one thing that should stand out the only thing that does?

## 12. Serial position effect
**Evidence** A for memory (primacy and recency). B for navigation and lists.

**What it says.** Items at the start and end of a list are remembered best.

**Apply.**
- Put the most important navigation items first and last.
- In feature lists and onboarding, lead with the strongest point and end on a strong one.

**Audit question.** Are the most important items at the start or end of lists and menus?

## 13. Fitts's law
**Evidence** A (Fitts 1954, extensively replicated in HCI).

**What it says.** Time to hit a target depends on its distance and size. Big, close targets are fast. Screen edges and corners act as infinitely deep targets on desktop.

**Apply.**
- Make primary actions large and place them near where the user's attention or cursor already is.
- Keep related actions close together and destructive actions away from frequent ones.
- On mobile, full-width primary buttons near the bottom for key flows.
- Make the whole card or row clickable, not just the text.

**Audit question.** Are frequent and important targets large and close, and are risky targets separated from them?

## 14. Touch target size and the thumb zone
**Evidence** Standards plus B. WCAG 2.2 Success Criterion 2.5.8 (AA) requires targets of at least 24 by 24 CSS pixels or adequate spacing. 2.5.5 (AAA) asks for 44 by 44. Apple's guidelines recommend 44 by 44 points and Material Design 48 by 48 dp. Hoober's 2013 observational study found many users hold phones one-handed and shift grip often.

**Apply.**
- Minimum 24 by 24 CSS pixels for all targets, 44 to 48 for primary and frequent touch targets, with at least 8 pixels between adjacent targets.
- Put primary mobile actions in easy reach (lower and middle of the screen). Put rarely used or destructive actions higher.
- Don't rely on edge-of-screen precision taps.

**Audit question.** Can every tap target be hit comfortably with a thumb, without hitting a neighbor?

## 15. Affordances and signifiers
**Evidence** B (Norman 1988 and 2013. NN/g found weak signifiers in flat designs make users hesitate and spend longer finding clickable elements).

**What it says.** Users need visible cues about what can be clicked, dragged, swiped or typed into.

**Apply.**
- Buttons look like buttons (shape, fill, or clear border). Links look like links (color plus underline in body text).
- Inputs look like inputs (visible border, adequate height).
- Hidden gestures (swipe to delete, long press) need a visible alternative.
- Use cursor changes, hover states and focus states.

**Audit question.** Can a user tell what is interactive without hovering or guessing?

## 16. Icons and labels
**Evidence** B (NN/g icon usability research. Few icons are universally understood, such as home, search, print and close).

**Apply.**
- Pair icons with text labels, especially in navigation.
- Use standard icons for standard meanings. Never reuse a familiar icon for a different meaning.
- The hamburger menu reduces discoverability of what's inside. Expose top destinations when space allows.

**Audit question.** Would a new user know what each icon does without a label?

## 17. Typography and readability
**Evidence** B for minimum sizes and contrast. C for exact line lengths (studies by Dyson and others are mixed, but 50 to 75 characters is a sound default).

**Apply.**
- Body text 16 px minimum on the web. Line height about 1.4 to 1.6 for body text.
- Line length about 50 to 75 characters for reading-heavy content.
- Two typefaces at most. Limit sizes to a defined scale.
- Avoid long passages in all caps, light weights at small sizes, and justified text on the web.
- Support text resizing to 200% without loss of content (WCAG 1.4.4).

**Audit question.** Is the body text comfortable to read on a phone at arm's length?

## 18. Color and contrast
**Evidence** Standards. WCAG 1.4.3 requires 4.5 to 1 contrast for normal text and 3 to 1 for large text. 1.4.11 requires 3 to 1 for UI components and graphics. D for fixed color-emotion claims ("red increases conversions").

**Apply.**
- Meet contrast minimums, including placeholder text, disabled-looking buttons that are actually enabled, and text on images.
- Use color semantically and consistently (one accent for primary actions, standard red, amber and green for status), always backed by text or icons.
- About 1 in 12 men and 1 in 200 women have color vision deficiency. Test in grayscale and with simulators.
- Provide a dark mode for products used for long sessions or at night, designed deliberately rather than auto-inverted.

**Audit question.** Does all text and every control meet contrast minimums, and does meaning survive in grayscale?

## 19. Motion and animation
**Evidence** B (NN/g recommends roughly 100 to 500 ms for UI animation. Vestibular disorders make some motion harmful).

**What it says.** Motion explains change (where something came from or went), gives feedback, and adds personality. Too much or too slow motion feels sluggish or distracting.

**Apply.**
- Microinteractions about 100 to 200 ms. Larger transitions about 200 to 400 ms. Rarely more than 500 ms.
- Ease-out for entering elements, ease-in for exiting, and avoid linear motion for UI.
- Animate to show causality (an item flying to the cart, a panel sliding from the button that opened it).
- Respect `prefers-reduced-motion`. Replace large movements and parallax with fades or nothing.
- Never animate in a way that delays the user's next action.

**Audit question.** Does every animation explain something or give feedback, and is it fast enough not to block the user?

## 20. Density and whitespace
**Evidence** C (practitioner consensus, context dependent).

**What it says.** Whitespace improves scanning and perceived quality for consumer products. Expert tools (trading, analytics, admin) benefit from higher density.

**Apply.**
- Generous spacing on marketing and consumer flows.
- Offer density controls (comfortable or compact) in data-heavy tools.
- Use an 8-point spacing scale for consistency.

**Audit question.** Is the density right for this user's expertise and task?

## 21. Change blindness and feedback location
**Evidence** A (Simons and Levin, inattentional and change blindness research).

**What it says.** People miss changes outside their focus of attention, even large ones.

**Apply.**
- Show feedback where the user is looking (next to the button they pressed, at the field they edited).
- Use motion or brief highlight to draw attention to changes elsewhere (cart count updating).
- Don't rely on a toast at the top of a long page to report an error at the bottom.

**Audit question.** After each action, does feedback appear where the user is already looking?

## 22. Imagery and faces
**Evidence** B to C (NN/g eyetracking shows users ignore generic stock photos and look at real, relevant images. Faces attract attention, and gaze direction can guide it).

**Apply.**
- Use real product images and real people over generic stock.
- Product images that show scale, detail and use in context (Baymard finds users want multiple images including in-scale and in-use shots).
- If a face appears, have it look toward the content or CTA.
- Write meaningful alt text for informative images and empty alt for decorative ones.

**Audit question.** Does every image inform, or is some of it decoration that users will skip?
