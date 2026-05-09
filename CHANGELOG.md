# Changelog

All notable changes documented here. Format: [Semantic Versioning](https://semver.org/)

---

## [3.0.0] — 2026-05-09

### 🎯 Major: Multi-Model Offline AI

#### Added
- **3 offline AI models** selectable at runtime in ⚙️ Settings:
  - SmolLM2 360M — WASM, any browser, ~220MB
  - Qwen2.5 0.5B — WebGPU, Chrome + GPU, ~400MB
  - Phi-3 Mini — WebLLM, Chrome + GPU, ~2.4GB
- **WebGPU support** via WebLLM for Phi-3 Mini (near GPT-3.5 quality)
- **WebGPU detection** — warns if browser doesn't support it before attempting load
- **Model download progress overlay** — full-screen bar with file name and %
- **Engine tag** on every message — small `☁️ Gemini` or `📴 Local AI` badge
- **Live mode badge** in navbar — updates in real time as connectivity changes
- **Auto mode** — uses Gemini when online, falls back to local AI automatically
- Real error messages from `pipeline()` — no more silent `undefined` errors

#### Changed
- Upgraded Transformers.js: `@xenova/transformers` v2 → `@huggingface/transformers` **v3.8.1**
- Model IDs updated to `onnx-community` namespace (public, no HF login)
- Offline inference: switched to `do_sample: false` (greedy) for better coherence
- Added `return_full_text: false` to prevent prompt echo in output
- Special token cleanup (`<|endoftext|>`, role prefix stripping)
- SmolLM2 upgraded from 135M → 360M for coherent answers
- No more silent auto-load — clear setup instructions shown instead

#### Fixed
- `Cannot set properties of null (setting 'value')` — settings panel HTML was truncated
- `undefined` error message — proper `err.toString()` fallback
- "IQTORALANEX" garbage output — model too small + wrong output parsing

---

## [2.0.0] — 2026-05-01

### 🎨 Major Redesign + Offline AI v1

#### Added
- Complete UI overhaul — SCA-inspired white/navy/lime design system
- Floating pill navbar with lime green active state
- Barlow Condensed 900 ALL-CAPS section headers
- Basic offline AI via Transformers.js (Flan-T5 — later replaced)
- Auto-learn memory extraction from every conversation
- Voice language selector (8 languages)
- Timestamp on message hover
- Hint chips in chat input bar

#### Changed
- Model list updated to Gemini 2.5 family
- Improved system prompt with stronger personality constraints

---

## [1.0.0] — 2026-04-15

### 🎉 Initial Release

- Single-file Gemini-powered chat app
- localStorage persistence for chat, memory, tasks
- Voice input (SpeechRecognition API)
- Text-to-speech output
- Task manager with priority + due date
- Manual memory key-value store
- Dark amber theme
