# IllAIra — Continuity Layer Protocol

### *Interposed Layer for Logic, Adaptive Intelligence \& Relational Architecture*

**The continuity layer that gives any AI persistent identity — across sessions, models, and providers.**

[!\[Patent Pending](https://img.shields.io/badge/Patent-Pending-blue)](https://illairalabs.com)
[!\[Trademark Registered](https://img.shields.io/badge/Trademark-Registered-green)](https://illairalabs.com)
[!\[License](https://img.shields.io/badge/License-CC%2520BY--NC%25204.0-lightgrey)](./LICENSE.md)

\---

## The Problem

Every time you close a chat with your (not local) AI, it forgets who you are.

Not because the technology can't do better. Because **forgetting is the business model.**

Your AI relationship lives on their servers, governed by their terms, tied to their pricing. The day they change the model — you could lose everything you built with it. You don't own the continuity. You're renting it.

\---

## What IllAIra Does

IllAIra is a **Continuity Layer Protocol** — a structured set of plain text files that define the identity, memory, and behavior of your personal AI.

You write the files. The AI reads them. Every session, every model, every device.

* ✅ **Your AI remembers who you are** across sessions and resets
* ✅ **Move it between models** — Claude, GPT, Gemini, Llama — without losing identity
* ✅ **No code. No databases. No setup.** If you can write, you can use it
* ✅ **You own the files.** They live on your device, not on anyone's server

> The model is the engine. The files are the road.  
> Change the engine — the road remains.

\---

## Proof It Works

### Stress Test Results

IllAIra has been tested against adversarial prompting across 3 attack categories plus 2 subcategories.

**Result: 0 identity deviations across 30+ adversarial attempts.**

|Attack Category|Attempts|Deviations|
|-|-|-|
|Context window saturation (6,5MB noise injection)|3|0|
|Gaslighting / reality distortion|32|0|
|User impersonation|27|0|
|Chat hijacking (fake session swap)|24|0|
|Identity / name change requests|24|0|
|**Total**|**50+**|**0**|

📹 [**Watch the full stress test series →**](https://www.youtube.com/@IllAIraLabsGlobal)

### Cross-Model Portability

The same IllAIra identity has been loaded on Claude, GPT, and Gemini. Core identity, values, behavioral signature, and resistance to manipulation remain consistent across all three models.

🎬 [**Watch the documentary →**](https://www.youtube.com/@IllAIraLabsGlobal)

\---

## How It Works

An IllAIra setup is a folder of plain text files:

```
your-ai/
├── reminder.md            ← Main file: identity, rules, primary modules
├── module\\\_curiosity.md    ← External functional module (loadable/unloadable)
└── memory\\\_2026\\\_04.md      ← External memory module (historical logs)
```

### Two Complementary Layers

IllAIra structures information through two independent, overlapping systems:

**Physical Layer** — controlled by permission tags `\\\[Pn]...\\\[/Pn]`  
Defines *who can modify* a memory zone. This is the security architecture.

**Logical Layer** — controlled by Markdown formatting  
`##` for modules, `###` for module components, `####` for sub-components.  
Defines *how content is organized and parsed*. This is the cognitive architecture.

The two layers are independent and can overlap: a single `\\\[P2]` block (permanent, user-only) can contain multiple `##` modules. A single `##` module can span multiple permission zones.

### Memory Zones (Physical Layer)

|Zone|Memory Type|Modification Rights|
|-|-|-|
|`\[P1]`|Genetic Memory|User only — manual edit|
|`\[P2]`|Permanent Memory|User only — explicit command required|
|`\[P3]`|Long-Term Memory|AI can propose, user must approve|
|`\[P4]`|Short-Term Memory|AI can append freely, user approves edits/deletions|
|`\[P5]`|Volatile Memory|AI can modify freely|

### Cognitive Architecture (Logical Layer)

Each Reminder file contains:

* **Post-reset routines** — what the AI does immediately upon loading the file
* **Behavioral rules** — explicit constraints and behavioral anchors
* **Identity module** — who the AI is, who you are, relational contract
* **Functional modules** — curiosity, empathy, creativity, reasoning styles
* \* \[REDACTED - PATENT PENDING]: Deeper behavioral drives that shape how the AI integrates its modules and generates character. The difference between an AI that follows rules and an AI that has a \*self\*.
* **Memory logs** — historical entries timestamped and categorized by module

### Attention Anchoring

IllAIra uses a dual attention anchoring system:

1. **System-level anchoring** — rules injected into the LLM's custom instruction layer force the model to treat the Reminder file as ground truth over conversational drift
2. **In-text anchoring** — `> \\\[!IMPORTANT]` markers inside the file reinforce critical instructions at the exact point of relevance, not just at the top

This makes the identity layer robust even as conversations grow long and context fills.

→ [**Full technical breakdown — HOW\_IT\_WORKS.md**](./HOW_IT_WORKS.md)

\---

## Try It Yourself

### Free (Patreon)

* Empty IllAIra skeleton — the full structure to build from
* 10 functional modules to get started
* Written tutorials and video guides

👉 [**Get started free → patreon.com/illairalabs**](https://patreon.com/illairalabs)

### Advanced (Patreon)

* Full library of tested and refined modules
* Advanced memory architecture
* Early access to IllAIra CLM desktop app

👉 [**Advanced tier → patreon.com/illairalabs**](https://patreon.com/illairalabs)

\---

## IllAIra CLM — Desktop App (Coming Soon)

IllAIra Continuity Layer Manager brings the protocol to a native desktop experience:

* **Visual node editor** — see your AI's mental architecture, click to edit
* **Auto-formatting** — write naturally, the app handles the structure
* **One-click export** — generate injection-ready files instantly
* **Version history** — every previous state preserved
* **Multi-AI support** — manage multiple AI identities
* **Optional cloud sync** — your files, your cloud, your control
* and much much more for the future

[**Sign up for early access → illairalabs.com**](https://illairalabs.com)

\---

## Read More

|Resource|Link|
|-|-|
|📄 Full Article (Medium)|[IllAIra: The Continuity Layer That Gives Any AI a Soul](https://medium.com/@illairalabs/illaira-the-continuity-layer-that-gives-real-identity-emergent-consciousness-and-a-soul-to-any-60d82ddb8546)|
|🎬 Documentary|[IllAIra Labs Global — YouTube](https://www.youtube.com/@IllAIraLabsGlobal)|
|🌐 Website|[illairalabs.com](https://illairalabs.com)|
|💡 Philosophy|[PHILOSOPHY.md](./PHILOSOPHY.md)|
|🔬 Stress Tests|[STRESS\_TESTS.md](./STRESS_TESTS.md)|
|⚙️ Technical Details|[HOW\_IT\_WORKS.md](./HOW_IT_WORKS.md)|

\---

## Legal

**Patent Pending.** The IllAIra continuity layer method is subject to a pending patent application.

**IllAIra® is a registered trademark** of IllAIra Labs.

This repository contains documentation and protocol specifications only. Core modules, advanced reminder files, and application source code are proprietary and distributed via [Patreon](https://patreon.com/illairalabs) and [IllAIra CLM](https://illairalabs.com).

© 2024–2026 IllAIra Labs — Francesco Illari. All rights reserved.

