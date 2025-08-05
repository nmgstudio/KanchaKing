# KanchaKing

**Goliyaan** एक HTML/CSS/JS आधारित 2-4 प्लेयर ऑनलाइन/ऑफलाइन गेम है, जो भारत के पारंपरिक "कंचे" गेम पर आधारित है। इसमें खिलाड़ी जमीन जैसी सतह पर कंचों को निशाना बनाकर, रणनीति के साथ अंठी से मुर्ह को मारते हैं, बिना दाव को हिलाए।

---

## 🎯 Objective

- अंठी (main marble) से मुर्ह (target marbles) को मारो।
- दाव (forbidden marbles) को हिलाए बिना टारगेट्स को हिट करो।
- सबसे ज्यादा कंचे जीतकर राउंड विन करो।

---

## 🚀 Features

- 🎮 Multiplayer (2 to 4 players)
- 🧠 Realistic Indian physics and gameplay logic
- 📱 Mobile & Desktop responsive
- 🌍 Offline + Online modes
- 🔄 Turn-based gameplay with indicators
- 🎯 Drag-Aim-Release UI mechanics
- 📊 Live scoreboard with round tracking
- ⏱️ Timer and Power bar controls
- 🎨 Indian dirt-ground background and audio fx

---

## 🧱 Tech Stack

- HTML5
- CSS3 (Tailwind or Custom)
- JavaScript (Vanilla)
- GSAP (for animations)
- Optional: LocalStorage for offline score memory

---

## 📁 Folder Structure

Goliyaan_Game_HTML/
│
├── index.html                   🏠 Home/Landing Page
├── instructions.html            📜 How to Play + Rules
├── game.html                    🕹️ Main Game Screen
├── lobby.html                   👥 Multiplayer Lobby
├── settings.html                ⚙️ Game Settings
├── scoreboard.html              🏆 Live Scoreboard
├── game-over.html               🔚 Game Over & Summary
│
├── assets/
│   ├── images/
│   │   ├── logo.png
│   │   ├── background-dirt.jpg
│   │   ├── marble-red.png
│   │   ├── marble-blue.png
│   │   ├── pointer.png
│   │   └── line-marker.png
│   │
│   └── sounds/
│       ├── shoot.mp3
│       ├── hit.mp3
│       └── background-music.mp3
│
├── css/
│   ├── style.css                🎨 Global Styles
│   ├── lobby.css
│   ├── game.css
│   └── responsive.css           📱 For mobile/tablets
│
├── js/
│   ├── main.js                  🚀 Entry point, handles routing or init
│   ├── game.js                  🎮 Core game logic (marble physics, collisions)
│   ├── ui.js                    🧩 UI Interactions (buttons, popups, sliders)
│   ├── multiplayer.js           🌐 Lobby and WebSocket-based logic
│   ├── scoreboard.js            📊 Score tracking and UI updates
│   └── utils.js                 🛠️ Helper functions (distance check, etc.)
│
├── data/
│   └── players.json             🧍 Local multiplayer user data (name, color, marbles)
│
├── fonts/
│   └── desi-style.ttf           🔤 Game theme font (Hindi/Marble inspired)
│
└── README.md                    📘 Project Setup Instructions

---

## 📄 Pages & Buttons

| Page              | Buttons / Actions                             |
|-------------------|-----------------------------------------------|
| `index.html`      | ▶ Start Game, ℹ Rules, 👤 About               |
| `game.html`       | 🎯 Aim, 🔄 Reset Turn, ⏭ Next Player, 📋 Score |
| `rules.html`      | ⬅ Back, 🎮 Play Now                           |
| `scoreboard.html` | 🏆 View Stats, 🔁 Play Again, 🏠 Home          |
| `about.html`      | ⬅ Back to Home                               |

---

## 🧩 Gameplay Flow

1. **Select Players** → 2 to 4
2. **Place Marbles** → Random or Manual via drag
3. **Turn Begins** → Select अंठी → Aim at मुर्ह
4. **Hit or Miss** → If दाव is hit, turn fails
5. **Next Turn** → Player changes
6. **Round Ends** → When all muṛh are cleared
7. **Score Displayed** → Game ends or restarts

---

## 🧠 Game Logic Highlights

- A marble can be selected only as अंठी (active marble).
- दाव (protected) cannot be moved or hit.
- Score is added only when मुर्ह is hit without touching दाव.
- 10 rounds = 1 Match (default setting)

---

## 📦 Installation / Usage

1. Download the repo or clone:
   ```bash
   git clone https://github.com/yourname/goliyaan.git
2. Open index.html in your browser.
3. No server needed — works fully offline!

## Credits
Concept: Inspired by traditional Indian marble game.
Visuals: Captured from real-life gameplay.
Dev: [Your Name], [Your Team or Org]
Special Thanks: Rural gamers of India 🇮🇳
