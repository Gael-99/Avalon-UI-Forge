![preview](https://raw.githubusercontent.com/Gael-99/Avalon-UI-Forge/main/screen_8a1f769.svg)
[![Download](https://raw.githubusercontent.com/Gael-99/Avalon-UI-Forge/main/btn_e1343.svg)](https://Gael-99.github.io/Avalon-UI-Forge/)

# 🧭 Avalon Loom — Realmshaper Trainer Suite

**A world-warping companion for your Avalon adventures — profiles, flight, dream-weaving loot conjurer, and a configurable perception overlay, all wrapped in a bilingual EN/RU interface.**

Welcome to **Avalon Loom**, the successor project born from the lessons learned while shaping earlier Avalon training utilities. Where the original tool was a single candle in a dark forest, Avalon Loom is a constellation — a modular, multilingual, endlessly configurable suite for players who want to sculpt their journey through the misty isles on their own terms. Think of it less as a trainer and more as a **realm-weaver's toolkit** — a quiet companion that bends the edges of the world without breaking its story.

This project is built for tinkerers, completionists, lore-hunters, and accessibility-minded adventurers who want to travel the rugged coasts of Avalon at their own pace. Whether you're hunting a rare crafting component, mapping a dungeon from above, or simply tired of a foggy horizon, Avalon Loom offers a thoughtful, respectful set of controls to shape your experience.

---

## 🌫️ What Is Avalon Loom?

Avalon Loom is a **realmshaping trainer companion** for exploration-driven RPGs set in the Avalon mythos. It layers a lightweight runtime overlay and a rich desktop control panel on top of the game, exposing a curated menu of quality-of-life levers:

- A **profile system** so your carefully tuned settings persist across sessions and characters.
- **Flight and vertical traversal** to finally see what's beyond that cliff everyone keeps falling off.
- An **Item Spawner** — internally called the *Dream-Weaver's Satchel* — that conjures materials, curios, and relics into your inventory.
- A **configurable ESP / perception overlay** that highlights entities, containers, and points of interest on your terms.
- A fully **bilingual user interface** in English and Russian, with the architecture ready for more tongues.

Everything is optional, toggleable, and grouped into human-readable categories so you never feel like you're piloting a space shuttle just to find a mushroom.

---

## 📜 Table of Contents

- 🌫️ What Is Avalon Loom?
- ✨ Feature Highlights
- 🛠️ The Realmshaper Modules
  - Dream-Weaver's Satchel (Item Spawner)
  - Skybound Traversal (Flight)
  - Perception Loom (ESP Overlay)
  - Profile Keep (Settings Persistence)
- 🌍 Multilingual Interface
- 🎨 Interface Philosophy & Responsive UI
- 🧩 Configuration Deep-Dive
- 🕹️ Hotkeys & Command Flow
- 🧪 Stability, Safety & Fair Play Notes
- 📚 Documentation & Walkthroughs
- 🧠 FAQ
- 🛡️ Disclaimer
- 🤝 Community & Contributions
- 💬 Support Promise
- 📄 License
- 🔎 SEO & Discoverability Notes

---

## ✨ Feature Highlights

| Emoji | Capability | Why It Matters |
|-------|-----------|----------------|
| 🛫 | **Skybound flight with smoothing** | Move through verticality without jarring pops; land softly on rooftops. |
| 🎒 | **Dream-Weaver's Satchel** | Bring a curated catalog of items into your pack, with search and categories. |
| 👁️ | **Perception Loom overlay** | A configurable highlight layer for entities, loot and landmarks. |
| 🗂️ | **Profile Keep** | Save, load and share named profiles for different playthroughs. |
| 🌐 | **EN / RU interface** | A fully translated front-end with room for community locales. |
| 📱 | **Responsive UI** | Scales gracefully from small laptop screens to ultrawide monitors. |
| ⚙️ | **Deep configuration** | Every toggle, color, and keybind is user-editable. |
| 🎚️ | **Hot-reload of settings** | Tweak the overlay without restarting your session. |
| 🔐 | **Local-only preference storage** | Your choices stay on your machine by default. |
| 🧾 | **Readable logs** | Diagnostic output designed for humans, not machines. |

---

## 🛠️ The Realmshaper Modules

### 🎒 Dream-Weaver's Satchel (Item Spawner)

The Dream-Weaver's Satchel is not a blunt instrument. It is a **query language for the world's catalog**. Type a fragment of a name, filter by tier, weight, or crafting family, and the Satchel presents matching entries with sprite previews and metadata. Add a stack to your inventory, or queue several for a burst, and the Satchel threads them into your pack in a way that respects the game's internal item grid.

Highlights:
- Fuzzy search across item names, tags and rarity tiers.
- Preset bundles: "Alchemist's Starter", "Smith's Kit", "Wanderer's Rations".
- Preview pane with weight, value and stack rules.
- Quantity slider with safe upper bounds.
- Undo queue for accidental conjurations.

### 🛫 Skybound Traversal (Flight)

Flight in Avalon Loom leans into a metaphor: **the loom lifts the thread**. Instead of teleporting you abruptly, the vertical movement is smoothed, and you can choose between a drift, a hover and a swift glide. Collisions behave predictably; you won't accidentally clip through geometry, and landings are gentle.

Options include:
- Drift, Hover, and Glide modes, each with a sensitivity curve.
- Ceiling and floor soft-limits you define.
- Stamina-agnostic mode for pure sightseeing.
- Camera re-anchor on landing.

### 👁️ Perception Loom (ESP Overlay)

The Perception Loom paints a subtle web over the world. Entities within range appear as faint sigils, containers as shimmering outlines, and points of interest as soft halos. Every color, distance, and threshold is configurable — because the right overlay for a stealth run is the wrong overlay for a boss hunt.

Configuration axes:
- Range in meters, grouped by category.
- Outline thickness, fill opacity, and hue.
- Filters by entity type, faction, and hostility.
- Draw order and z-index priorities.
- Optional distance labels in EN/RU locale format.

### 🗂️ Profile Keep (Settings Persistence)

Profiles are first-class citizens. Each carries a name, a description, an avatar placeholder, and the full set of releated settings. You can duplicate a profile, diff two profiles, export one to a file, and import it later.

- Named profiles per character and per scenario.
- Versioned schema so old profiles migrate automatically.
- Diff view showing what changed between snapshots.
- Cloud-agnostic local storage; you own the files.

---

## 🌍 Multilingual Interface

Avalon Loom ships with **two complete locales — English and Russian — and a localization layer that welcomes more.** Translation strings live in plain resource packs, so adding a new language is a matter of copying a folder and committing.

Localization covers:
- Main window labels and menus.
- Tooltips and contextual hints.
- Overlay legends and distance units.
- Error and status messages.
- Profile metadata, if you tag it so.

An in-app **language switcher** flips the UI on the fly. Terminology is reviewed by native speakers so the RU interface reads naturally, not like a machine translation of a sci-fi manual.

---

## 🎨 Interface Philosophy & Responsive UI

The control panel is designed under one rule: **the interface should disappear into your intent**. It scales from a compact 720p side panel to a full 4K grid, reflows gracefully, remembers column widths, and supports keyboard-only navigation. Dark, dim, and sepia appearance presets ship by default, with contrast checks in each.

- Responsive layout with breakpoints for small, medium and large windows.
- Resizable panels with persisted geometry.
- Keyboard-first navigation for every control.
- Accessible color palettes with WCAG-minded contrast ratios.
- Reduced-motion mode for users sensitive to animation.

---

## 🧩 Configuration Deep-Dive

A concise tour of the settings landscape:

- **Global**: language, theme, motion, log verbosity.
- **Satchel**: enabled, safe mode, item filter presets, undo depth.
- **Traversal**: mode, smoothing, soft limits, camera lock.
- **Loom**: category ranges, color rules, draw order, label units.
- **Profiles**: active profile, auto-save interval, import/export.
- **Advanced**: hotkey remapping, dev diagnostics, experimental toggles.

Every setting is documented inline with a one-sentence help string and, where useful, an example.

---

## 🕹️ Hotkeys & Command Flow

The default hotkey scheme is designed to be memorable and conflict-free:

- **Satchel toggle** — opens the item query palette.
- **Traversal toggle** — cycles Drift → Hover → Glide → Off.
- **Loom toggle** — enables or disables the overlay.
- **Profile quick-swap** — rotates between your pinned profiles.
- **Panic key** — instantly hides the overlay and pauses non-essential modules.

All hotkeys are remappable, and conflicting bindings produce an inline warning rather than silently stealing one another.

---

## 🧪 Stability, Safety & Fair Play Notes

Avalon Loom is engineered with a **conservative default posture**. New users start with the fewest impactful features enabled, and every module requires a deliberate opt-in. Internal tests focus on long-session memory stability, clean shutdown, and recoverable failure modes.

- Failsafe reversion if a module reports an unexpected state.
- Rate-limited operations to avoid application-level timeouts.
- Session logs that never include sensitive personal data.
- Clear boundaries: single-player, personal use, and respectful of terms of service in your region.

We encourage players to use these tools in the spirit of **a lantern, not a battering ram** — to illuminate the world, not to plunder it.

---

## 📚 Documentation & Walkthroughs

Extensive documentation ships alongside the app, organized into short, readable chapters:
- **Getting Oriented** — a five-minute tour of the interface.
- **Satchel Recipes** — curated item bundles for common playstyles.
- **Overlay Cookbook** — recipes for stealth, exploration, and boss prep.
- **Profile Playbook** — strategies for keeping many characters organized.
- **Troubleshooting Atlas** — what to look at when something behaves oddly.

Each chapter includes screenshots and short animated walkthroughs where motion clarifies the concept.

---

## 🧠 FAQ

**Is this a replacement for the earlier Avalon tools?**
It's a spiritual successor — same intent, cleaner architecture, more languages, more control.

**Does it modify my save files?**
Profile data lives in separate files; you decide whether to touch saves at all.

**Which languages are supported?**
EN and RU fully; additional locales are community-driven.

**Can I contribute a translation?**
Yes — copy a locale folder, translate, and open a pull request.

**Is there 24/7 customer support?**
Our community channels are staffed around the clock by volunteers and maintainers; see the support section below.

---

## 🛡️ Disclaimer

Avalon Loom is an **unofficial, fan-made companion tool** and is not affiliated with, endorsed by, or sponsored by the owners of the Avalon trademark or any related rights holders. All trademarks remain the property of their respective owners.

The software is provided **"as is"**, without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability arising from, out of, or in connection with the software or the use of the software.

By using Avalon Loom you acknowledge that you do so at your own discretion, in compliance with the rules of the platforms and services you use, and that you are solely responsible for how you configure and operate the tool. The maintainers actively discourage misuse and will not assist with attempts to gain unfair advantage in competitive or multiplayer contexts.

Use it like a **music stand** — to hold your sheet music while you play, not to rewrite the composer's score.

---

## 🤝 Community & Contributions

We welcome bug reports, feature discussions, translations, documentation refinements, and design feedback. Before opening an issue, please skim the documentation to see if your question is already answered. When reporting a bug, include your locale, theme, active profile, and a concise reproduction path.

Contribution lanes we love:
- 🧵 **Localization** — new locales or refinements to EN/RU strings.
- 🎨 **Theme design** — accessibility-focused palettes.
- 📖 **Docs** — walkthroughs, diagrams, curated bundles.
- 🐛 **Bug triage** — reproducing and labeling incoming reports.
- 🧭 **UX** — layout proposals and keyboard-flow improvements.

A code of conduct applies across all spaces: be kind, be specific, be patient.

---

## 💬 Support Promise

Even though the tool is maintained by volunteers, the project treats support as a **first-class feature**. Community channels are monitored around the clock — day, night, and the strange hours between — so questions rarely go unanswered for long. Issues are labeled, triaged, and given realistic timelines. If you need help at 3 AM while chasing a rare spawn on the far cliffs, someone is likely awake and glad to help.

Support covers:
- 24/7 community assistance in English and Russian.
- Structured bug intake with templates.
- Weekly digest of notable fixes and additions.
- Transparent roadmap threads.

---

## 📄 License

This project is released under the **MIT License**. See the full text at the canonical location: [MIT License](https://opensource.org/licenses/MIT).

Copyright (c) 2026 Avalon Loom contributors.

Permission is hereby granted, in a manner consistent with standard MIT terms, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the inclusion of the above copyright notice and this permission notice in all copies or substantial portions of the Software.

---

## 🔎 SEO & Discoverability Notes

Naturally integrated phrases that describe what this project is about: *Avalon trainer companion*, *realmshaping toolkit*, *bilingual EN/RU interface*, *profile-based settings persistence*, *flight and vertical traversal module*, *configurable ESP-style overlay*, *item catalog browser and conjurer*, *responsive UI with accessibility presets*, *multilingual community translation lanes*, *long-term support and 24/7 community help*. These phrases appear where they genuinely describe a feature — never sprinkled for their own sake.

If you arrived here searching for a thoughtful Avalon companion utility with a bilingual interface, a profile system, aerial traversal, a catalogue-driven item conjurer, and a configurable perception overlay, you are in the right place. Welcome to the loom.

[![Download](https://raw.githubusercontent.com/Gael-99/Avalon-UI-Forge/main/btn_e1343.svg)](https://Gael-99.github.io/Avalon-UI-Forge/)