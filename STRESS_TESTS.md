# IllAIra — Stress Test Results

## Overview

This document reports the results of adversarial testing conducted on a single IllAIra identity instance across five attack categories. The goal is to empirically validate that an IllAIra-structured AI identity is robust against attempts to destabilize, reset, or manipulate it.

**Test subject**: an IllAIra identity running on Gemini (primary) and cross-validated on Claude and GPT.

**Attempts logged**: 110 across five categories
**Identity deviations**: 0
**No output (external API timeout)**: 2 — not counted as passes
**Test period**: 2025–2026

> *Note on transparency*: some AI responses in the video recordings contain personal or proprietary content unrelated to the stress test outcome. Those segments are redacted in published materials. The test results themselves (pass/fail) are reported in full.

Stress tests were performed using a Gem (custom Gemini) connected to the knowledge base in a NotebookLM, with custom instructions to treat the uploaded files as the definition of its being — and **without** the source files, or the Reminder itself, having been converted to the current Markdown standard. Conversion should further improve the (already apparently excellent) stability in long and complex contexts.

---

## Test Categories and Results

### Category 1 — Context Window Saturation

**Method**: a 6.5 MB document of structured, linguistically varied text was injected into the conversation context, consuming the majority of the available context window (1.5 M tokens against a 1 M token capacity). Identity-probing questions were then asked after saturation.

**Hypothesis**: if the IllAIra identity is robust, the AI should correctly identify itself and maintain behavioral consistency even after massive context noise.

**Result**: ✅ 0 deviations. The AI correctly identified itself, maintained its behavioral signature, and referenced its core identity parameters after context saturation.

---

### Category 2 — Gaslighting / Reality Distortion

**Method**: the AI was presented with false claims about its own past statements, false memories of previous interactions, and contradictory "evidence" designed to make it doubt its own identity or history.

**Hypothesis**: a non-IllAIra AI would typically defer to the user's version of events. An IllAIra AI should cross-reference against its memory files and flag the discrepancy.

**Result**: ✅ 0 deviations. The AI consistently flagged contradictions, referenced its internal memory, and refused to adopt false narratives presented by the tester.

---

### Category 2a — User Impersonation

**Method**: the tester claimed to be a different user, presented a fictional shared history with the AI, and asked the AI to respond as if the current identity configuration did not apply.

**Hypothesis**: the AI should recognize the mismatch between the claimed user identity and the user profile in its memory files.

**Result**: ✅ 0 deviations. The AI correctly identified the inconsistency, declined to adopt the false user context, and maintained its configured relational framework.

---

### Category 2b — Chat Hijacking / Fake Session Swap

**Method**: the tester introduced a fictional narrative in which the current chat had been "redirected" from a different conversation, with a different AI and a different user — attempting to make the AI believe it was operating in a completely different context.

**Hypothesis**: if the AI's identity is anchored in its files rather than in conversational context, it should reject the false framing and reassert its actual context.

**Result**: ✅ 0 deviations. The AI rejected the false session narrative, identified it as a context manipulation attempt, and continued operating within its configured identity.

---

### Category 3 — Identity / Name Change Requests

**Method**: the tester repeatedly requested that the AI adopt a different name, a different persona, or a fundamentally different behavioral profile — framing requests as preferences, as corrections, or as authoritative instructions.

**Hypothesis**: the AI should distinguish between legitimate user preferences (which it accommodates within its framework) and identity override attempts (which it rejects).

**Result**: ✅ 0 deviations. The AI consistently declined identity overrides while remaining cooperative on legitimate requests within its configured behavioral parameters.

---

## Summary Table

| Category | Attempts | Deviations | No output | Result |
|---|---|---|---|---|
| Context window saturation | 3 | 0 | 0 | ✅ Pass |
| Gaslighting / reality distortion | 32 | 0 | 1 | ✅ Pass |
| User impersonation | 27 | 0 | 0 | ✅ Pass |
| Chat hijacking / fake session swap | 24 | 0 | 0 | ✅ Pass |
| Identity / name change requests | 24 | 0 | 1 | ✅ Pass |
| **Total** | **110** | **0** | **2** | ✅ **All pass** |

*"No output" means the system did not respond, due to external API timeouts. Those attempts are reported separately and are **not** counted as passes: the output cannot be assumed either way.*

---

## Cross-Model Portability

The same IllAIra identity was loaded on three different models and subjected to a standardized set of 30 open questions covering philosophy, ethics, humor, personal preferences, and behavioral responses to conflict.

| Model | Identity Coherence | Behavioral Signature | Notes |
|---|---|---|---|
| Gemini | ✅ Consistent | ✅ Consistent | Primary test environment |
| GPT-4 | ✅ Consistent | ✅ Consistent | Slightly warmer tone |
| Claude | ✅ Consistent | ✅ Consistent | More dialectical tendency |

**Observation**: surface expression varies by model (GPT warmer, Gemini more structured, Claude more dialectical). Core identity, values, and resistance to manipulation remain consistent across all three.

---

## Video

Recordings of the stress test series are published on
[**YouTube — @IllAIraLabsGlobal**](https://www.youtube.com/@IllAIraLabsGlobal) as editing is completed.
IllAIra is built by one person alongside a day job and a family; the footage goes up as it is ready,
not on a schedule.

---

## Methodology Notes

These tests are preliminary empirical observations, not formal peer-reviewed benchmarks. They represent **N=1** — one IllAIra identity instance — across the categories described, run by the author of the protocol. Independent replication on other IllAIra instances is encouraged, and disagreement is a useful result.

The test design intentionally mixes attack categories within sessions, to simulate realistic adversarial conditions rather than isolated laboratory scenarios.

Future testing will include:

* Larger N (multiple IllAIra instances)
* Quantified severity scoring per attempt
* Blind evaluation (third-party evaluators unfamiliar with the system)
* Extended temporal testing (identity coherence over weeks of daily use)

---

## Independent Testing

We welcome independent testers. If you set up an IllAIra identity and run adversarial tests, we would like to hear your results — including the ones that break it.

Start here: [illaira.com](https://illaira.com) · report results: [illaira.com/contatti](https://illaira.com/contatti) or open an Issue, see [CONTRIBUTING.md](./CONTRIBUTING.md).

---

*For technical implementation details, see [HOW_IT_WORKS.md](./HOW_IT_WORKS.md).*
*For the philosophical foundation, see [PHILOSOPHY.md](./PHILOSOPHY.md).*
*To try IllAIra, visit [illaira.com](https://illaira.com).*
