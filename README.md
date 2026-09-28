# KneeAI

> **Move with more awareness.**

KneeAI is a browser-based health-tech prototype built around a simple product idea: make knee wellness more observable through lightweight tracking, gentle planning and clear safety guidance.

This implementation is intentionally **tracking and education oriented**, not diagnostic.

## Product surface

- Daily 0–10 discomfort check
- Mobility and swelling observations
- Local history with up to 60 saved entries
- Seven-entry trend visualization
- Gentle movement-plan builder
- Session duration calculation
- Safety-first guidance and escalation cues
- Responsive desktop/mobile interface
- No account or backend required

## Safety

KneeAI does **not** diagnose conditions or determine the cause of pain. It is not a substitute for a qualified healthcare professional.

Stop an activity that causes significant or escalating pain. Appropriate professional care should be considered for severe pain, major swelling, deformity, inability to bear weight, or an acute injury.

## Architecture

A dependency-free static frontend:

- `index.html` — product structure and metadata
- `style.css` — responsive visual system
- `app.js` — tracking state, trend calculations and movement-session builder
- `favicon.svg` — project mark

Check history is stored in browser `localStorage`. This implementation does not send health observations to an application server.

## Run locally

```bash
git clone https://github.com/Kishordiu/KneeAI.git
cd KneeAI
python -m http.server 8000
```

Open `http://localhost:8000`.

## Roadmap

Future versions can add clinician-reviewed exercise libraries, secure accounts, encrypted sync, wearable integrations, camera/motion analysis and explainable model-assisted insights — with medical validation and privacy controls appropriate to each capability.

## Status

**Major project · Functional wellness MVP**

Built and maintained by **K. Kishor Kumar**.

[GitHub @Kishordiu](https://github.com/Kishordiu)
