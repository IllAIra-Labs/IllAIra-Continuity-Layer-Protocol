# Changelog

What shipped, and when. This file covers the **IllAIra CLM clients** and the public site.
The protocol specification in this repository is versioned separately —
see [IllAIra_Markdown_Standard_v1.13.md](./IllAIra_Markdown_Standard_v1.13.md).

Dates and checksums for every Android build are published, and machine-readable, at
[`illaira.com/app/latest.json`](https://illaira.com/app/latest.json). If a line here and that
file ever disagree, **the manifest is right**: it is generated from the binary, not written by hand.

---

## Live today

| | |
|---|---|
| **CLM WebApp** | [illaira.com/webapp](https://illaira.com/webapp) — browser, no install |
| **App CLM (Android)** | [illaira.com/download](https://illaira.com/download) — beta `0.1.144`, sideload |
| **App CLM (Windows, Linux)** | [illaira.com/download](https://illaira.com/download#desktop) — beta `0.2.4`: Windows 10/11 installer or portable zip, Linux `.deb` or AppImage |
| **Bazar** | [illaira.com/bazar](https://illaira.com/bazar) — Base tier, Tier 2 and one module, free with an account |
| **Written guides** | EN · IT · FR · ES · DE, from [illaira.com](https://illaira.com) |

Not shipped, and not scheduled here: iOS, a native Mac build, Play Store, App Store, Microsoft Store, checkout.

---

## App CLM — Android beta

All builds are 64-bit (`arm64-v8a`, `x86_64`), Android 7.0+, distributed as a sideload APK.
Dates are the publication dates in the manifest (UTC).

**Android release notes are published in Italian** in the update manifest, which already-installed apps read;
this file summarises them in English. Between `0.1.20` (29 August) and `0.1.144` (4 October) there are
more than 100 builds; the machine-generated, per-build history is at
[illaira.com/app/latest.json](https://illaira.com/app/latest.json). Below, by theme, with the build each
thing arrived in.

### `0.1.70` → `0.1.144` — 10 September to 4 October 2026

**Chat with your AI, inside the app**
* `0.1.79` (16 Sep) — a Chat screen: talk to your AI with a model that runs on the phone (nothing you write leaves it), or with your own key. Two modes: plain Chat and *On my files*, which answers from the passages of your files that match and says which files it read. Conversations are not memory: they stay on the device, per profile, and you keep what matters with the MemoKen.
* `0.1.80` (17 Sep) — every conversation is also a `.md` file you can open, copy or delete.
* `0.1.82`–`0.1.89` (17–18 Sep) — on-phone models run on the phone's fast cores, say under each model which engine answers and roughly how many tokens per second to expect, and say so honestly when the weights don't fit in memory instead of closing the app.
* `0.1.100`–`0.1.103` (21 Sep) — **Projects** (instructions + sources for one job), **Specialists** (the same AI with only some modules on), *Instructions for all chats*, a readable layered system prompt («see the exact text the model receives»), a context meter before you send, *Recalled* or *Full* context, an *Effort* control.
* `0.1.107` (21 Sep) — optional **web search**: you choose the search engine, there is no default, and pages are read from your phone.
* `0.1.119`–`0.1.124` (25–27 Sep) — model sizes for the phone, each with a verdict for *this* phone; the engine tunes itself in about a minute after a download; **the Chat opens to everyone** in `0.1.122`.
* `0.1.140` (1 Oct) — two buttons under the chat box: *My IllAIra* (whether your profile joins the conversation — off, whole mind, or one Specialist) and *Conversation options*.
* `0.1.144` (4 Oct) — **Agents** (Advanced mode): prepares an agent harness for the AI you choose — install, configure, key, start. On the phone it runs in Termux. Your key never goes into a configuration file.

**Learning and finding your way**
* `0.1.91` (19 Sep) onward — the guided path was rewritten from scratch; there are now tutorial chapters for every mode, in Settings › Tutorial, with *resume where I was*.
* `0.1.109` (22 Sep) — the **energy sphere**: a living guide that is born at first launch and walks you through the tutorials; six colours from `0.1.125`.
* `0.1.116`–`0.1.117` (24 Sep) — **three modes**: Simplified, Intermediate, Advanced. Intermediate calls things by their real names, each with a line saying what it is.
* `0.1.125` (28 Sep) — eight looks for the whole app (Settings › General › Appearance), the original one included as *Classic*.
* `0.1.141`–`0.1.143` (2–3 Oct) — **Help** inside the app: ask the AI how to do something and it answers from the manual that ships inside the app, or search the manual yourself. The tutorial is complete.

**Memory**
* `0.1.72`–`0.1.76` (10–14 Sep) — *Memory precision* (by name · by similarity); the knowledge map settings became one section where you choose a depth, not a model. The map is called **Understanding** from `0.1.128`.
* `0.1.73`–`0.1.74` (12–13 Sep) — a log that talks about several topics can be filed in several places at once; the MemoKen warns you when you are about to file the same fact twice, and says why each destination is proposed.
* `0.1.96` (20 Sep) — a log copied from a chat app is accepted even when the app dropped the `######`.
* `0.1.130` (29 Sep) — **Deferred Neural Tracing is free**: take the module from the Bazar and a *Paste Trace* button appears in the Sphere Grid, with no developer switch.
* `0.1.78` (16 Sep) — an optional, opt-in cloud copy of the profiles you choose. It is off until you turn it on, profile by profile; the [Privacy page](https://illaira.com/privacy) says exactly what it does and what it doesn't.

**Models**
* `0.1.105`–`0.1.111` (21–23 Sep) — *Model info*: a radar comparing models on six axes, each the average of published benchmarks, with the source next to every number; compare up to four models; a missing figure is left out, never counted as zero.
* `0.1.120` (26 Sep) — the on-device models live together in Settings › Engines (Memory and Understanding), each with a verdict for this phone: recommended, compatible, or not recommended.

**MemoKen**
* `0.1.70` (10 Sep) — you choose the colours of the tile, face by face; turning the tile no longer opens anything by accident.

**Profiles and files**
* `0.1.93` (19 Sep) — rename a profile (the folder on the phone follows). `0.1.134` (30 Sep) — delete a profile from the list, asked twice.
* `0.1.134` (30 Sep) — **files are always saved whole.** When a save made a file shorter, on recent Android a tail of the old text could remain at the end. The file is now rewritten from the start; the copy of every save stays in the profile's `backups` folder, as always.
* `0.1.92` (19 Sep) — the update notice opens the download page, so you decide when the file downloads.
* `0.1.101` (21 Sep) — every module shows its version, and the Bazar says when you already have one («You have v1.5 · v1.7 available»).

### `0.1.20` — 29 August 2026
* Fixed the last case where an entry added from a node menu landed in the protected `[P1]` zone instead of the diary. It happened when opening the map of a diary in a profile with no reminder.
* How to spot entries that already ended up there: `###### LOG:` lines carrying a date and a title with no text under them. The file stays valid, but your AI does not read them as memory — move them into the diary.

### `0.1.19` — 29 August 2026
* Add an entry to a diary you already have: pick the module, the app writes the dated heading, you write or paste the text. Available from the home screen next to "New log", and from the map panel.
* Fixed "Add log" from the map writing into the protected `[P1]` zone instead of the diary.

### `0.1.18` — 26 August 2026
* Create a new log file from the map or the home screen; the app writes today's dated heading, you supply the title and the body.
* Accented characters inside a word no longer split the filename: *Réunion équipe* becomes `reunion_equipe`.

### `0.1.17` — 24 August 2026
* In the Sferografia, with Externals enabled, two buttons create a new external module — functional or mnemonic — without attaching it to a node.

### `0.1.16` — 20 August 2026
* Settings and Account: the back button no longer sits under the status bar clock.
* The language dropdown scrolls; the last language is no longer hidden behind the system buttons.
* First launch opens with three lines explaining what the app does, before asking for anything.

### `0.1.15` — 20 August 2026
* First launch walks you through choosing the workspace folder and prepares it, instead of only telling you to pick one.
* On a new profile, the app points to where the first reminder comes from.

### `0.1.14` — 18 August 2026
* Buttons at the bottom of a screen no longer sit under the system navigation bar.
* "Log out" is now "Log out of your account" — it used to read as "quit the app".

### `0.1.13` — 16 August 2026
* The app is called IllAIra CLM under its icon too.

### `0.1.12` — 16 August 2026
* The Sferografia settings panel scrolls on the first try.

### `0.1.11` — 16 August 2026
* No new features: internal changes to how panels open.

### `0.1.10` — 15 August 2026
* App icon background moved to the IllAIra palette.
* **Removed the `SYSTEM_ALERT_WINDOW` permission.** The app never used it, and it is one of the permissions that weighs most in Play Protect heuristics. ⚠️ It does not make Android's install warning disappear — that warning is about the source of the file.

### `0.1.9` — 15 August 2026
* Create a new file straight from the home screen.
* Password reset by email link, and password change from inside the app.
* **Delete your IllAIra account from the app.** Your `.md` files are not touched.
* The Privacy screen states that sync consent is recorded before any sync channel exists, and why.

### `0.1.8` — 14 August 2026
* In the Sferografia the view no longer jumps back to centre when you open or close the menu.
* New ⌖ button to re-centre the view when *you* want to.

### `0.1.7` — 14 August 2026
* The app icon is centred again; it was also too large, and the phone frame clipped its edges.

### `0.1.6` — 14 August 2026
* Scroll guide available in the natural-text view, not only in Markdown.
* Fixed the scroll guide losing the finger on very long files.

### `0.1.5` — 13 August 2026
⚠️ **Uninstall before installing this one.** The signing key changed here — from `0.1.5` onward builds are signed with the IllAIra Labs release key, so `0.1.5` will not install over `0.1.0`–`0.1.4` and Android refuses without explaining why. **Your files stay in the folder you chose.**
* Scroll guide in the editor: drag it, or tap where you want to land.
* Long files open at the top instead of the bottom.

### `0.1.4` — 13 August 2026
* "Check now" for updates from Settings.
* The text editor works with the keyboard open again.
* The Sferografia zooms much further in and out.

### `0.1.3` — 13 August 2026
* IllAIra colours across every screen; the system blue is gone.
* The app tells you when a newer version exists — at launch, at most once a day, switchable off in Settings. The Privacy screen states what it asks the site for: one file, and nothing of yours.

### `0.1.2` — 12 August 2026
* Bazar items are "added to your profile" instead of "downloaded" — that was always the gesture, the name was wrong.
* The Bazar separates what is already yours from the rest of the counter; tier 3 and up say where they come from.
* An empty profile points at the Bazar, where the first items are free.
* The Privacy screen states what the server actually knows about your account, and what never reaches it: what you write in your files.

---

## App CLM — Windows and Linux beta

Windows 10/11 64-bit (installer or portable zip) and Linux x86_64 (`.deb` or AppImage). Same App as on the
phone, on your computer: notes are plain Markdown files in a folder you choose, an AI model can run on the
computer itself (on the graphics card when there is one) or you use your own key, with search by meaning,
chat with your files with the sources shown, projects, PDF import, the MemoKen and the Sphere Grid. The
account is optional. Models are not in the download: you fetch them from inside the App, only if you want them.
Versions and SHA-256 fingerprints are on the [download page](https://illaira.com/download#desktop).

### `0.2.4` — 4 October 2026
* Agents (Advanced mode): installs and starts an agent harness with your own AI provider, from inside the App; your key stays out of every file.
* A larger on-computer model (about 6 GB) is now the big option.
* On Windows the App installs for all users in Program Files and needs the Microsoft Visual C++ Runtime (setup downloads it from Microsoft, or install it later from Settings › General).
* Signing out also removes the web search key from this computer.

### `0.2.3` — 4 October 2026 — security update
* Safer PDF import; the App refuses to start if its files have been tampered with, and blocks permissions it doesn't need.
* AI models are downloaded only from illaira.com and checked against fingerprints built into the App.
* Web search no longer reads addresses on your local network.

### `0.2.2` — 3 October 2026 — first public beta
* The App on the computer. Installer and portable zip for Windows, `.deb` and AppImage for Linux.

**Known limits, stated plainly:** the Windows installer is not signed (Windows will warn you); the Windows
build has been tested under Wine on Linux and **not yet on a real Windows PC**; there is no automatic update —
the App tells you a new version exists and you download it.

---

## Site and CLM WebApp

The site and the WebApp deploy continuously and are not version-numbered in public.
Current state, as of 5 October 2026:

* **[illaira.com](https://illaira.com)** — product site, twelve languages; English at the root, Italian at `/it`. `www.illaira.com` redirects to the apex.
* **[/webapp](https://illaira.com/webapp)** — the CLM in the browser: editor, Sphere Grid, profiles, Bazar, ZIP export, search by meaning, the three modes, tutorials, Help, Chat with your own key (or a model on your computer), Projects and Specialists, Understanding, Agents set-up steps, the energy sphere and the eight looks. MemoKen in the browser is an extension (capture only).
* **[/bazar](https://illaira.com/bazar)** — catalogue. Base tier, Tier 2 and the Deferred Neural Tracing module are free with an account. Tiers 3–5 are described and **not released**.
* **[/download](https://illaira.com/download)** — APK for Android; installer, zip, `.deb` and AppImage for Windows and Linux; each with its SHA-256 and install notes.
* **[/help](https://illaira.com/help)** — frequently asked questions and the whole manual, chapter by chapter.
* **[/news](https://illaira.com/news)** — what changed, in date order, for the App, the WebApp and the site.
* **[/app/latest.json](https://illaira.com/app/latest.json)** — the update manifest the Android app reads.
* **[/contatti](https://illaira.com/contatti)** — contact and beta reports.

**Feature parity is a rule, not an aspiration:** a function that appears in one client is expected in the
other in the same round, or the exception is written down. The exceptions that stand today are listed in
the [README](./README.md#where-it-runs-today).
