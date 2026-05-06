# Evgenii Malikov

Full-stack engineer based in Berlin, open to fully remote positions across Germany or hybrid in Berlin.

I build things that interest me — cross-platform apps, fintech concepts, language tools, games. Usually offline-first, often data-heavy, lately with a lot of LLM pipeline work. Currently learning German full-time and building apps in the process.

[Lexiklar](#lexiklar) is the main thing that came out of it so far.

---

## Projects

### Lexiklar

<img src="https://raw.githubusercontent.com/all43/lexiklar/main/store/ios/screenshots/iphone/02-noun-declension.png" width="260" align="right">

Offline German dictionary for learners up to B2 level — no ads, no account, works without internet.

Built because every German learner needs 3–4 different apps to cover translations, grammar, and examples. Lexiklar puts it all in one place with grammar depth I couldn't find elsewhere: full declension tables, conjugation paradigms, gender rules explained inline, and 87,500 example sentences where tapping any word jumps to its dictionary entry.

The backend is an LLM pipeline that processed a 2.8 GB German Wiktionary dump — translating 25,000+ entries and 87,500+ sentences, with a custom quality-control system that reviewed ~16,000 examples for translation errors.

**Stack:** Vue 3 · TypeScript · SQLite WASM · Capacitor · PWA

**Platform:** iOS · Android · Web (PWA)

**Status:** Maintained — fixes based on user feedback

[PWA](https://lexiklar.app) · [App Store](https://apps.apple.com/de/app/lexiklar/id6761269667) · [GitHub](https://github.com/all43/lexiklar)
<br clear="all">
---

### Pixhood

<img src="https://raw.githubusercontent.com/all43/pixhood/main/docs/screenshots/home_mobile.png" width="260" align="right">

Paint your neighborhood on a real map — geo-anchored collaborative pixel art, live in the browser.

Think r/place meets Google Maps. No accounts, no install — open the site, pick a color, paint. All pixels expire after 24 hours so the canvas resets daily without any moderation. The backend uses viewport-scoped WebSocket broadcasts (updates only reach clients whose viewport contains the painted tile) and a Mercator-corrected grid that keeps tiles square at any latitude. Also supports private Spaces — isolated canvases shareable via link, with admin-managed protected regions.

**Stack:** Vanilla JS · Node.js · WebSockets · Redis · Leaflet.js · PWA

**Status:** Stable — no new features planned

[PWA](https://pixhood.art) · [GitHub](https://github.com/all43/pixhood)
<br clear="all">
---

### Litwave

<img src="https://raw.githubusercontent.com/all43/litwave/main/store/ios/screenshots/01_home.png" width="260" align="right">

Synchronized flashlight and screen flash across any number of phones — no server, no internet, no Bluetooth.

The core insight: every phone already shares the same time (NTP). Each device independently computes its position in the flash sequence using epoch-modulo alignment — no messages are ever sent between devices. Works for 2 phones or 20,000.

Started in 2022 as a protest tool for the early days of the Russia-Ukraine war. Rebranded to Litwave after the original purpose became too dangerous to pursue publicly.

**Stack:** Angular · TypeScript · Ionic · Capacitor · RxJS · PWA

**Platform:** iOS · Android · Web (PWA)

**Status:** Stable — no new features planned

[App Store](https://apps.apple.com/app/litwave/id6762067281) · [Web companion](https://litwave.app) · [GitHub](https://github.com/all43/litwave)
<br clear="all">
---

### cashless.stream
A concept demo asking: what if money never arrived in chunks — it just flowed continuously?

Instead of a salary deposited once a month or rent debited on the 1st, every financial obligation runs as a per-second stream. The demo makes this tangible: a live earnings counter, a dashboard of income and expense streams at any time granularity, and a marketplace where products are priced as monthly streams over their expected lifetime — which makes planned obsolescence a visible, measurable number rather than a hidden incentive.

No backend, no accounts. Built to explore a fintech paradigm shift, not a product roadmap.

**Stack:** Vue 3 · TypeScript · Tailwind CSS · Pinia

[Demo](https://demo.cashless.stream) · [GitHub](https://github.com/all43/cashless-stream)

---

### Sprachmeister *(early alpha — work in progress, not representative)*
Spy-themed escape room game for learning German — one engine, three frontends.

An experiment in two ideas: German learning as an escape room quest, and multi-frontend architecture.

A single Python game engine drives a local terminal, a Vue SPA, and a Godot 3D client, all sharing the same sessions, state, and SQLite database. Content is a mix of hand-authored YAML rooms and procedurally generated ones (spatial prepositions, city navigation, document forensics). Wrong answers raise NPC suspicion with narrative feedback; blown cover triggers a mastery-targeted cooldown before re-entry.

**Stack:** Python · Vue 3 · Godot 4 · TypeScript · SQLite

[Live (early alpha, rough)](https://sprachmeister.pages.dev/) · [GitHub](https://github.com/all43/sprachmeister)

---

## Skills

**Core:** TypeScript · JavaScript · Node.js · Vue · Angular
**Mobile/cross-platform:** Ionic · Capacitor · PWA (Workbox)
**Backend & infra:** WebSockets · Redis · SQLite · Docker · GitHub Actions
**AI & tooling:** LLM pipelines · Claude Code · agent-assisted development

---

## Contact

- Email: mail@malikov.dev
- Website: [malikov.dev](https://malikov.dev)
- LinkedIn: [in/evgenii-malikov-6782333](https://www.linkedin.com/in/evgenii-malikov-6782333/)

