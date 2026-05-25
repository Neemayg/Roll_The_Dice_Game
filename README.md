# 🎲 Roll The Dice Game

A fun, two-player browser-based dice game built with vanilla HTML, CSS, and JavaScript. Race against your opponent to be the first player to reach **100 points**!

---

## 📸 Preview

> Open `index.html` in your browser to play instantly — no setup required!

---

## 🎮 How to Play

The game is played between **two players**, taking turns:

1. **Roll the Dice 🎲** — Click the "Roll dice" button to roll a random dice (1–6).
   - The rolled number is added to your **Current Score**.
   - If you roll a **1**, you lose your entire current score and it becomes the other player's turn.

2. **Hold 📥** — Click the "Hold" button to **bank your current score** into your total score and pass the turn to the other player.

3. **Win 🏆** — The first player to reach a **total score of 100 or more** wins the game!

4. **New Game 🔄** — Click "New Game" at any time to reset everything and start fresh.

---

## ✨ Features

- 🎲 Random dice roll with realistic dice face images (1–6)
- 👥 Two-player turn-based gameplay
- 📊 Tracks both **current round score** and **total score** per player
- ⚡ Active player highlight for clear turn indication
- 🏆 Winner announcement with visual styling
- 🔄 Instant game reset with the "New Game" button
- 🎨 Glassmorphism UI with a vibrant gradient background

---

## 🗂️ Project Structure

```
Roll_The_Dice_Game/
│
├── index.html          # Game layout and structure
├── index.css           # Styling and visual design
├── index.js            # Game logic (rolling, holding, switching, winning)
│
└── Photos_Dice/        # Dice face images
    ├── dice-1.png
    ├── dice-2.png
    ├── dice-3.png
    ├── dice-4.png
    ├── dice-5.png
    └── dice-6.png
```

---

## 🚀 Getting Started

### Prerequisites
No libraries or frameworks needed. Just a modern web browser!

### Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Neemayg/Roll_The_Dice_Game.git
   ```

2. **Navigate into the project directory:**
   ```bash
   cd Roll_The_Dice_Game
   ```

3. **Open the game:**
   - Simply open `index.html` in your browser, OR
   - Use a local development server (e.g., VS Code's **Live Server** extension) for the best experience.

---

## 🛠️ Built With

| Technology | Purpose |
|---|---|
| **HTML5** | Game structure & layout |
| **CSS3** | Styling, glassmorphism, gradients |
| **Vanilla JavaScript** | Game logic & DOM manipulation |

---

## 🧠 Game Logic Overview

```
Roll Dice
   ├── dice === 1  →  currentScore = 0, switch player
   └── dice !== 1  →  currentScore += dice

Hold
   ├── totalScore[activePlayer] += currentScore
   ├── totalScore >= 100  →  🏆 PLAYER WINS
   └── totalScore < 100   →  switch player

New Game  →  Reset all scores & state
```

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 👤 Author

**Neemayg**  
GitHub: [@Neemayg](https://github.com/Neemayg)

---

> _"Fortune favors the bold — but holding at the right time wins the game!"_ 🎲
