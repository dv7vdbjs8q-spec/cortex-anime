# Cortex AI for iOS

**CortexAnime · OmegaTech × CortexAnime · iOS 27 or newer**

Cortex AI is the CortexAnime player for iPhone: the full Hungarian catalogue, subtitles,
downloads, and a built-in assistant — **Cortex Phantom** — that answers about series,
episodes, genres, scores, and even arithmetic, from our own brain. It speaks Hungarian;
the interface speaks English.

This repository is the **distribution point**. It holds no application source code —
only what you need to install the app and keep it updated.

---

## Install

### Way one — AltStore or SideStore (recommended)

Your phone signs the app with **your own Apple ID**, on your device. Nothing is sent to us,
and no certificate of ours is involved.

1. Install [AltStore](https://altstore.io) or [SideStore](https://sidestore.io) from their own sites.
2. Open the app, go to **Sources**, and add:

   ```
   https://cortanime.eu/api/cortexai/app/source.json
   ```

3. Open the **CortexAnime** source, tap **Cortex AI**, then **Install**.

A free Apple ID signs for seven days. AltStore refreshes it automatically while both devices
are on the same Wi-Fi. SideStore refreshes on the device itself.

### Way two — download the IPA and sign it yourself

If you already use a signer, take the file and sign it there:

- **Build:** [CortexAI-1.5.ipa](https://cortanime.eu/api/cortexai/app/ipa) — 4 323 198 bytes,
  `sha256 0c033fabc817de0ba9e95b45e0f13e242e03c531624be4d3dc76baa506b133d8`
- **Signer (third party):** [applejr.net signer](https://applejr.net/#signer)

Upload the IPA to the signer, sign it with your certificate, then install the signed result.
That step happens between you and the signer; we never see it.

### The install page

Everything above, in one place, formatted for a phone:

**https://cortanime.eu/api/cortexai/app/install**

---

## Requirements

| | |
|---|---|
| Device | iPhone (built for iPhone and iPad layouts) |
| System | **iOS 27.0** or newer |
| Size | about 4 MB |
| Account | none — the app needs no sign-up |
| Computer | not required for AltStore / SideStore |

If an install fails, remove a previous copy first: two builds with the same bundle
identifier (`eu.cortex.ai`) cannot coexist on one device.

---

## What is in the app

- The CortexAnime catalogue with Hungarian titles, episodes, genres, scores and descriptions.
- Subtitles and downloads, with covers.
- **Cortex Phantom** — the assistant. Catalogue questions, episode counts, genres, scores,
  dates, units and arithmetic are answered instantly by our own brain layer, without a
  provider in between. Open-ended conversation runs on our own model as it gets stronger,
  with a fallback while it learns.
- Memory: what you tell it stays with the conversation across restarts, and you can delete
  any note from Settings.
- No trackers, no advertising identifiers, no account.
- **Settings → Get Cortex AI** inside the app shows this same install information, with a
  copy button for the source address and a share link for the install page.

---

## What is not here, on purpose

- **No application source code.** The app is proprietary and is not open source. This
  repository, the build, and the install page are the whole distribution.
- **No certificates or signing keys.** Nothing that could sign an app for someone else is
  published here, and we do not hand out certificates.
- **No subtitle files.** Our Hungarian subtitles are our own work and stay on our servers.

---

## Versions

| Version | Date | Notes |
|---|---|---|
| 1.5 | 2026-11-01 | Settings → **Get Cortex AI**: the install screen now lives inside the app |
| 1.4 | 2026-11-01 | Cortex Phantom answers from the brain layer first; faster chat, better memory |
| 1.3 | 2026-10-31 | Memory across restarts |
| 1.0 | 2026-10-27 | First public build |

The version served by the AltStore source is always the latest build.

---

## Support

- Site: [cortanime.eu](https://cortanime.eu)
- Install problems: check the requirements above, remove the previous build, and try again.
  A failed signature is almost always an expired certificate or a full seven-day free-account
  limit — refresh in AltStore and retry.

---

<sub>Cortex AI, Cortex Phantom, CortexAnime and OmegaTech are names of this project.
Apple, iPhone, iOS and AltStore are trademarks of their respective owners. This project is
not affiliated with Apple Inc.</sub>
