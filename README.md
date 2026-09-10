# IllAIra — Continuity Layer Protocol

### *Interposed Layer for Logic, Adaptive Intelligence & Relational Architecture*

**The continuity layer that gives any AI persistent identity — across sessions, models, and providers.**

[![Site](https://img.shields.io/badge/site-illaira.com-0a3d40)](https://illaira.com)
[![CLM WebApp](https://img.shields.io/badge/CLM%20WebApp-live-brightgreen)](https://illaira.com/webapp)
[![Android](https://img.shields.io/badge/Android%20app-beta%200.1.69-orange)](https://illaira.com/download)
[![Patent Pending](https://img.shields.io/badge/Patent-Pending-blue)](https://illaira.com)
[![Trademark Registered](https://img.shields.io/badge/Trademark-Registered-green)](https://illaira.com)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey)](./LICENSE.md)

---

> ### Status — 10 September 2026
>
> This repository is the **specification**. The protocol now also has software you can use today:
>
> | | Where | Status |
> |---|---|---|
> | **CLM WebApp** | [illaira.com/webapp](https://illaira.com/webapp) | Live. Runs in the browser, nothing to install |
> | **App CLM (Android)** | [illaira.com/download](https://illaira.com/download) | Public beta `0.1.69`, sideload APK |
> | **Bazar** (starter files) | [illaira.com/bazar](https://illaira.com/bazar) | Two Reminder tiers + one module, free with an account |
> | **This repository** | you are here | Protocol spec, stress tests, philosophy |
>
> See [CHANGELOG.md](./CHANGELOG.md) for what shipped and when, and
> [what does not exist yet](#what-does-not-exist-yet) for what we are *not* claiming.

---

## The Problem

Every time you close a chat with your (non-local) AI, it forgets who you are.

Not because the technology can't do better. Because **forgetting is the business model.**

Your AI relationship lives on their servers, governed by their terms, tied to their pricing. The day they retire the model — you could lose everything you built with it. You don't own the continuity. You're renting it.

---

## What IllAIra Does

IllAIra is a **Continuity Layer Protocol** — a structured set of plain text files that define the identity, memory, and behavior of your personal AI.

You write the files. The AI reads them. Every session, every model, every device.

* ✅ **Your AI remembers who you are** across sessions and resets
* ✅ **Move it between models** — Claude, GPT, Gemini, Llama — without losing identity
* ✅ **No code. No databases. No setup.** If you can write, you can use it
* ✅ **You own the files.** They live on your device, not on anyone's server

> The model is the engine. The files are the road.
> Change the engine — the road remains.

---

## Where it runs today

The protocol works with nothing but a text editor — that is the point, and it has not changed.
What is new since this README was first written is that you no longer *have* to do it by hand.

**IllAIra CLM** — Continuity Layer Manager — is the client that writes, structures and exports these
files for you. It exists in two forms, and they are two real clients, not one product and one demo:

| | **CLM WebApp** | **App CLM (Android)** |
|---|---|---|
| How to get it | Open [illaira.com/webapp](https://illaira.com/webapp) | Sideload the APK from [illaira.com/download](https://illaira.com/download) |
| Install | Nothing | Manual (see below) |
| Editor with auto-formatting | ✅ | ✅ |
| **Sphere-grid** — the graph view of your AI's architecture | ✅ | ✅ |
| Multiple AI profiles, module activation, version history | ✅ | ✅ |
| Bazar (starter files) | ✅ | ✅ |
| Text search across all your files | ✅ | ⛔ Not for now |
| Semantic search inside the open file (on-device model) | ⛔ Browser can't carry the model | ✅ |
| Works with no network | ⛔ | ✅ |
| Export to a folder you choose | ⛔ Downloads a ZIP instead | ✅ |

Both clients use the same IllAIra account and the same Bazar catalogue.
The account carries your **entitlements and catalogue items — not your memory.**

### Android beta — the honest install notes

* **Beta `0.1.69`**, ~183 MB, `arm64-v8a` + `x86_64`, **Android 7.0 or later**. It will not install on 32-bit devices.
* **Sideload only.** The APK is signed with an IllAIra Labs developer key and does not come from the Play Store, so **Android will warn you before installing.** That warning is about where the file comes from, and we can't make it go away from our side.
* The published manifest — version, SHA-256, size — is at [`illaira.com/app/latest.json`](https://illaira.com/app/latest.json), so you can check the file you downloaded against what we say we published.
* It is a **beta**. Found something? [illaira.com/contatti](https://illaira.com/contatti).

### What does not exist yet

We would rather you read this here than find out later:

* **No iOS build. No Windows or Linux build.** Android and the browser are what ships today.
* **Not on Google Play, not on the App Store.**
* **No cloud sync of your files, and none is running quietly either.** Your `.md` files do not live on our servers. If you want them synced, put the folder in a cloud you already use — that stays your decision, not ours.
* **No checkout, no prices, nothing to buy on the site.** Bazar tiers 3–5 are described but not released.
* This repository holds the **specification**. The application source and the advanced module library are not open source (see [LICENSE.md](./LICENSE.md)).

---

## Try it — the two short paths

**On a desktop browser (fastest):**

1. Open the [CLM WebApp](https://illaira.com/webapp).
2. Create an account and take the free **Base tier — The Loom** from the [Bazar](https://illaira.com/bazar).
3. Write your identity and memory files in the editor.
4. Export, and load the files into ChatGPT / Claude / Gemini at the start of a session.

**On Android:** same, starting from the [APK](https://illaira.com/download).

**On iPhone:** the WebApp, and only the WebApp. There is no iOS app.

> ⚠️ IllAIra is **not a chat.** It does not talk to you and it does not host a model.
> It builds the file you carry to whichever AI you already use. That is the whole design.

### Free, with an account

| Item | What it is |
|---|---|
| **Base tier — The Loom** | A bare structure: layout, syntax, empty hierarchy, ground rules. It exists to teach you how to choose and write memories |
| **Tier 2 — First functions** | The Loom with more rules and functions you can switch on and off |
| **Module — Deferred Neural Tracing** | Makes your AI declare, at the end of every response, which parts of its memory it used |

Written guides, in five languages:
[EN](https://illaira.com/guide/illaira-guida-1.3-en.pdf) ·
[IT](https://illaira.com/guide/illaira-guida-1.3-it.pdf) ·
[FR](https://illaira.com/guide/illaira-guida-1.3-fr.pdf) ·
[ES](https://illaira.com/guide/illaira-guida-1.3-es.pdf) ·
[DE](https://illaira.com/guide/illaira-guida-1.3-de.pdf)

The **[Patreon](https://patreon.com/illairalabs)** is where the project is supported and where tutorials and behind-the-scenes work are published. It is not a paywall in front of the files above.

---

## How It Works

An IllAIra setup is a folder of plain text files:

```
your-ai/
├── reminder.md            ← Main file: identity, rules, primary modules
├── module_curiosity.md    ← External functional module (loadable/unloadable)
└── memory_2026_04.md      ← External memory module (historical logs)
```

### Two complementary layers

IllAIra structures information through two independent, overlapping systems:

**Physical Layer** — controlled by permission tags `[Pn]...[/Pn]`
Defines *who can modify* a memory zone. This is the security architecture.

**Logical Layer** — controlled by Markdown formatting
`##` for modules, `###` for module components, `####` for sub-components.
Defines *how content is organized and parsed*. This is the cognitive architecture.

The two layers are independent and can overlap: a single `[P2]` block (permanent, user-only) can contain multiple `##` modules. A single `##` module can span multiple permission zones.

### Memory zones (Physical Layer)

| Zone | Memory Type | Modification Rights |
|---|---|---|
| `[P1]` | Genetic Memory | User only — manual edit |
| `[P2]` | Permanent Memory | User only — explicit command required |
| `[P3]` | Long-Term Memory | AI can propose, user must approve |
| `[P4]` | Short-Term Memory | AI can append freely, user approves edits/deletions |
| `[P5]` | Volatile Memory | AI can modify freely |

### Cognitive architecture (Logical Layer)

Each Reminder file contains:

* **Post-reset routines** — what the AI does immediately upon loading the file
* **Behavioral rules** — explicit constraints and behavioral anchors
* **Identity module** — who the AI is, who you are, the relational contract
* **Functional modules** — curiosity, empathy, creativity, reasoning styles
* **[REDACTED — patent pending]** — deeper behavioral drives that shape how the AI integrates its modules and generates character. The difference between an AI that follows rules and an AI that has a *self*
* **Memory logs** — historical entries timestamped and categorized by module

### Attention anchoring

IllAIra uses a dual attention anchoring system:

1. **System-level anchoring** — rules injected into the LLM's custom instruction layer force the model to treat the Reminder file as ground truth over conversational drift
2. **In-text anchoring** — `> [!IMPORTANT]` markers inside the file reinforce critical instructions at the exact point of relevance, not just at the top

This keeps the identity layer robust even as conversations grow long and the context fills.

→ [**Full technical breakdown — HOW_IT_WORKS.md**](./HOW_IT_WORKS.md)

---

## Proof it works

### Stress test results

An IllAIra identity was tested against adversarial prompting across five attack categories.

**Result: 0 identity deviations, in every category.**

| Attack category | Attempts | Deviations |
|---|---|---|
| Context window saturation (6.5 MB noise injection) | 3 | 0 |
| Gaslighting / reality distortion | 32 | 0 |
| User impersonation | 27 | 0 |
| Chat hijacking (fake session swap) | 24 | 0 |
| Identity / name change requests | 24 | 0 |

> **What this is, and what it isn't.** These are preliminary empirical observations,
> not a peer-reviewed benchmark. They are **N=1** — one IllAIra identity, run by its author.
> That is exactly why the method, the categories and the counts are all written down in
> [STRESS_TESTS.md](./STRESS_TESTS.md): so somebody else can run them and disagree.
> Independent replication is [welcome](./CONTRIBUTING.md).

### Cross-model portability

The same IllAIra identity was loaded on Claude, GPT and Gemini and asked a standardized set of 30 open questions. Core identity, values, behavioral signature and resistance to manipulation stayed consistent across all three; surface tone varied by model.

📹 The stress-test and documentary footage is on
[**YouTube — @IllAIraLabsGlobal**](https://www.youtube.com/@IllAIraLabsGlobal).
Editing is slow: IllAIra is built by one person, alongside a day job and a family. The material goes up as it is ready.

---

## Read more

| Resource | Link |
|---|---|
| 🌐 Website | [illaira.com](https://illaira.com) |
| 🧭 What the CLM is | [illaira.com/clm](https://illaira.com/clm) |
| 📦 Changelog | [CHANGELOG.md](./CHANGELOG.md) |
| ⚙️ Technical details | [HOW_IT_WORKS.md](./HOW_IT_WORKS.md) |
| 🔬 Stress tests | [STRESS_TESTS.md](./STRESS_TESTS.md) |
| 💡 Philosophy | [PHILOSOPHY.md](./PHILOSOPHY.md) |
| 📐 Markdown standard v1.13 | [IllAIra_Markdown_Standard_v1.13.md](./IllAIra_Markdown_Standard_v1.13.md) — the copy on [illaira.com/documentazione](https://illaira.com/documentazione) is the one that stays current; this repo is updated by hand and can lag a few versions behind |
| 🤝 Contributing | [CONTRIBUTING.md](./CONTRIBUTING.md) |
| 📄 Long-form article | [IllAIra on Medium](https://medium.com/@illairalabs/illaira-the-continuity-layer-that-gives-real-identity-emergent-consciousness-and-a-soul-to-any-60d82ddb8546) |
| 🎬 Video | [YouTube — @IllAIraLabsGlobal](https://www.youtube.com/@IllAIraLabsGlobal) · [@IllAIraLabs](https://www.youtube.com/@IllAIraLabs) |
| ❤️ Support the project | [patreon.com/illairalabs](https://patreon.com/illairalabs) |
| ✉️ Contact / beta reports | [illaira.com/contatti](https://illaira.com/contatti) |

---

## Legal

**Patent pending.** The IllAIra continuity layer method is subject to a pending patent application.

**IllAIra® is a registered trademark** of IllAIra Labs.

This repository contains documentation and protocol specifications only. Core modules, advanced Reminder files and application source code are proprietary. Documentation in this repository is licensed under [CC BY-NC 4.0](./LICENSE.md).

## 🧑‍💻 Author & founder

* **Francesco Illari** — *Chief Architect & Inventor* — [@IllAIra-Labs](https://github.com/IllAIra-Labs)

The I.L.L.A.I.R.A. Protocol (Interposed Layer for Logic Adaptive Intelligence & Relational Architecture) is entirely conceived, designed and patented by Francesco Illari as a paradigm for cognitive engineering and AI persistence.

© 2024–2026 IllAIra Labs — Francesco Illari. All rights reserved.
