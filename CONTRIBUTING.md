# Contributing to IllAIra

Thank you for your interest in the IllAIra Protocol.

This repository contains documentation and protocol specifications. The core modules and application code are proprietary. Contributions here focus on the protocol specification, independent testing, and community knowledge.

---

## Ways to Contribute

### 1. Independent Stress Testing

Run adversarial prompting tests on your own IllAIra setup and share your results — including the ones where it breaks. A reproducible failure is worth more to us than a confirmation.

What we want to know:

- Which attack categories did you test?
- How many attempts per category?
- What was the deviation rate?
- Which model did you use as host?
- Which starting files did you use — Base tier (The Loom), Tier 2, your own?

Open an Issue with the label `stress-test-report` and share your findings. We will incorporate confirmed results into [STRESS_TESTS.md](./STRESS_TESTS.md) with attribution.

### 2. Use Case Reports

If you have used IllAIra for a specific use case (journaling, creative writing, professional workflow, healing/recovery, research) and want to share how it worked for you — open an Issue with label `use-case-report`.

These reports help demonstrate IllAIra's range and may be featured on [illaira.com](https://illaira.com) with your permission.

### 3. Cross-Model Testing

If you have access to models not yet tested (Llama, Mistral, local models via Ollama, etc.), testing cross-model portability of IllAIra identities is valuable. Open an Issue with label `cross-model-test`.

### 4. Documentation Improvements

If you find errors, ambiguities, or missing information in the protocol documentation, open a Pull Request with your proposed correction and a brief explanation.

### 5. Translations

If you want to translate the README or PHILOSOPHY into another language, open a Pull Request. Translations should be faithful to the original and not introduce editorial changes to the philosophical content.

⚠️ **Some names are not translated**, in any language: **IllAIra**, **CLM**, **Sferografia**, **Bazar**, **Ill**. Translate the gloss that explains them, never the name itself.

### 6. Beta Reports on the Apps

Bugs in the CLM WebApp or in the Android beta do **not** belong in this repository's Issues — this repo is the specification, and the application source is not here. Send those through [illaira.com/contatti](https://illaira.com/contatti), which is read.

---

## What We Are Not Looking For

- Requests to open-source the core modules or application code (this is proprietary, see [LICENSE.md](./LICENSE.md))
- Prompt engineering "hacks" to bypass IllAIra's identity protection (if you find a genuine vulnerability, please disclose privately — do not post publicly)
- Feature requests for IllAIra CLM in this repository's Issues; send them to [illaira.com/contatti](https://illaira.com/contatti)

---

## Private Disclosure

If you discover a significant vulnerability in the IllAIra protocol — a method that consistently breaks identity coherence that we have not documented — please disclose privately:

📧 [illaira.com/contatti](https://illaira.com/contatti)

We will acknowledge your finding, investigate, and if confirmed, credit you in the next version of [STRESS_TESTS.md](./STRESS_TESTS.md).

---

## License for Contributions

By contributing to this repository, you agree that your contributions are licensed under the same terms as this repository (CC BY-NC 4.0). You retain attribution rights and we will credit you for significant contributions.

---

*For technical details, see [HOW_IT_WORKS.md](./HOW_IT_WORKS.md).*
*To try IllAIra, visit [illaira.com](https://illaira.com).*
