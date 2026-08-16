# RapidResQ

RapidResQ is an AI-powered emergency assistance app designed to help people respond faster during critical situations. The platform combines voice and text emergency detection, live GPS location sharing, and AI-guided first-aid support to deliver timely, relevant guidance when every second matters.

## Overview

RapidResQ is built for real-world emergency response scenarios where users may be unable to clearly explain what is happening. By analyzing voice and text inputs, the app can detect possible emergencies and route users to immediate, actionable support.

### Core Features
- Voice-based emergency detection using speech analysis and natural language understanding
- Text-based distress input detection for quick reporting and triage
- AI-powered first-aid recommendations generated through an LLM
- Live GPS location sharing for responders and emergency contacts
- Fast access to emergency guidance during high-stress situations
- Multi-platform app experience with mobile-first design

## Problem We Solve
Many emergency situations require immediate support, but users may be panicked, injured, or unable to communicate clearly. RapidResQ reduces friction by enabling fast detection, contextual analysis, and immediate guidance while making the user’s location available to responders.

## Tech Stack

### Mobile App
- Flutter
- Dart
- On-device speech-to-text (`speech_to_text` package — no API key required)

### Backend and APIs
- Django (Python)
- REST APIs
- SQLite (development database)

### AI and Intelligence
- Google Gemini API (LLM for emergency detection and first-aid guidance)
- Python

### Location and Services
- GPS / device location services
- OpenStreetMap + Leaflet (chosen to avoid Google Maps API's billing requirement)

### DevOps and Collaboration
- GitHub (GitHub Organization: RapidResQ)
- GitHub Actions (CI/CD, planned)
- Team-based agile development

## System Flow
1. User enters an emergency via voice or text.
2. App analyzes the input for urgency and context.
3. Location services capture and share active GPS coordinates.
4. AI backend generates the most relevant first-aid or urgent action guidance.
5. Response flow prioritizes actionable help and communication with emergency contacts or responders.

## Team

| Name | Role | Focus Area |
| --- | --- | --- |
| Nirali | Project Lead | Product direction, AI, APIs, LLM integration |
| Deekshitha | App Development |Flutter frontend, media editing, and user experience |
| Pranjal | Backend and Repo Management | Django, emergency logic, and deployment |
| Rudra | Location & Integration | GPS, maps, and live sharing workflows |

## Repository workflow

This repository follows a simple branch-based workflow so the team can stay organized without making things heavy.

- Keep `main` as the stable branch
- Work on a feature branch for your task
- Open a pull request before merging
- Keep PRs small and easy to review
- Use short, readable branch names

Examples:

- `pranjal-backend`
- `nirali-ai`
- `deekshitha-ui`
- `rudra-location`

The full workflow guidance is in [docs/TEAM_WORKFLOW.md](docs/TEAM_WORKFLOW.md), and the repo includes a simple PR template in [.github/pull_request_template.md](.github/pull_request_template.md).

## Goals
- Build a fast and understandable emergency assistance experience
- Support both voice and text-driven crisis detection
- Deliver relevant first-aid guidance while preserving user safety
- Enable real-time location sharing for emergency response coordination
- Create a scalable foundation for future integrations and expansion

## Getting Started

This project is organized into functional folders for team collaboration:

- `ai/` — LLM integration, emergency detection, and first-aid logic
- `backend/` — server-side logic and APIs
- `app/` — mobile app code
- `location/` — GPS and mapping logic
- `media/` — project assets and visuals
- `docs/` — documentation and project planning
## License
This project is currently under active team development and is intended for collaborative use within the RapidResQ project.
