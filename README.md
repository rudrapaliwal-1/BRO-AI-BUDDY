# 🤖 Bro — Free AI Buddy

> A smart, single-file AI chat app powered by Google Gemini. No server. No backend. No subscription. Just drop the HTML file anywhere and go.

<img width="1280" height="640" alt="image" src="https://github.com/user-attachments/assets/4790758d-fa13-47dc-a667-2175d2b4195f" />


---

## ✨ What is Bro?

**Bro** is a 100% free, single-file AI chat application that runs entirely in your browser. It uses Google's **Gemini API** (free tier — no credit card required) and stores everything locally — your chat history, memory, and tasks never leave your device.

Built with love by one person. No VC funding. No paywalls

---

## 🚀 Live Demo

https://amazing-dolphin-157033.netlify.app/

Or host it instantly:
- **GitHub Pages** — push this repo and enable Pages → done
- **Netlify Drop** — drag the folder to [netlify.com/drop](https://netlify.com/drop)
- **Vercel** — `vercel --prod` in this folder

---

## 🎯 Features

| Feature | Details |
|---|---|
| 💬 **AI Chat** | Powered by Gemini 2.5 Flash — fast, smart, free |
| 🧠 **Memory** | Bro learns from your chats and remembers you |
| ✅ **Tasks** | Priority-sorted to-do list with due dates |
| 🎤 **Voice Input** | Speak your messages (Chrome) |
| 🔊 **Text-to-Speech** | Bro reads replies aloud |
| 🌍 **Multilingual Voice** | Hindi, Tamil, Telugu, Marathi, Bengali + more |
| 📴 **Offline-first** | All data in localStorage — works without internet once loaded |
| 🔒 **Private** | Your API key never touches any server except Google's |
| 📱 **Mobile Ready** | Responsive, works as a PWA |

---

## 🔑 Getting Your Free API Key

1. Go to [aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)
2. Sign in with your Google account
3. Click **"Create API key"**
4. Copy the key (starts with `AIzaSy...`)
5. Open Bro → **⚙️ Settings** → paste the key

**Free tier limits:**
- `gemini-2.5-flash` → 250 requests/day
- `gemini-2.5-flash-lite` → 1,000 requests/day
- `gemini-2.5-pro` → 100 requests/day

---

## 📁 File Structure

```
bro/
├── index.html          ← The entire app (single file, self-contained)
├── README.md           ← This file
├── LICENSE             ← MIT License
├── .gitignore          ← Standard web .gitignore
└── assets/
    ├── banner.png      ← Social preview image
    └── screenshot.png  ← App screenshot
```

---

## 🛠️ Tech Stack

| Layer | Tech |
|---|---|
| Frontend | Vanilla HTML, CSS, JavaScript |
| AI | Google Gemini API (REST) |
| Storage | Browser localStorage |
| Fonts | Barlow Condensed + Barlow (Google Fonts) |
| Voice | Web Speech API (SpeechRecognition + SpeechSynthesis) |
| Hosting | Any static host |

Zero dependencies. Zero build step. Zero backend.

---

## 🎨 Design

Bro's UI is inspired by clean corporate design systems — white backgrounds, deep navy, and a sharp lime green accent. The floating pill navbar, condensed ALL-CAPS headings, and horizontal-rule section labels give it a polished, professional feel that's unlike typical "AI chatbot" aesthetics.

- **Font:** Barlow Condensed 900 (headers) + Barlow 400/600 (body)
- **Colors:** `#f4f5f7` bg · `#0d2137` navy · `#8dc63f` lime
- **Layout:** Floating pill nav · accordion rows · pill CTAs

---

## 🧠 How Memory Works

Bro automatically extracts facts from your conversations using a secondary Gemini call:

```
User: "I'm studying DSA for my IGDTUW exams"
→ Bro saves: { college: "IGDTUW", study_subject: "DSA" }
```

These facts are silently injected into every future conversation so Bro always knows who you are. You can view, add, or delete memories from the **🧠 Memory** tab.

---

## 🤖 Bro's Personality

Bro is configured with a system prompt that makes him:
- Talk like a **smart friend** — direct, honest, occasionally funny
- Keep replies **short by default** (long answers only if you ask)
- **Never** say "Certainly!", "Absolutely!", "Great question!" (ugh)
- Acknowledge your **stress** before diving into solutions
- Call out bad ideas: *"bro that's a bad idea because..."*

---

## ⚙️ Configuration

All config is stored in `localStorage`. Keys:

| Key | Description |
|---|---|
| `bro_gkey` | Your Gemini API key |
| `bro_msgs` | Chat history (last 120 messages) |
| `bro_mem` | Memory key-value store |
| `bro_tasks` | Task list (JSON array) |
| `bro_cfg` | Settings (model, language) |

To reset everything: **⚙️ Settings → Reset Everything**

---

## 🚢 Deploying to GitHub Pages

```bash
# 1. Fork or clone this repo
git clone https://github.com/YOUR_USERNAME/bro.git
cd bro

# 2. Push to GitHub
git add .
git commit -m "🤖 Deploy Bro"
git push origin main

# 3. Enable GitHub Pages
# Go to repo Settings → Pages → Source: main branch → / (root)
# Your app will be live at: https://YOUR_USERNAME.github.io/bro
```

---

## 📜 License

MIT — do whatever you want with it. If you build something cool, star the repo ⭐

---

## 🙏 Credits

Built with [Google Gemini API](https://ai.google.dev/) — free tier, no credit card required.

---

<p align="center">Made with ☕ and zero budget &nbsp;·&nbsp; <strong>Bro</strong> is open source forever</p>
