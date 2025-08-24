# 🎙️ Transcripto – AI Urdu Audio Assistant

Transcripto is an AI-powered automation that takes **Urdu audio files (MP3)** and processes them into multiple useful outputs:
- Roman Urdu Transcription
- English Translation
- Structured English Summary

It is built with **n8n automation**, **OpenAI models**, and a **custom frontend**, showcasing how AI can bridge linguistic and accessibility gaps.

# Features
- Upload MP3 audio files via frontend
- Automatic Urdu speech-to-text using **GPT-4o-Transcribe**
- Convert Urdu text into **Roman Urdu** using a custom **Transliteration Agent**
- Perform direct Urdu → English translation using **Whisper-1**
- Generate a **structured English summary** with headings and bullet points
- Frontend interface built on **Lovable**, backend orchestrated in **n8n**

# Tech Stack
- n8n (workflow automation)
- OpenAI GPT-4o-Transcribe (speech-to-text)
- OpenAI Whisper-1 (direct Urdu → English translation)
- Custom Transliteration Agent
- Custom Summary Agent
- Lovable (frontend hosting)

# Workflow
- User uploads MP3 → Webhook receives input
- Switch node routes based on user choice:
  - Translation → Urdu audio → English text using **Whisper-1**
  - Transcription → Urdu audio → Urdu text using **GPT-4o-Transcribe**, then converted to **Roman Urdu**
  - Summary → Urdu audio → Urdu text using **GPT-4o-Transcribe**, then summarized into **structured English notes**
- Result returned to frontend for display



⭐ If you like this project, drop a star on the repo!
