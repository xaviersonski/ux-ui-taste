# 06. Feedback, Control, Forms and Interaction

The mechanics of interaction. Most conversion losses in forms, checkout and settings live here.

## Contents
1. Nielsen's ten usability heuristics
2. Visibility of system status
3. User control and freedom
4. Error prevention
5. Postel's law (be liberal in what you accept)
6. Inline validation
7. Form design essentials
8. Checkout design essentials
9. Account creation and login
10. Multi-step vs single-page flows
11. Navigation and wayfinding
12. Search
13. Filters and sorting
14. Empty states
15. Modals, popups and interruptions
16. Mobile interaction
17. Settings and preferences
18. Accessibility in interaction

---

## 1. Nielsen's ten usability heuristics
**Evidence** B (Nielsen 1994, still the most used evaluation framework).

1. Visibility of system status
2. Match between system and the real world
3. User control and freedom
4. Consistency and standards
5. Error prevention
6. Recognition rather than recall
7. Flexibility and efficiency of use
8. Aesthetic and minimalist design
9. Help users recognize, diagnose and recover from errors
10. Help and documentation

Use them as a fast first pass in audits. The rest of this library goes deeper on each.

**Severity scale (Nielsen).** 0 not a problem, 1 cosmetic, 2 minor, 3 major (fix soon), 4 catastrophe (fix before release). Rate by frequency, impact and persistence.

## 2. Visibility of system status
**Evidence** B.

**Apply.**
- Every action gets feedback within 100 ms (pressed state, spinner in the button, inline check).
- Disable submit buttons only while submitting, and show progress in the button. Avoid disabling buttons before the form is valid, since users can't tell what's missing. Let them press and show what to fix.
- Show save status for editors ("Saved", "Saving", "Offline, changes will sync").
- Show where users are (active nav item, breadcrumb, step indicator).

**Audit question.** After every action, does the user know it worked?

## 3. User control and freedom
**Evidence** B.

**Apply.**
- Clear exits (close, cancel, back) on every modal and flow step.
- The browser back button must work as users expect in single-page apps and multi-step flows, without losing data.
- Undo for reversible actions (see 05).
- Let users edit earlier steps from the review step without starting over.

**Audit question.** Can users always go back, cancel or undo without losing work?

## 4. Error prevention
**Evidence** B (Norman's slips and mistakes. Poka-yoke from manufacturing).

**Apply.**
- Constrain inputs to valid values (date pickers for dates, steppers for quantities, dropdowns only for short known lists).
- Use the right input types and `autocomplete` attributes so browsers and keyboards help.
- Good defaults reduce wrong choices.
- Warn before irreversible consequences, with specifics ("This will cancel 3 scheduled posts").
- Separate destructive buttons from frequent ones.

**Audit question.** What mistakes are likely here, and does the design make them hard to make?

## 5. Postel's law
**Evidence** B as a design principle (Postel 1980, applied to UX by practitioners and Baymard's input formatting research).

**What it says.** Be liberal in what you accept and conservative in what you send.

**Apply.**
- Accept phone numbers, card numbers and postcodes with or without spaces, dashes and brackets. Format them for the user instead of rejecting them.
- Accept dates in multiple formats or use clear separate fields.
- Trim stray whitespace. Make email matching case-insensitive.
- Never reject a field only because of formatting the system could fix.

**Audit question.** Does any field reject input that a computer could easily normalize?

## 6. Inline validation
**Evidence** B to C. Wroblewski and Etre 2009 tested 22 users on six form variants. Inline validation produced 22% higher success rates, 22% fewer errors, 31% higher satisfaction and 42% faster completion. The sample was small, but Baymard's checkout research supports the direction.

**Apply.**
- Validate when the user leaves a field (on blur), not on every keystroke, except where live feedback helps (password strength, username availability, character counts).
- Don't show errors on empty fields before the user has had a chance to fill them.
- Remove the error as soon as it's fixed.
- Positive confirmation (a check) is useful for fields with complex rules. Avoid it on simple fields where its absence could suggest a problem.
- On submit, move focus to the first error and summarize errors at the top for long forms.

**Audit question.** Do users learn about errors at the right moment, near the field, with a clear fix?

## 7. Form design essentials
**Evidence** B (Baymard, NN/g, Wroblewski's "Web Form Design", GOV.UK Design System research).

**Apply.**
- **Fewer fields.** Question every field. Can it be inferred, deferred or dropped? Baymard finds the average US checkout shows about 23.5 form elements by default, while an ideal flow can use 12 to 14 (7 to 8 actual fields).
- **Single column.** Users scan one column faster and skip fewer fields. Short related fields (city and postcode) can share a row.
- **Labels above fields,** always visible. Never use placeholder text as the only label (it vanishes, has low contrast, and is mistaken for prefilled data).
- **Mark optional fields** ("optional") when most fields are required, or mark required ones when most are optional. Be consistent.
- **Single name field** where your system allows, or clearly labeled first and last.
- **Field width hints expected length** (short for postcode, long for address).
- **Right keyboard on mobile** (`type="email"`, `type="tel"`, `inputmode="numeric"`).
- **Autocomplete attributes** on every standard field so browsers can autofill.
- **Address lookup** with a manual entry fallback.
- **Explain sensitive fields** ("Phone, only used if there's a problem with delivery").
- **Show password rules up front** and add a show-password toggle. Don't require password confirmation fields when a show toggle exists.
- **Button labels state the outcome** ("Create account", "Pay £42.00").

**Audit question.** Could this form be shorter, and is every field labeled, explained and easy to fill on a phone?

## 8. Checkout design essentials
**Evidence** B (Baymard's large-scale checkout research. Abandonment reasons from Baymard's US survey, excluding "just browsing", were extra costs too high 40%, delivery too slow 20%, didn't trust the site with card details 19%, forced account creation 18%, too long or complicated checkout 17%, errors or crashes 17%, unsatisfactory returns policy 13%, couldn't see total cost up front 12%, card declined 10%, not enough payment methods 9%).

**Apply.**
- Full cost, delivery date and returns policy visible before checkout begins.
- Guest checkout prominent. Offer account creation after the order.
- Express wallets (Apple Pay, Google Pay, PayPal, Shop Pay) at the top of checkout and in the cart.
- Order summary always visible (collapsible on mobile).
- Billing address defaults to "same as delivery".
- Promo code field present but not prominent (a large empty coupon field sends users off to search for codes). A collapsed link works well.
- Payment area visually reinforced for security (see 03).
- Handle declines gracefully with specific reasons and keep all entered data.
- Test the flow on slow mobile connections. Errors and crashes cost 17% of abandoners.

**Audit question.** Run Baymard's top reasons as a checklist. Which ones could a shopper hit here?

## 9. Account creation and login
**Evidence** B (Baymard. NN/g. Passwordless and passkey adoption data from FIDO Alliance and platform vendors).

**Apply.**
- Let users experience value before requiring an account where possible.
- Offer social login and passkeys alongside email. Magic links and one-time codes reduce password friction.
- Login and signup clearly distinguished, with an easy switch between them.
- When a returning user tries to sign up with an existing email, help them log in instead of showing a dead-end error.
- Password reset in as few steps as possible, with a link back to the original destination.
- Keep users logged in on personal devices, with a clear option to change.

**Audit question.** How many steps and decisions does it take a new user to get in, and a returning user to get back in?

## 10. Multi-step vs single-page flows
**Evidence** B. Baymard notes that complaints about "too long" checkouts aren't solved by cramming into one page, because perceived complexity matters more than the step count.

**Apply.**
- Group into a few logical steps with clear names. Each step should feel short.
- Start with the easiest step.
- Keep a persistent summary and allow editing previous steps.
- One-page flows suit short forms. Multi-step suits long or branching ones.

**Audit question.** Does each step feel short and logical, and can users see the whole path?

## 11. Navigation and wayfinding
**Evidence** B (NN/g. Baymard homepage and category research).

**Apply.**
- Navigation labels in user language, organized by user tasks and mental models (validate with card sorting and tree testing).
- Show where users are (highlighted nav, breadcrumbs for deep hierarchies, clear page titles).
- On desktop, visible top-level navigation. On mobile, bottom tabs for core destinations and a menu for the rest.
- Search prominent for content-heavy and catalog sites.
- Utility navigation (account, cart, help) in expected places.

**Audit question.** Can a new user find the three most important destinations without searching?

## 12. Search
**Evidence** B (Baymard e-commerce search research, NN/g).

**Apply.**
- Visible search field (not just an icon) on content-heavy sites, wide enough for typical queries.
- Autocomplete with suggestions, categories and popular queries. Highlight the completing part.
- Tolerate typos, synonyms, plurals and product codes.
- Never show a dead-end "no results" page. Offer spelling corrections, related categories, popular items and contact options.
- Keep the query visible and editable on the results page.

**Audit question.** Does search understand messy, real-world queries and always offer a way forward?

## 13. Filters and sorting
**Evidence** B (Baymard product list research).

**Apply.**
- Filters that match how users choose (use case, compatibility, size, price, rating), specific to each category.
- Show applied filters as removable chips, with result counts.
- Apply filters quickly without full page reloads, and keep the scroll position.
- On mobile, a full-screen filter panel with a clear "Show 42 results" button.
- Sort options users actually want (price, rating, newest, best selling).

**Audit question.** Can users narrow results the way they actually think about the products?

## 14. Empty states
**Evidence** B (practitioner consensus. Strong link to activation).

**What it says.** The first screen of a new product is usually empty. It's the onboarding.

**Apply.**
- Explain what will appear here and why it's useful.
- One clear action to fill it ("Create your first project"), or templates and sample data.
- Different messages for first-use empty, user-cleared empty (inbox zero, a moment to celebrate) and no-results empty (offer a way out).

**Audit question.** Does every empty state tell users what to do next?

## 15. Modals, popups and interruptions
**Evidence** B (NN/g found popups and interstitials are among the most hated web patterns. Google penalizes intrusive mobile interstitials in search).

**Apply.**
- Don't show popups on arrival. Wait for engagement or exit intent, and show at most once per session.
- Use modals only for focused tasks that need a decision before continuing.
- Every modal closes with Escape, a visible close button and a click outside (unless data would be lost).
- Trap focus inside modals and return it when they close.
- Use non-modal patterns (inline banners, toasts, side panels) for information that doesn't need a decision.

**Audit question.** Does any interruption appear before the user has gotten value, or block them without need?

## 16. Mobile interaction
**Evidence** B (Baymard mobile research. Platform guidelines).

**Apply.**
- Sticky primary CTA on long mobile product and checkout pages.
- Tap targets at least 44 to 48 px for primary actions.
- Don't rely on hover. Every hover reveal needs a tap equivalent.
- Hidden gestures need a visible alternative.
- Keep inputs visible above the keyboard and avoid layout jumps when it opens.
- Make phone numbers, addresses and emails tappable.
- Test with one hand, on a small screen, on a slow network.

**Audit question.** Can the key flow be completed one-handed on a small phone with a weak connection?

## 17. Settings and preferences
**Evidence** C (Jared Spool's observation that very few users change default settings is widely cited but informal. Consistent with default research in 03).

**Apply.**
- Get defaults right, since most users will never change them.
- Group settings by user goal, with search for large settings areas.
- Apply changes immediately where safe, with confirmation feedback.
- Explain consequences in plain language next to each setting.

**Audit question.** Would a user who never opens settings still get a good experience?

## 18. Accessibility in interaction
**Evidence** Standards and law. WCAG 2.2 is the current W3C standard. The European Accessibility Act has applied to covered products and services, including e-commerce, since 28 June 2025, with EN 301 549 (incorporating WCAG 2.1 AA) as the benchmark. US ADA litigation commonly references WCAG.

**Apply.**
- Everything works with a keyboard, in a logical order, with a clearly visible focus indicator that isn't hidden by sticky headers (WCAG 2.2 2.4.11).
- Semantic HTML first (real buttons, links, labels, headings). ARIA only to fill gaps.
- Every input has a programmatic label. Errors are announced and described in text.
- Don't require dragging without a single-pointer alternative (WCAG 2.2 2.5.7).
- Don't make users re-enter information already provided in the same process (WCAG 2.2 3.3.7).
- Authentication without cognitive tests like transcribing or memorizing, or with alternatives such as paste and password managers allowed (WCAG 2.2 3.3.8).
- Consistent help location across pages (WCAG 2.2 3.2.6).
- Test with a screen reader (VoiceOver, NVDA) on the key flow at least once.

**Audit question.** Can the core flow be completed by keyboard alone and with a screen reader?
