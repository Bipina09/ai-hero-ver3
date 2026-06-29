# 🤖 AI Hero's Journey — Teacher Edition
### Browser-Based Educational Game · No Installation Required

---

## 📁 Files

```
ai-hero/
├── index.html   ← The entire game (open this!)
└── README.md    ← This file
```

Everything is in a single file — HTML + CSS + JavaScript, no frameworks, no dependencies.

---

## 🚀 How to Run in VS Code

### Option A — Live Server (Recommended, 30 seconds)

1. Open **VS Code**
2. Press `Ctrl+Shift+X` → search **"Live Server"** → click **Install** (by Ritwick Dey)
3. `File → Open Folder` → select the `ai-hero` folder
4. Right-click `index.html` → **"Open with Live Server"**
5. Game opens automatically at `http://127.0.0.1:5500` ✅

### Option B — Python (if you have Python installed)

```bash
cd path/to/ai-hero
python -m http.server 8080
```
Then open: `http://localhost:8080`

### Option C — Node.js

```bash
npm install -g http-server
cd path/to/ai-hero
http-server -p 8080
```
Then open: `http://localhost:8080`

> ⚠️ Do NOT open index.html by double-clicking — audio and some features need a local server.

---

## 🌐 Internet Requirement

The game loads **Google Fonts** (Nunito + Fredoka One) on first launch.
All game logic works **100% offline** after fonts are cached.

**To make fully offline:**
Add this inside `<head>` to use system fonts instead:
```html
<!-- Remove the Google Fonts <link> tag and add: -->
<style>
  :root { --font: system-ui, sans-serif; --head: Impact, sans-serif; }
</style>
```

---

## 🎮 The 5 Missions

| # | Location | Mechanic | Learning Outcome |
|---|----------|----------|-----------------|
| 1 | 🏫 School | **Drag & Sort** — AI vs Not AI | Identify what AI actually is |
| 2 | 🎨 Creative Studio | **Match** scenarios to AI tools | Choose the right AI tool for classroom tasks |
| 3 | ✍️ Prompt Workshop | **Build** a COSTAR prompt by dragging components | Write effective AI prompts |
| 4 | 🔬 AI Lab | **Scan + Match** mystery clues to prompt quality | Understand how prompt quality affects results |
| 5 | 🛡️ Safety Center | **Click** falling good practices (arcade-style) | Identify responsible AI behaviors |

---

## 🏆 Celebration Levels

| Stars Earned | Rank |
|---|---|
| 93–100% | 🏆 AI Champion |
| 76–92% | 🚀 AI Explorer |
| 56–75% | ⭐ AI Practitioner |
| Below 56% | 🌱 Keep Exploring |

---

## ✨ Features

- ✅ Zero dependencies — pure HTML/CSS/JS
- ✅ Web Audio API sound effects (no audio files needed)
- ✅ Confetti animation on mission complete
- ✅ Animated starfield background
- ✅ Drag-and-drop with mouse AND touch support
- ✅ Local progress saving (localStorage)
- ✅ Sound toggle (mute/unmute)
- ✅ Celebratory finish page
- ✅ Mobile responsive
- ✅ All 5 missions in one file (~900 lines)

---

## 🖥️ Browser Support

Chrome ✅ · Firefox ✅ · Edge ✅ · Safari ✅ (latest versions)

---

## 🔧 Customisation Tips

**Change player avatar:** Find `.player-avatar` in CSS — swap the emoji.

**Add more sorting items (Mission 1):** Find the `items` array in `buildMission1()` and add:
```js
{id:'myitem', label:'My Item', icon:'🎯', isAI:true, reason:'Explanation here'}
```

**Adjust Safety Center speed:** In `buildMission5()`, change `speed=8000` (lower = faster).

**Change celebration text:** In `showCelebration()`, adjust the message and stats shown on the final page.

---

Made with ❤️ for AI-literate educators
