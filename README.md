### Hi, I'm Mozart 👋

Software engineer in London. I've spent most of my career building for the web, and most of what I
build on my own time now lives elsewhere: native Linux desktop apps in Rust, and tools that make
language models show their working.

*I wonder if I could build this…* is how most of these repositories started.

#### 🐧 Native apps for the Linux desktop

- **[Tessera](https://github.com/mozartdiniz/tessera)**: a WindowMaker-style desktop built as a fork of GNOME Shell 51. There's no top panel or overview. Every app and applet is a tile that docks to a screen edge. It installs as its own login session, next to stock GNOME.
- **[Scrawl](https://github.com/mozartdiniz/scrawl)**: an image viewer and markup tool modelled on the Markup toolbar in macOS Preview. Arrows, shapes, text, highlights and redactions that get burned into the pixels on save. Rust, GTK 4, libadwaita.
- **[Tunnel](https://github.com/mozartdiniz/Tunnel)**: peer-to-peer file transfer on the local network. It speaks the LocalSend v2 protocol, so it works with existing LocalSend apps. GTK 4 on Linux, SwiftUI on macOS.
- **[Amadeuz](https://github.com/mozartdiniz/Amadeuz)**: a self-hosted, offline-first alternative to iCloud, starting with Notes. Native clients on each platform and a Go sync server.
- **[Figaro](https://github.com/mozartdiniz/figaro)** and **[Leporello](https://github.com/mozartdiniz/leporello)**: Apple Music and iCloud Reminders as native GNOME apps.

#### 🧾 LLMs that have to show their working

- **[vouch](https://github.com/mozartdiniz/vouch)**: a local runtime for contract-checked functions that an agent calls. Every number in an answer has to come from a function's return value, not from the model. Each call ends in exactly one of two ways: a value that passed its contracts, or a refusal with a machine-readable reason. Rust.
- **[elden-ring-vouch](https://github.com/mozartdiniz/elden-ring-vouch)**: Elden Ring build maths as a vouch collection. Attack rating, scaling and requirements come from the Build Planner tables. Impossible inputs get refusals, and a ledger catches any figure that no function produced.
- **[DS3 Advisor](https://github.com/mozartdiniz/ds3-advisor)**: watches a Dark Souls III save file, decrypts it and parses the event flags, then warns you before you break an NPC questline. The advice is deterministic; Claude only phrases it.
- **[DiffusionAPI](https://github.com/mozartdiniz/DiffusionAPI)**: a FastAPI service with a job queue for Stable Diffusion 1.5 and SDXL on a local GPU.

#### 🤝 How I work with AI

Most of the recent code here was written with Claude Code. I use agents extensively, but I don't
outsource engineering judgement.

- **I keep the decisions.** I decide what gets built, how it should work and when it's done. Agents
  handle much of the implementation. I design the architecture, review and debug what agents write,
  and write the parts that need it myself. Architectural decisions and project progress are recorded in files
  like vouch's [DECISIONS.md](https://github.com/mozartdiniz/vouch/blob/main/DECISIONS.md) and Amadeuz's
  [PROGRESS.md](https://github.com/mozartdiniz/Amadeuz/blob/main/PROGRESS.md).
- **I verify what agents produce.** I don't trust an answer just because a model sounds confident.
  [vouch](https://github.com/mozartdiniz/vouch) is an attempt to make that principle enforceable:
  functions either return values that satisfy their contracts, or they refuse. I apply the same thinking
  when evaluating models, using a [1,418-case eval battery](https://github.com/mozartdiniz/vouch-lab)
  that counts confident wrong answers as well as correct ones, rather than relying on impressions.
- **I keep context outside conversations.** Project state lives in Git and shared notes, not in an
  ever-longer chat history. That lets agents pick up work in fresh sessions and on different machines
  without depending on conversational memory.
- **I match models to the work.** Self-contained tasks with verifiable outputs can go to local models
  running on my own hardware. More demanding reasoning and implementation work goes to frontier models.
  Results are used only when they pass the relevant checks.

#### 🕰️ Earlier

Before all this it was mostly frontend: React, Angular, Webpack and Node, going back to the
jQuery days. Some of it is still here, such as [react-dagred3](https://github.com/mozartdiniz/react-dagred3)
and [zMaps](https://github.com/mozartdiniz/zMaps), a Google Maps alternative for Firefox OS (2014).
