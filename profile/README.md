# Vura Labs | The Cognitive Operating System

**Zero-Friction Cognitive Offloading.**  
Vura Labs is building tools that help people instantly unload thoughts, worries, schedules, and ideas — then trust the system to organize everything.

## What We’re Building

### Aura (Consumer Edition)
A minimal mobile app for thought capture:

- Hold one button (or use home-screen widget)
- Speak naturally
- Release
- Done

Aura automatically understands intent and routes your input to the right destination (tasks, journal, expense, notes).

## Why This Matters

Most productivity apps create more friction than value.  
Aura is designed for **speed, trust, and mental clarity** — like a brain inbox that actually works.

## Product Principles

- **Capture in seconds**
- **No form fatigue**
- **Intelligence over manual sorting**
- **Quiet UX, powerful backend**

## Core Intent Types

Aura classifies voice input into:

- `TASK` — reminders, todos
- `JOURNAL` — daily reflections, emotions
- `EXPENSE` — spending and purchases
- `NOTE` — ideas and quick thoughts

## High-Level Architecture

- **Mobile:** React Native (Expo)
- **Backend:** Go (Fiber/Gin)
- **Database:** Supabase (PostgreSQL + pgvector-ready)
- **Speech-to-Text:** Groq Whisper API
- **Intent Router:** Claude / GPT with strict JSON routing

Pipeline:

1. Record audio on app
2. Upload `.m4a` to Go backend
3. Transcribe with Groq Whisper
4. Route intents with LLM
5. Store structured outputs in Supabase
6. Return confirmation + optional push feedback

## Status

🚧 Early build phase  
We are shaping Aura into the default cognitive capture layer for everyday life.

## Vision

To become the default app on billions of home screens —  
a place where people can “throw” every thought in, and know it will be handled.

---

**Vura Labs**  
Building the interface between human thought and calm execution.