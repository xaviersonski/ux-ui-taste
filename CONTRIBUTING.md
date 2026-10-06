# Contributing to UX/UI Taste

Thank you for your interest in contributing to **UX/UI Taste**! This project aims to bridge the gap between rigorous cognitive science, ethical design, and real-world product engineering.

---

## Principles for Contributing

To preserve the integrity and utility of this library, all contributions must uphold these standards:

1. **Empirical Grounding**: Do not submit personal opinions or unverified guru heuristics as scientific fact. When proposing a principle, cite peer-reviewed research, meta-analyses, or scaled industry benchmarks (e.g., Baymard Institute, NN/g).
2. **Assign an Evidence Grade**:
   - **Grade A (Robust)**: Meta-analyses or multiple independent replications, including field experiments.
   - **Grade B (Solid but conditional)**: Replicated or backed by large-scale industry benchmarks, with known boundaries or modest effect sizes.
   - **Grade C (Promising but thin)**: Single lab study, small sample, or practitioner heuristic. Explicitly framed as a hypothesis to test.
   - **Grade D (Myth / Debunked)**: Documented failure to replicate or common misconception.
3. **Consistent Schema**: Every principle entry in `references/` must follow the 5-part structure:
   - **What it says**: Clear explanation of the underlying phenomenon.
   - **Evidence grade**: Letter grade with supporting citations or replication context.
   - **How to apply it**: Practical, concrete rules of thumb for screens and flows.
   - **Limits & boundary conditions**: When the principle breaks down or backfires.
   - **Audit question**: A yes/no check suitable for an audit checklist.
4. **Zero Dark Patterns**: We do not accept tactics designed to manipulate, deceive, trap, or confuse users against their best interests. Fair, honest alternatives are required.

---

## How to Contribute

### 1. Proposing a New Principle or Study
- Check existing modules in `references/` to make sure it doesn't already exist.
- Open an Issue using the **New Principle / Study Proposal** template with source links, methodology, and suggested evidence grade.

### 2. Updating Legal and Regulatory Notes
- Consumer protection regulations (such as FTC guidelines, the EU Digital Services Act, and the UK DMCC Act) evolve rapidly.
- PRs citing updated enforcement actions, statutory changes, or official guidance are welcomed in `references/07-ethics-dark-patterns-law.md`.

### 3. Improving Existing Guides
- Fix typos, clarify confusing explanations, or improve code and design snippets.
- Keep tone direct, calm, and objective. Avoid hyperbole or marketing jargon.

---

## Local Development & Verification

Before submitting a pull request:
1. Verify that all relative links in Markdown documents resolve correctly.
2. Ensure consistent LF line endings and no trailing whitespace.
3. Keep OS-specific files (`.DS_Store`, `._*`) out of git.

---

## Code of Conduct

Please review and adhere to our [Code of Conduct](CODE_OF_CONDUCT.md). We are committed to providing a welcoming, respectful, and harassment-free community for everyone.
