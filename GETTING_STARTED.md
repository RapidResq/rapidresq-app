# Getting Started — RapidResQ

Welcome to the team! This guide walks you through setting up the project on your computer and starting work on your module.

## 1. Prerequisites

Before you begin, make sure you have installed:
- **Git** — [git-scm.com](https://git-scm.com)
- **VS Code** — [code.visualstudio.com](https://code.visualstudio.com)
- A **GitHub account**, added to the RapidResQ organization

## 2. Clone the repository

1. Go to [github.com/RapidResq/rapidresq-app](https://github.com/RapidResq/rapidresq-app)
2. Click the green **Code** button → copy the HTTPS link
3. Open a terminal on your computer and run:
   ```bash
   git clone https://github.com/RapidResq/rapidresq-app.git
   ```

## 3. Open the project in VS Code

- **File → Open Folder** → select the `rapidresq-app` folder that was just created

## 4. Create your own branch

Never work directly on `main`. Create a branch named `yourname/short-description`:

```bash
git checkout main
git pull
git checkout -b yourname/what-youre-building
```

**Example branch names:**

| Member | Branch |
|---|---|
| Nirali | `nirali/ai-llm` |
| Deekshitha | `deekshitha/mobile-ui` |
| Pranjal | `pranjal/backend-db` |
| Rudra | `rudra/location-gps` |

## 5. Project folder structure

Work inside your assigned folder:

| Folder | Owner | What goes here |
|---|---|---|
| `ai/` | Nirali | LLM integration, emergency-type detection, first-aid response logic, speech-to-text |
| `app/` | Deekshitha | Flutter UI, screens, navigation, TTS, media editing/UX |
| `backend/` | Pranjal | Django backend, emergency classification logic, database (SQLite/Firebase) |
| `location/` | Rudra | Maps, GPS, hospital lookup, SOS, live location sharing |
| `docs/` | Everyone | Documentation — each person's section in their own file |

## 6. Environment variables (API keys)

1. Copy `.env.example` to a new file named `.env`
2. Fill in your own API keys (see table below)
3. **Never commit your `.env` file** — it's already in `.gitignore` to keep keys private

| Key needed | Used for | Free option |
|---|---|---|
| `GEMINI_API_KEY` | LLM emergency analysis | [aistudio.google.com](https://aistudio.google.com) — free, no card |
| — | Maps / GPS | OpenStreetMap + Leaflet — no key needed |
| — | Speech-to-Text | Flutter's `speech_to_text` package — no key needed, runs on-device |

## 7. Save your work

Commit often, with clear messages describing what changed:

```bash
git add .
git commit -m "add GPS location fetching"
git push
```

First time pushing a new branch, Git may ask you to run:
```bash
git push --set-upstream origin yourname/your-branch
```
Just copy-paste that exact line if it appears.

## 8. Open a Pull Request

1. Go to [github.com/RapidResq/rapidresq-app](https://github.com/RapidResq/rapidresq-app)
2. You'll see a banner for your recently pushed branch → click **Compare & pull request**
3. Give it a clear title, then **Create pull request**
4. Once reviewed (or if it's routine setup work), merge it into `main`

## 9. Task tracking

Check the **Issues** tab for your assigned checklist of tasks. Move your card across the **Project board** (To Do → In Progress → In Review → Done) as you make progress.

## Questions?

Ask in the team group chat, or tag a teammate directly on your Pull Request or Issue.
