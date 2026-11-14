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

#### 🕰️ Earlier

Before all this it was mostly frontend: React, Angular, Webpack and Node, going back to the
jQuery days. Some of it is still here, such as [react-dagred3](https://github.com/mozartdiniz/react-dagred3)
and [zMaps](https://github.com/mozartdiniz/zMaps), a Google Maps alternative for Firefox OS (2014).
