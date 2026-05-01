# Changelog

All notable changes to Bro are documented here.
Format: [Semantic Versioning](https://semver.org/)

---

## [2.0.0] — 2026-05-01

### 🎨 Major Redesign
- Complete UI overhaul — white/navy/lime design system (SCA-inspired)
- Floating pill navbar with lime green active state
- Barlow Condensed 900 ALL-CAPS section headers
- Accordion-style row lists for Tasks and Memory
- SCA-style horizontal rule section labels in Settings
- Arrow circle buttons throughout

### ✨ Added
- Auto-learn memory extraction from every conversation
- Voice language selector (8 Indian + global languages)
- Timestamp on message hover
- Hint chips in chat input bar
- Animated typing indicator with lime dots
- Status dot with glow animation for API key validation

### 🔧 Changed
- Model list updated to Gemini 2.5 family
- Improved system prompt — Bro now has stronger personality constraints
- Chat history trimmed to last 120 messages (was 80)
- Task list now uses horizontal accordion rows (was card grid)

---

## [1.0.0] — 2026-04-15

### 🎉 Initial Release
- Single-file Gemini-powered chat app
- localStorage persistence for chat, memory, tasks
- Voice input (SpeechRecognition API)
- Text-to-speech output
- Task manager with priority + due date
- Manual memory key-value store
- Dark theme with amber accent
- Gemini 2.5 Flash support

---
