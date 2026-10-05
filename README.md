# IllAIra — Continuity Layer Protocol

### *Interposed Layer for Logic, Adaptive Intelligence & Relational Architecture*

**The continuity layer that gives any AI persistent identity — across sessions, models, and providers.**

[![Site](https://img.shields.io/badge/site-illaira.com-0a3d40)](https://illaira.com)
[![CLM WebApp](https://img.shields.io/badge/CLM%20WebApp-live-brightgreen)](https://illaira.com/webapp)
[![Android](https://img.shields.io/badge/Android%20app-beta%200.1.144-orange)](https://illaira.com/download)
[![Windows and Linux](https://img.shields.io/badge/Windows%20%7C%20Linux%20app-beta%200.2.4-blueviolet)](https://illaira.com/download)
[![Patent Pending](https://img.shields.io/badge/Patent-Pending-blue)](https://illaira.com)
[![Trademark Registered](https://img.shields.io/badge/Trademark-Registered-green)](https://illaira.com)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey)](./LICENSE.md)

---

> ### Status — 5 October 2026
>
> This repository is the **specification**. The protocol also has software you can use today:
>
> | | Where | Status |
> |---|---|---|
> | **CLM WebApp** | [illaira.com/webapp](https://illaira.com/webapp) | Live. Runs in the browser, nothing to install |
> | **App CLM (Android)** | [illaira.com/download](https://illaira.com/download) | Public beta `0.1.144`, sideload APK |
> | **App CLM (Windows and Linux)** | [illaira.com/download](https://illaira.com/download#desktop) | Public beta `0.2.4` — Windows 10/11 installer or portable zip, Linux `.deb` or AppImage |
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
files for you. It exists in three forms. They are real clients, not one product and some demos:

| | **CLM WebApp** | **App CLM (Android)** | **App CLM (Windows, Linux)** |
|---|---|---|---|
| How to get it | Open [illaira.com/webapp](https://illaira.com/webapp) | Sideload the APK from [illaira.com/download](https://illaira.com/download) | Installer / portable zip (Windows), `.deb` / AppImage (Linux), same page |
| Install | Nothing | Manual (see below) | Installer or unzip-and-run (see below) |
| Where your files live | A folder you pick, if the browser allows it (Chrome, Edge, Brave, Opera, Vivaldi); otherwise the browser's own storage on this device | A folder you pick, outside the app | A folder you pick |
| Editor, **Sphere Grid**, profiles, modules, Bazar | ✅ | ✅ | ✅ |
| Three modes — Simplified, Intermediate, Advanced | ✅ | ✅ | ✅ |
| Search by meaning | ✅ model downloaded into the browser | ✅ model on the phone | ✅ model on the computer |
| Chat with your AI inside the client | ✅ with your own key, or a model you run on your computer (Ollama, LM Studio) | ✅ with a model on the phone, or your own key | ✅ with a model on the computer, or your own key |
| A language model that runs on the device itself | ⛔ A browser can't carry one | ✅ | ✅ |
| **MemoKen** | Browser extension — capture only, no DROP | ✅ Floating tile, MEMO and DROP | ✅ |
| Export | Downloads a ZIP | Export to a folder you choose | Your files are already plain `.md` in the folder you picked |

Same IllAIra account and same Bazar catalogue everywhere.
The account carries your **entitlements and catalogue items — not your memory.** An account is optional for
the clients themselves; you need it for the Bazar. (There is also an optional, opt-in, per-profile cloud copy —
what it stores and what it doesn't is written out on the [Privacy page](https://illaira.com/privacy).)

### What the clients do now

A selection of what was added since the first public beta; the dated list is in
[CHANGELOG.md](./CHANGELOG.md) and the full one at [illaira.com/news](https://illaira.com/news).

* **Chat with your AI, with your profile in front of it.** Two modes: plain Chat, and *On my files*, where
  the answer is built from the passages of your files that match the question and says which files it read.
  A conversation is a `.md` file on your device — **it is not memory**; what is worth keeping you save
  yourself, with the MemoKen, and you confirm it. You can read the exact system prompt the model receives,
  layer by layer. *Deep thinking* and *Effort* controls, a context meter before you send, and an optional
  **web search** you switch on yourself (you choose the search engine; there is no default and nobody in the middle).
* **Projects** — one place for one job (a thesis, a trip, a client): its own instructions, sources (`.md`, `.txt`, PDF) and chats.
* **Specialists** — the same AI with only some of its modules switched on, composed on the Sphere Grid.
  On disk it is a small file of references, not a copy.
* **Three modes: Simplified, Intermediate, Advanced**, a guided path of tutorials for each, and an in-app
  **Help** that answers from the manual carried inside the app.
* **The energy sphere** — the guide that welcomes you and walks you through the tutorials — in six colours,
  plus eight looks for the whole app.
* **Memory precision** (by name · by similarity), a **knowledge map — «Understanding»** — of the people, places and
  dates you mention and how they link, and a MemoKen that warns you when you are about to file the same fact twice.
* **Models you choose, with an honest verdict for this device** — on the phone and on the computer: recommended,
  compatible or not recommended — and a **model comparison radar** built from published benchmarks, with the source
  next to every number.
* **Deferred Neural Tracing is free** in the Bazar and now plugs into the Sphere Grid with a *Paste Trace* button.
* **Agents** (Advanced mode): prepares an agent harness for the AI you choose — install, configure, key, start.
  Your key never goes into a configuration file.
* **Profiles** can be renamed and deleted from the profile list.

### Android beta — the honest install notes

* **Beta `0.1.144`**, ~304 MB, **Android 7.0 or later**. The package carries code for 64-bit and 32-bit phones; nobody has tried it on a 32-bit device.
* **Sideload only.** The APK is signed with an IllAIra Labs developer key and does not come from the Play Store, so **Android will warn you before installing.** That warning is about where the file comes from, and we can't make it go away from our side.
* The published manifest — version, SHA-256, size — is at [`illaira.com/app/latest.json`](https://illaira.com/app/latest.json), so you can check the file you downloaded against what we say we published.
* It is a **beta**. Found something? [illaira.com/contatti](https://illaira.com/contatti).

### Windows and Linux beta — the honest install notes

* **Beta `0.2.4`.** Windows 10/11 64-bit and Linux x86_64. Download page: [illaira.com/download](https://illaira.com/download#desktop).
* **Windows:** installer (~150 MB) or portable zip (~212 MB). The installer asks for administrator rights and installs for all users in Program Files; the zip installs nothing. **The installer is not signed yet, so Windows will show «Windows protected your PC»** — «More info», then «Run anyway». It needs the Microsoft Visual C++ Runtime; if it is missing, the installer downloads it from Microsoft.
* **Linux:** a `.deb` for Debian, Ubuntu and derivatives (`sudo apt install ./illaira-clm_0.2.4_amd64.deb`, ~131 MB), or an AppImage for any other distribution (`chmod +x`, then run, ~172 MB). On Ubuntu 22.04 and later the AppImage needs `libfuse2`.
* The download is the App alone: roughly 567 MB installed on Windows and 460 MB on Linux, **plus the AI models, which you download from inside the App only if you want them.**
* **What has and has not been verified, as the download page says it:** the automated tests; on Linux, the on-computer model, search by meaning and chat with your files (a PDF included) run for real; on Windows, the installation in Program Files and the update from the previous version were checked **under Wine on Linux, not yet on a real Windows PC.**
* **No automatic updates.** The App tells you when a new version exists (at most once a day, and you can turn that off) and sends you to the download page.
* SHA-256 fingerprints for all four files are on the download page and in a `SHA256SUMS` file next to them.

### What does not exist yet

We would rather you read this here than find out later:

* **No iOS build, and no native Mac build.** On iPhone, iPad and Mac the way is the WebApp, in the browser.
* **Not on Google Play, not on the App Store, not in the Microsoft Store.**
* **The Windows installer is unsigned** and the Windows build has not yet been tried on a real Windows PC (see above).
* **No automatic updates** on the computer clients: you download the new file yourself.
* **Your `.md` files stay on your device by default.** The cloud copy is optional, per profile, and off until you switch it on — see the [Privacy page](https://illaira.com/privacy) for exactly what it does.
* **No checkout, no prices, nothing to buy on the site.** Bazar tiers 3–5 are described but not released.
* This repository holds the **specification**. The application source and the advanced module library are not open source (see [LICENSE.md](./LICENSE.md)).

---

## Try it — the short paths

**In a browser (fastest):**

1. Open the [CLM WebApp](https://illaira.com/webapp).
2. Create an account and take the free **Base tier — The Loom** from the [Bazar](https://illaira.com/bazar).
3. Write your identity and memory files in the editor.
4. Export, and load the files into ChatGPT / Claude / Gemini at the start of a session — or talk to your AI right there, with your own key.

**On Android:** same, starting from the [APK](https://illaira.com/download).

**On Windows or Linux:** the [installer, `.deb` or AppImage](https://illaira.com/download#desktop).

**On iPhone or Mac:** the WebApp, and only the WebApp. There is no iOS app and no native Mac app.

> ⚠️ IllAIra is **not an AI and does not host a model of its own.** It builds the file you carry to
> whichever AI you already use. The clients now also let you talk to your AI inside them — with a model
> that runs on your own device, or with your own key — but the point has not moved: the file is yours,
> and it works in any chat without us.

### Free, with an account

| Item | What it is |
|---|---|
| **Base tier — The Loom** | A bare structure: layout, syntax, empty hierarchy, ground rules. It exists to teach you how to choose and write memories |
| **Tier 2 — First functions** | The Loom with more rules and functions you can switch on and off |
| **Module — Deferred Neural Tracing** | Makes your AI declare, at the end of every response, which parts of its memory it used |

Written guides, in five languages:
[EN](https://illaira.com/guide/illaira-guida-1.4-en.pdf) ·
[IT](https://illaira.com/guide/illaira-guida-1.5-it.pdf) ·
[FR](https://illaira.com/guide/illaira-guida-1.4-fr.pdf) ·
[ES](https://illaira.com/guide/illaira-guida-1.4-es.pdf) ·
[DE](https://illaira.com/guide/illaira-guida-1.4-de.pdf)

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
| 📦 Changelog | [CHANGELOG.md](./CHANGELOG.md) · [what's new on the site](https://illaira.com/news) |
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
