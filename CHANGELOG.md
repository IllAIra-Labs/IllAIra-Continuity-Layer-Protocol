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
| **App CLM (Android)** | [illaira.com/download](https://illaira.com/download) — beta `0.1.69`, sideload |
| **Bazar** | [illaira.com/bazar](https://illaira.com/bazar) — Base tier, Tier 2 and one module, free with an account |
| **Written guides** | EN · IT · FR · ES · DE, from [illaira.com](https://illaira.com) |

Not shipped, and not scheduled here: iOS, Windows, Linux, Play Store, App Store, cloud sync, checkout.

---

## App CLM — Android beta

All builds are 64-bit (`arm64-v8a`, `x86_64`), Android 7.0+, distributed as a sideload APK.
Dates are the publication dates in the manifest (UTC).

**Between `0.1.20` (29 August) and today, the app moved to `0.1.69` (9 September)** — see
[illaira.com/app/latest.json](https://illaira.com/app/latest.json) for the full, machine-generated
history in the meantime. The per-version notes below resume once the site's own user-facing changelog
is live, so this file stays a record of what actually shipped rather than a guess at it.

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

## Site and CLM WebApp

The site and the WebApp deploy continuously and are not version-numbered in public.
Current state, as of 29 August 2026:

* **[illaira.com](https://illaira.com)** — product site, five languages. `www.illaira.com` redirects to the apex.
* **[/webapp](https://illaira.com/webapp)** — the CLM in the browser: editor, Sferografia, profiles, Bazar, ZIP export.
* **[/bazar](https://illaira.com/bazar)** — catalogue. Base tier, Tier 2 and the Deferred Neural Tracing module are free with an account. Tiers 3–5 are described and **not released**.
* **[/download](https://illaira.com/download)** — APK, with the published SHA-256, size and install notes.
* **[/app/latest.json](https://illaira.com/app/latest.json)** — the update manifest the Android app reads.
* **[/contatti](https://illaira.com/contatti)** — contact and beta reports.

**Feature parity is a rule, not an aspiration:** a function that appears in one client is expected in the
other in the same round, or the exception is written down. The exceptions that stand today are listed in
the [README](./README.md#where-it-runs-today).
