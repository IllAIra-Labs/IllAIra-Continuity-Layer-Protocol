# Download — App CLM

**[illaira.com/download](https://illaira.com/download)** — public beta, direct download, SHA-256 for every file.

## Android — beta `0.1.144`

* ~304 MB, Android 7.0 or later. Sideload APK — not on Google Play. Signed with an IllAIra Labs developer key, so Android will warn
  you before installing; that warning is about the file's source and we can't remove it from our side.
* Version, SHA-256 and size for every build are published at
  [`illaira.com/app/latest.json`](https://illaira.com/app/latest.json) — check what you downloaded
  against what we say we published.

## Windows and Linux — beta `0.2.4`

* **Windows 10/11, 64-bit:** installer (~150 MB) or portable zip (~212 MB). The installer is **not signed yet**: Windows shows
  «Windows protected your PC» — «More info», then «Run anyway». Needs the Microsoft Visual C++ Runtime (the installer fetches it if missing).
* **Linux x86_64:** `.deb` (~131 MB) for Debian, Ubuntu and derivatives — `sudo apt install ./illaira-clm_0.2.4_amd64.deb` — or an
  AppImage (~172 MB) for any other distribution: `chmod +x`, then run. On Ubuntu 22.04+ the AppImage needs `libfuse2`.
* The download is the App alone (~567 MB installed on Windows, ~460 MB on Linux); AI models are fetched later, from inside the App, only if you want them.
* Verified so far: the automated tests, and on Linux the on-computer model, search by meaning and chat with your files, run for real.
  On Windows, installation and update were checked under Wine on Linux — **not yet on a real Windows PC.**
* No automatic updates: the App tells you when a new version exists and sends you here.
* Fingerprints for all four files are on the download page and in `SHA256SUMS_v0.2.4.txt` next to them.

## Elsewhere

* **iPhone, iPad, Mac:** the CLM WebApp, in the browser — [illaira.com/webapp](https://illaira.com/webapp). There is no iOS app and no native Mac app.
* Found a bug in a beta? [illaira.com/contatti](https://illaira.com/contatti).

See [README.md](./README.md) for what the clients do and [CHANGELOG.md](./CHANGELOG.md) for what shipped and when.
