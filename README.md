# CivicMind AI

CivicMind AI is an autonomous multi-agent civic operating system. Citizens upload an image, video, or voice note; the system detects the issue, maps it, verifies it, prioritizes it, routes it to the right authority, coordinates citizens, predicts future hotspots, and measures civic impact.

## What This Demo Includes

- Premium responsive React operations cockpit with dark mode visuals, animated issue cards, map simulation, ward health index, agent timeline, upload intake, dashboards, and leaderboard.
- Express backend exposing production-shaped API endpoints for media intake, agent orchestration, issue tracking, insights, confirmations, and escalation.
- Mock Gemini Vision, Google Maps, verification, priority, routing, prediction, communication, and impact agents with deterministic structured output.
- Finals-ready documentation: architecture, agent communication diagram, database schema, API, deployment plan, pitch deck, judge explanation, and demo script.

## Quick Start

```bash
npm install
npm run dev
```

Open the client at `http://localhost:5173`. The API runs at `http://localhost:8080`.

If PowerShell blocks `npm`, use:

```bash
npm.cmd install
npm.cmd run dev
```

## Demo Flow

1. Drop any image, video, or voice file into the intake panel.
2. Click **Run AI Civic Pipeline**.
3. Watch nine agents produce a verified, routed, prioritized civic case.
4. Inspect the map, urgent issue queue, ward health index, predicted hotspots, and government performance dashboard.

## Google Cloud Production Mapping

- Gemini API / Vertex AI: vision detection, reasoning, multilingual communication, action plans.
- Google Maps Platform: geocoding, ward lookup, nearby landmarks, schools, hospitals, traffic context.
- Firebase Auth: citizen and official identities.
- Firestore: issues, reports, votes, departments, wards, escalations, predictions.
- Cloud Storage: citizen media, before/after photos, time-lapse proof.
- Cloud Run: agent orchestration API.
- Pub/Sub + Cloud Tasks: async agent events, reminders, escalation follow-ups.
- Speech-to-Text / Text-to-Speech / Translation: voice and multilingual channels.
- Document AI: formatted municipal letters, work orders, and compliance reports.

## Project Structure

```text
civicmind-ai/
  src/                 React frontend
  server/              Express API and agent pipeline
  docs/                Finals documentation and pitch assets
  .env.example         Deployment configuration template
```

## Important Docs

- [Architecture](docs/ARCHITECTURE.md)
- [Agent Communication Diagram](docs/AGENT_COMMUNICATION.md)
- [Database Schema](docs/DATABASE.md)
- [API](docs/API.md)
- [Deployment](https://0fb6e5ef9053ee.lhr.life/)
- [Pitch Deck](docs/PITCH_DECK.md)
- [Judge Explanation](docs/JUDGE_EXPLANATION.md)
- [Demo Script](docs/DEMO_SCRIPT.md)

## Production Notes

This repository is intentionally runnable without paid cloud keys. The mock services in `server/services` mirror the shape of Gemini, Maps, Firestore, and communication adapters so they can be replaced incrementally with real Google Cloud clients.
