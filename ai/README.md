# AI Module

This folder handles the AI/LLM layer of RapidResQ.

## What's here
- Integration with Google Gemini API for emergency-type detection and analysis
- First-aid response logic based on detected emergency type
- Speech-to-text handling (via Flutter's on-device `speech_to_text` package, called from here for processing logic)

## Tech
- Google Gemini API (free tier via aistudio.google.com — no card required)
- Python (for any standalone processing/prompt logic, if applicable)

## Setup
- Requires `GEMINI_API_KEY` in your `.env` file (see root `.env.example`)
