# Contributing to Bro 🤖

Thanks for wanting to make Bro better! Since Bro is a single-file app, contributing is super simple.

---

## 🐛 Reporting Bugs

Open an [Issue](../../issues) and include:
- What you expected to happen
- What actually happened
- Browser + OS
- Console errors (F12 → Console tab)

---

## 💡 Suggesting Features

Open an Issue with the `enhancement` label. Describe:
- What problem it solves
- How you'd expect it to work

---

## 🛠️ Making Changes

Since Bro is a single `index.html` file, the workflow is dead simple:

```bash
# 1. Fork the repo on GitHub

# 2. Clone your fork
git clone https://github.com/YOUR_USERNAME/bro.git
cd bro

# 3. Open index.html in your editor
# Make your changes

# 4. Test it — just open index.html in a browser
open index.html

# 5. Commit and push
git add index.html
git commit -m "feat: describe your change"
git push origin main

# 6. Open a Pull Request on GitHub
```

---

## 🎨 Design Principles

Keep these in mind when making UI changes:

- **White / Navy / Lime** — don't introduce new colors
- **Barlow Condensed** for headings, **Barlow** for body — don't change fonts
- **Pill shapes** for CTAs and nav — keep the SCA-inspired aesthetic
- **Mobile first** — test on a 375px viewport
- Keep it a **single file** — no build tools, no npm, no bundlers

---

## 📋 Code Style

- Vanilla JS only — no frameworks
- CSS variables for all colors/spacing (defined in `:root`)
- Keep localStorage keys consistent (see `S` object in the script)
- Comment non-obvious logic

---

## ✅ PR Checklist

- [ ] Tested in Chrome and Firefox
- [ ] Tested on mobile (or DevTools mobile emulation)
- [ ] No new external dependencies added
- [ ] Still a single self-contained HTML file
- [ ] Follows existing naming conventions

---

Thank you! 🙏
