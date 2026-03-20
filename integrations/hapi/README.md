# HAPI

Voice interface combining speech-to-text (STT) and text-to-speech (TTS) for voice-based AI interaction.

## Requirements

- STT service (e.g., Whisper, Deepgram)
- TTS service (e.g., ElevenLabs, OpenAI TTS)
- Audio input/output device

## Setup

1. Choose and configure STT and TTS providers
2. Store API keys in your credential vault
3. Set up the voice pipeline: microphone → STT → AI → TTS → speaker
4. Configure wake word or push-to-talk activation

## Pipeline

```
Microphone → STT (speech to text) → AI Agent → TTS (text to speech) → Speaker
```

## Use Cases

- Hands-free AI interaction while cooking, driving, etc.
- Voice-based task creation and queries
- Accessibility interface for the AI agent
- Quick lookups without opening a terminal
