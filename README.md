![KNEEAI — bespoke brushed-metal project artwork](./assets/readme-metal-hero.svg)

# KNEEAI

**A small, local-first wellness journal for tracking knee discomfort and preparing gentle movement sessions.**

KneeAI is a static HTML, CSS, and JavaScript prototype. It lets a user record a pain score, note mobility and swelling, save an optional note, view a short history, and select a predefined set of gentle exercises. The entries are stored in the browser using `localStorage`.

## The daily loop

```text
Record today's check
        │
        ├── Pain score (0–10)
        ├── Mobility / swelling selections
        └── Optional note
                │
                ▼
       Browser localStorage
                │
                ▼
Recent history + simple trend view
                │
                ▼
Select exercises for a gentle session
```

## What is implemented

- **Check-in log:** Saves a timestamp, pain score, mobility and swelling selections, and optional note.
- **Recent trend:** Calculates a simple average from recent saved entries and draws a small visual history.
- **Session builder:** Lets the user select predefined exercise prompts and totals their estimated duration.
- **Local persistence:** Uses browser storage; records remain in that browser profile and are not a synced medical record.

## Run locally

No dependency installation or build step is required.

Open `index.html` directly, or serve the repository root:

```bash
python -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000).

## Safety and privacy boundary

**KneeAI is not a diagnostic tool, treatment plan, or substitute for medical advice.** The trend is a basic summary of user-entered values, not a clinical inference. The exercise list is illustrative; stop any movement that worsens symptoms and seek appropriate professional care for concerning or persistent symptoms. Do not rely on the app for injury triage.

Because data is held in `localStorage`, it can be lost when browser storage is cleared and may be accessible to other people using the same browser profile. Avoid entering information you would not want stored on that device.

---

<p align="center"><sub>DIU FOUNDRY · WELLNESS INTERFACE / LOCAL-FIRST PRODUCT EXPLORATION</sub></p>
