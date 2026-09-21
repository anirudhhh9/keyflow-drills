![preview](https://raw.githubusercontent.com/anirudhhh9/keyflow-drills/main/poster_775141.svg)
[![Download](https://raw.githubusercontent.com/anirudhhh9/keyflow-drills/main/app_98b822b.svg)](https://anirudhhh9.github.io/keyflow-drills/)

# ⌨️ kbhabit — Turn Typing Into a Lifelong Ritual

**kbhabit** is a keyboard trainer built around one bold premise: muscle memory is not something you buy, it is something you *grow*. Where most typing tools hand you a scoreboard and send you on your way, kbhabit plants a seed and asks you to water it daily. This repository is the next chapter of that idea — a reimagined, habit-first training environment that treats every keystroke as a small act of craftsmanship.

If you have ever promised yourself you would learn touch typing "someday," kbhabit is the someday. It does not nag. It does not shame. It simply shows up, day after day, with a lesson that fits the shape of your schedule and the rhythm of your fingers.

The entire project is released under the MIT license and built with the belief that better typing is a public good, not a premium subscription.

---

## 🌱 What This Project Is

kbhabit is a desktop-first, browser-friendly keyboard trainer whose core unit is not the *lesson* but the *streak*. Instead of measuring how fast you typed today, it measures how many consecutive days you came back. Speed is a side effect of consistency — never the other way around.

This repository contains the full source tree for the trainer: the lesson engine, the habit tracker, the multilingual interface, the progress dashboard, and the styling system that keeps everything calm and legible at 2 a.m.

Think of it as a garden. Each practice session is a watering. The dashboard is the growth chart. The streak counter is the vine climbing the trellis. Miss a day and nothing dies — the vine simply waits, patient, for your return.

---

## 🎯 Why Another Keyboard Trainer?

Because the world has enough leaderboards. What it lacks is a trainer that respects your attention.

- Most trainers optimize for a single number: words per minute.
- kbhabit optimizes for a single behavior: returning tomorrow.

That shift changes everything — the lesson design, the pacing, the difficulty curve, the way progress is visualized, and the emotional tone of every screen. A fast typist who quits after a week gains nothing. A slow typist who practices for a year becomes unreachable. kbhabit is built for the second person.

---

## ✨ Feature Highlights

### 🧠 Habit-First Lesson Engine
Lessons adapt to your streak, not just your accuracy. Recover from a long break with a gentle warm-up. Ride a hot streak into progressively denser drills. The engine quietly adjusts difficulty so the session always feels finishable.

### 🎨 Responsive Interface
The layout reshapes itself from a wide desktop monitor down to a compact tablet window without losing a single control. Large hit targets, generous line height, and a color palette that survives both bright offices and dim bedrooms.

### 🌍 Multilingual Support
Interface strings, lesson hints, and drill vocabularies are decoupled from the code. Adding a language is a matter of dropping a translation file into the right directory — no rebuild of the core required. Community translations are welcomed and credited.

### 📊 Progress Without Pressure
Charts that show trajectory rather than judgement. Weekly heat maps, rolling accuracy curves, and a streak calendar that reads like a diary rather than a report card.

### 🔔 Thoughtful Reminders
Optional session nudges that respect quiet hours and never escalate in tone. A reminder from kbhabit should feel like a friend tapping the table, not a manager tapping a watch.

### 🕛 Always-On Support Cadence
Documentation, issue triage, and community answers run on a rolling schedule, so questions rarely sit unanswered for long — regardless of your timezone.

### 🖥️ Local-First Data
Your typing history lives with you. Export it, back it up, or move it between machines. No mandatory account, no silent synchronization, no mystery.

### 🧩 Extensible Drill Packs
Bring your own word lists — code snippets, medical terminology, a novel you are retyping for pleasure. The drill format is plain and documented.

### ♿ Accessibility Consideration
Keyboard-only navigation, visible focus states, adjustable contrast, and screen-reader labels on every interactive element.

[![Download](https://raw.githubusercontent.com/anirudhhh9/keyflow-drills/main/app_98b822b.svg)](https://anirudhhh9.github.io/keyflow-drills/)

---

## 🛠️ How It Fits Together

The architecture is deliberately boring, because boring software is software you can trust with a daily habit.

**Lesson Core** — parses drill definitions and emits the sequence of prompts you see on screen.

**Habit Ledger** — records each finished session with timestamp, accuracy, and duration. The ledger is append-only and portable.

**Streak Calculator** — derives current streak, longest streak, and consistency ratio from the ledger.

**Interface Shell** — renders the current prompt, the virtual keyboard hint, and the live metrics.

**Localization Layer** — resolves every user-facing string through a translation table.

**Theme System** — swaps color tokens and spacing scales without touching component logic.

Each layer talks to the next through a narrow, well-documented interface. Replacing any one of them should not disturb the others.

---

## 🚀 Getting Started (Conceptual Walkthrough)

This section describes the *shape* of the setup rather than the exact commands, because the exact commands depend on how you prefer to run desktop tooling.

1. Obtain a copy of this project onto your machine by whatever means you normally acquire source.
2. Ensure a modern runtime of your chosen platform is present.
3. Resolve the project's declared dependencies using your platform's package manager.
4. Launch the application in development mode to confirm the interface loads.
5. Open the habit ledger location and confirm the file is writable.
6. Complete one drill and verify the streak counter increments.

If step six succeeds, you are done. Everything after that is practice.

---

## 📚 Usage Patterns

### The Two-Minute Morning
Open the trainer, complete the shortest available drill, close it. The streak survives. This is the single highest-leverage habit in the entire system.

### The Deep Session
On days with more time, chain three or four drills across different vocabularies to stress different finger pathways.

### The Recovery Week
After travel or illness, use the warm-up drills exclusively. The engine will not punish you for a gap; it will simply re-measure where you are.

### The Language Swap
Switch the interface language and the drill vocabulary together to practice typing in a second language — a quietly powerful way to reinforce both skills at once.

---

## 🗺️ Roadmap for 2026

- Q1 2026 — Ledger schema stabilization and export format documentation.
- Q2 2026 — Additional community-contributed drill packs and expanded multilingual string coverage.
- Q3 2026 — Accessibility audit pass and contrast tuning across all themes.
- Q4 2026 — Long-term statistics view with yearly retrospectives and habit anniversary markers.

The roadmap is a direction, not a contract. Contributions that improve the daily return rate take priority over features that merely add novelty.

---

## 🤝 Contributing

Contributions are warmly welcomed, and the best ones are small.

- Fix a translation string that reads awkwardly in your language.
- Add a drill pack for a domain you know well.
- Improve the documentation where it confused you.
- Report a bug with a clear reproduction path.

Larger changes should start as a discussion issue so the design can be shaped before the code is written. There is no contribution too modest — a single corrected typo in a hint string has improved this project before.

Please keep the tone of issues and pull requests constructive. This is a habit project; the community around it should feel like one.

---

## 🔐 Privacy Stance

kbhabit keeps your practice history on your own machine by default. There is no telemetry pipeline, no analytics beacon, and no third-party tracker embedded in the interface. If you choose to share statistics, you do so by exporting them deliberately. The project holds no keys to your habits.

---

## 🧭 Design Principles

**Consistency over intensity.** A short session you actually complete beats a long session you abandon.

**Calm over competitive.** No global leaderboards, no public rankings, no pressure theater.

**Legible over clever.** Every screen should be readable by someone tired at the end of a long day.

**Portable over locked-in.** Your data leaves as easily as it arrives.

**Inclusive over exclusive.** Multiple languages, accessible controls, and no gatekeeping.

---

## ❓ Frequently Asked Questions

**Do I need an account?**
No. The trainer works entirely on local state.

**Will my streak break if I miss a day?**
The streak reflects consecutive days practiced. A missed day resets the count, but your ledger, statistics, and progress remain untouched.

**Can I practice in more than one language?**
Yes — the interface language and the drill vocabulary are independent settings.

**Is there a mobile version?**
The responsive layout works comfortably on tablets. Phone-sized layouts are on the roadmap.

**How do I back up my history?**
Copy the habit ledger file to any location you trust. It is plain, documented, and forward-compatible.

**Can I contribute a drill pack without writing code?**
Yes. Drill packs are declarative text; no programming knowledge is required.

---

## 🧾 License

This project is distributed under the MIT License. You may use, modify, and redistribute it with attribution. See the full text at the official license reference:

https://opensource.org/licenses/MIT

Copyright (c) 2026 kbhabit contributors.

---

## ⚠️ Disclaimer

kbhabit is provided as-is, without warranty of any kind, express or implied. The authors are not liable for any loss of data, interruption of practice, or physical discomfort arising from extended use. Typing is a physical activity; take breaks, stretch your hands, and adjust your workstation to a comfortable posture. Nothing in this repository constitutes medical or ergonomic advice. Statistics presented by the application are estimates derived from your own input and should be treated as guidance rather than measurement. Always keep independent backups of any habit ledger you care about.

---

## 💬 Final Thought

A keyboard trainer is only as good as the day you return to it. kbhabit exists to make that return effortless — a quiet room, a short drill, a streak that grows by one. Everything else in this repository serves that single moment.

[![Download](https://raw.githubusercontent.com/anirudhhh9/keyflow-drills/main/app_98b822b.svg)](https://anirudhhh9.github.io/keyflow-drills/)