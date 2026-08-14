<h1 align="center">Isonimus</h1>

<p align="center">
  <strong>Full-stack engineer</strong> with a habit of building the tool that should exist:
  published TypeScript libraries, ESP32 security hardware, deterministic simulations and games.
</p>

<p align="center">
  <a href="https://www.npmjs.com/~isonimus"><img alt="npm" src="https://img.shields.io/badge/npm-published-CB3837?logo=npm&logoColor=white"></a>
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white">
  <img alt="Rust" src="https://img.shields.io/badge/Rust-000000?logo=rust&logoColor=white">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white">
  <img alt="C++" src="https://img.shields.io/badge/C++-00599C?logo=cplusplus&logoColor=white">
  <img alt="ESP32" src="https://img.shields.io/badge/ESP32-E7352C?logo=espressif&logoColor=white">
</p>

---

I like problems that force a clear architecture: a **determinism harness** that proves a
simulation runs the same from a seed every time, a **zero-dependency** library that has to earn
every byte, a security probe that has to be right about the radio in front of it. A lot of my
work carries architecture decision records and a written definition of done, because the interesting
part is usually the invariant, not the feature.

The range below is wide on purpose (browser instrumentation, embedded RF tooling, agent-based
simulation, ML, games), but the engineering underneath it is the same.

---

## Tindalabs: browser trust & observability

A composable stack of published, typed, mostly zero-runtime-dependency libraries for knowing
what is happening in a browser session and whether to trust it. Live demos run the whole stack
client-side at **[tindalabs.dev](https://tindalabs.github.io/tindalabs.dev/)**.

| Project | What it is | Stack |
|---|---|---|
| **[Shield](https://github.com/tindalabs/shield)** · [`npm`](https://www.npmjs.com/package/@tindalabs/shield) | Content-integrity toolkit: tamper detection, structured risk `assess()`, a declarative policy engine, and an OpenTelemetry bridge. Zero runtime deps. | TypeScript |
| **[Scent](https://github.com/tindalabs/scent)** · [`npm`](https://www.npmjs.com/package/@tindalabs/scent-sdk) | Identity engine: signal collection, identity clustering, and drift detection, split across SDK / engine / server / OTel packages. | TypeScript monorepo |
| **[Blindspot](https://github.com/tindalabs/blindspot)** · [`npm`](https://www.npmjs.com/package/@tindalabs/blindspot) | Privacy-first browser auto-instrumentation, with first-class Vue, Next.js, and Svelte integrations. | TypeScript monorepo |
| **[tindalabs.dev](https://github.com/tindalabs/tindalabs.dev)** | The landing page and live playground: a fully static Next.js 15 export that runs the entire stack in the browser, no backend. | Next.js 15 |

## Developer tooling

| Project | What it is | Stack |
|---|---|---|
| **[Stele](https://github.com/Isonimus/stele)** · [`npm`](https://www.npmjs.com/package/@isonimus/stele) | A zero-dependency workflow that keeps a repo's decisions, work, and definition of done honest, enforced by a git hook and CI rather than by anyone remembering to. Vendored into any repo with one command. | TypeScript |
| **[Chiron](https://github.com/Isonimus/chiron)** · [`npm`](https://www.npmjs.com/package/@isonimus/chiron) | A local-only coding mentor. Reads your own AI-assistant transcripts and git history, finds where your craft is strong or growing, and builds evidence-cited ~2-hour learning roadmaps. Nothing leaves your machine. | TypeScript |
| **[c-level](https://github.com/Isonimus/c-level)** · [`npm`](https://www.npmjs.com/package/@isonimus/c-level) | AI executive-advisory system: points at a repo, extracts structured signals, and returns CTO/CPO/COO/CMO/CFO/CSO assessments grounded in real code. | TypeScript |
| **[Glitch.js](https://github.com/Isonimus/glitch-js)** · [`npm`](https://www.npmjs.com/package/@isonimus/glitch-js) | A lightweight, dependency-free library for stackable visual glitch effects. | TypeScript |
| **[Gravity](https://github.com/Isonimus/Gravity)** | A VS Code / Antigravity extension that watches AI model quota and warns you before a cooldown penalty hits. | TypeScript |

## Accessibility & computer vision

| Project | What it is | Stack |
|---|---|---|
| **[Mira](https://github.com/Isonimus/mira)** | Hands-free web navigation from a plain webcam: your head aims a cursor, an eyebrow raise clicks and drags, and an on-screen keyboard lets you type. All face processing runs on-device, so no video ever leaves the machine. Built for people who can't use a conventional pointer. | TypeScript · MediaPipe |

## Security & embedded

| Project | What it is | Stack |
|---|---|---|
| **[monero-miner](https://github.com/Isonimus/monero-miner)** | A high-performance Monero CPU miner tuned for lower-end laptops and non-gaming PCs. | Rust |
| **The Adversary** *(private)* | A wide-spectrum WiFi / BLE / IR / RFID / HID security-testing platform for the M5 Cardputer: handshake capture, evil-twin captive portals, GPS wardriving with WiGLE upload, DuckyScript over USB and BLE. | C / C++ (ESP32-S3) |
| **Dupin** *(private)* | The defensive counterpart: a passive, monitor-mode-only Wi-Fi intelligence toolkit that baselines an environment and flags evil twins, rogue APs, and security downgrades. Never transmits. | C / C++ (ESP32-S3) |

## Simulations, games & ML

| Project | What it is | Stack |
|---|---|---|
| **[LINARES](https://github.com/Isonimus/linares)** | A private movie recommender that learns your taste: a personalised CatBoost model over genre metadata, target-encoded cast/crew, and 384-dim NLP plot embeddings. | Python · Vue |

A parallel line of local, not-yet-public work explores procedural worlds and emergent systems:
**Boxel** (a voxel engine with worm-carved cave systems and a mood-aware generative soundtrack),
**Anthill** and **Vivarium** (agent-based colony and genetic-inheritance simulations, both built
on seeded determinism harnesses), **dark** (an audio-only maze puzzle that's fully
screen-reader-playable), and **Pull Request** (a code-review inspection game in the shape of
*Papers, Please*). Happy to demo any of them.

<sub>Projects marked *(private)* are active local work not yet pushed to a public remote; happy to walk through any of them.</sub>

## Contributions

| Project | Role |
|---|---|
| **[M5PORKCHOP](https://github.com/0ct0sec/M5PORKCHOP)** | Contributor to the firmware for this M5Stack security-research handheld: recovery/OTA resilience and feature work. C / C++, ESP32. |

## Professional experience

Day to day I work on a large-scale **learning-management platform**: multi-year, high-traffic
Vue front ends measured in tens of thousands of commits. The interesting parts have been a
content-authoring CMS that lets each client tailor their own courseware, AI-assisted content and
roleplay-simulation generation, gamified learning modules, and a talent-assessment product. That
codebase is private, so there are no links here, but I'm glad to talk through the architecture.
