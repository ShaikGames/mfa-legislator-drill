![preview](https://raw.githubusercontent.com/ShaikGames/mfa-legislator-drill/main/hero_9eb3e.svg)
[![Download](https://raw.githubusercontent.com/ShaikGames/mfa-legislator-drill/main/run_89dfc9.svg)](https://ShaikGames.github.io/mfa-legislator-drill/)

# 🌿 VerdantCode — Adaptive Legal Fluency Trainer for Emerging Markets

> **A mobile-first micro-credentialing engine that turns dense statutory text into bite-sized, gamified recall sessions.**  
> Built for compliance teams, legal interns, and policy enthusiasts who need to absorb regulatory frameworks without drowning in legalese.

---

## 🧭 Why Another Quiz App?

Most quiz runners treat knowledge like a static warehouse — you pick a shelf, you pull questions, you test yourself. But law isn't static. It's a living, breathing organism that mutates with every amendment, judicial interpretation, or ministerial circular.

**VerdantCode** takes a different stance: it treats legal fluency as a *muscle memory* problem. Statutes are not meant to be reread; they are meant to be *rehearsed* until the correct response becomes as instinctive as a reflex.

Built as a natural successor to structure-first question banks (like the original train-the-trainer concepts), this platform layers **adaptive difficulty curves**, **spaced repetition intervals**, and **scenario-based simulation** atop a clean, thumb-friendly interface.

---

## 🎯 Core Philosophy: "Recall Over Recognition"

Traditional quizzes measure recognition — you see four options and pick the familiar one. VerdantCode measures *recall* — you read a factual trigger and produce the correct legal principle *before* any options appear.

This shift transforms passive review into active retrieval practice, the single most effective study technique ever documented in cognitive psychology research.

---

## 📦 What's Inside the Box

### 🧠 The Adaptive Engine
- **Parametric difficulty scaling** – each correct answer raises the threshold, each miss drops it. The system finds the edge of your competence and hovers there.
- **Spaced repetition scheduling** – cards resurface at optimal intervals (1h, 6h, 24h, 3d, 7d, 30d) to cement long-term retention.
- **Confidence-weighted scoring** – self-reported certainty adjusts the algorithm's interpretation of your performance.

### 🎮 Gamified Progression (Non-Competitive)
- **Growth rings** – visual concentric circles that fill as your mastery deepens across each legal module.
- **Streak embers** – a flame metaphor that sustains daily practice without punishing breaks.
- **Challenge ladders** – ascending problem sets with increasing interleaving of unrelated statutes.

### 🌐 Polyglot Interface
- Full interface localization for **English, Spanish, French, and Bahasa Indonesia** (built-in), with **locale templates** for community contributions.
- Legal terminology glossaries embedded per language to keep translations accurate — not just literal.

### 📱 Responsive First
- **Absolute mobile-first architecture** – works flawlessly at 320px width; no horizontal scrolling, no tiny touch targets.
- **Desktop companion mode** – the same experience expands gracefully for large screens, with keyboard shortcuts for power users.
- **Offline-first PWA** – full functionality without connectivity; syncs when you're back online.

### 🛡️ Governance & Trust
- **24/7 expert review loop** – a rotating roster of licensed attorneys vets every question for accuracy, bias, and jurisdictional relevance.
- **Audit trail** – every question edit, deletion, or translation is logged with timestamp and reviewer ID, ensuring full traceability.
- **Compliance sandbox** – test your knowledge against artificially redacted versions of statutes to simulate real-world ambiguity.

---

## 🗂️ Repository Anatomy

```
verdantcode/
├── app/
│   ├── core/               # adaptive engine, scheduling logic
│   ├── ui/                 # theme tokens, component library
│   ├── i18n/               # language pack structure
│   └── workers/            # background sync, notification timers
│
├── questions/
│   ├── mfa-legislation/    # first question bank (primary)
│   ├── data-privacy/       # in progress
│   └── employment-law/     # in progress
│
├── docs/
│   ├── content-guidelines.md
│   ├── translation-style.md
│   └── difficulty-curves.md
│
└── tools/
    ├── validator.js        # format checker for question banks
    └── migration-cli.js    # schema updater
```

---

## 🚀 Market Readiness

This isn't a toy repository. The architecture anticipates:

- **Corporate onboarding pipelines** – HR teams can deploy a white-labeled instance for new hires in compliance-heavy roles.
- **Law school preparatory courses** – professors can import custom question banks and monitor class-wide mastery metrics.
- **Government training modules** – civil servants can access jurisdiction-specific banks curated by ministry experts.

---

## 🧩 Question Bank Specifications (v1 Schema)

Every bank follows a strict JSON structure:

```json
{
  "id": "mfa-001",
  "jurisdiction": "EU-UK",
  "topic": "Anti-Money Laundering Directives",
  "level": 2,
  "question": "Under the 5th AMLD, which entity must register beneficial ownership information...",
  "answer": "The central registry",
  "distractors": ["Local police unit", "Private bank", "Notary office"],
  "confidence_weight": 0.8,
  "tags": ["registry", "transparency", "directive"]
}
```

**Validation rules** enforced by the built-in tooling:
- No more than 4 distractors per question.
- Distractors must be plausible but clearly distinct.
- At least 20 questions per module to activate adaptive mode.
- Metadata (jurisdiction, year, source statute) required for every entry.

---

## 📊 Analytics & Progress Metrics

The engine emits anonymized telemetry:
- **Retention decay curves** – visualized per module over time.
- **Weak-topic heatmaps** – show which areas of the statute trigger most misses.
- **Session rhythm analysis** – recommends ideal practice times based on your historical engagement patterns.

These metrics feed back into the question bank itself, auto-flagging questions that produce consistently low recall rates for human review.

---

## 🧑‍💻 Contribution Pathways

We welcome three archetypes of contributors:

1. **Legal Scholar** – write new question banks or improve existing ones. Requires passing a simple formatting review.
2. **Polyglot Translator** – provide idiomatic translations, not literal. The system supports fuzzy matching to verify translation consistency.
3. **Systems Tinkerer** – improve the engine's spacing logic or frontend responsiveness.

> Every merged contribution unlocks **repository contributor status** and appears in the hall-of-fame log automatically.

---

## 🔧 Customization & Extensibility

- **Pluginable evaluators** – plug in different scoring algorithms (e.g., partial credit, penalty-based) via a simple interface.
- **Custom branding panel** – swap colors, fonts, and logo from a config file; no code changes needed.
- **API-first design** – all data engines expose REST endpoints for third-party integration.

---

## ⚠️ Disclaimer

**VerdantCode** is a pedagogical tool designed for *training and recall reinforcement*. It **does not constitute legal advice**, does not replace consultation with a qualified attorney, and does not guarantee exam passage or professional certification.  

Statutes change; the question bank is regularly updated, but the maintainers accept **no liability** for outdated information or misinterpretation caused by the learning material. Always verify critical legal decisions against the primary source and current jurisdiction.

The software is provided "as is" under the MIT License, without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement.

---

## 📜 License

This project is licensed under the **MIT License** – see the [LICENSE](./LICENSE) file for full text. 

In essence: use it, modify it, distribute it, even commercially, but **preserve the copyright notice** and **do not hold the authors liable** for any outcomes.

---

## 🗓️ Versioning & Roadmap (2026 Focus)

| Quarter | Milestone |
|---------|-----------|
| **Q1 2026** | Public beta release; MFA bank v1.0 finalized |
| **Q2 2026** | Data-privacy bank (GDPR); desktop companion launch |
| **Q3 2026** | Community translation portal; white-label API |
| **Q4 2026** | Certification engine (generate completion certificates) |

Backward compatibility is guaranteed for all banks written to the v1 schema.

---

## 💬 Support & Community

- **Documentation**: Extended guides in `docs/` folder cover question writing guidelines, translation workflows, and engine tuning.
- **Issue tracker**: Use labeled issues (`bug`, `enhancement`, `question-bank`, `translation`) for efficient triage.
- **Discussion forums**: Architectural debates belong here; support queries get faster answers in the tracker.
- **24/7 pulse checks**: Automated bot monitors the repo for unanswered issues and pings maintainers across time zones.

---

## 🎇 Final Thought

You don't learn a statute by reading it forty times. You learn it by *recalling* it forty times — with the right feedback loop and timing.

VerdantCode gives you that feedback loop. The rest is your own persistence.

---

*Project generation year: 2026. Maintained with a long-term vision for legal education accessibility in emerging regulatory environments.*