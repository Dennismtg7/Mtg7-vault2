# 🪨 Stone Pit – Chain Capture

A strategic two-player board game with chain mechanics, AI opponent, and online multiplayer. Built with pure HTML, CSS, and JavaScript.

![Game Screenshot](https://via.placeholder.com/800x400?text=Stone+Pit+Gameplay) 

## 🎮 Play Now

You can play the game directly in your browser:  
👉 **[Launch Stone Pit Game](./game.html)** (clone and open `game.html`)



 ✨ Features

- 3 Game Modes
  - 👥 **2 Players** – Pass & play on the same device
  - 🤖 **vs AI** – 3 difficulty levels (Easy / Medium / Hard)
  - 🌐 **Online Multiplayer** – Play with a friend anywhere using PeerJS (room code system)

- **Unique Chain Capture Mechanics**
  - Sow stones like Mancala, but with chain reactions
  - Land on an empty **inner pit** → capture opponent's entire column if their inner pit has stones
  - Land on an empty **outer pit** → turn ends immediately

- **Visual & Audio Feedback**
  - Glowing pits for valid moves
  - Stone-by-stone sowing animation
  - Capture shake effects and color-coded stones
  - Toast notifications for game events

- **Fully Responsive** – Works on desktop, tablet, and mobile (touch-optimized)

---

## 🕹️ How to Play

### Objective
Capture more stones than your opponent by landing on empty inner pits and stealing their column.

### Turn Flow
1. Click on any of your **glowing pits** (pits with stones).
2. Pick up all stones from that pit and sow them **clockwise** into subsequent pits (one stone per pit).
3. **If the last stone lands in a pit that already had stones** → you trigger a **chain**: pick up all stones from that pit and keep sowing.
4. **If the last stone lands in an empty INNER pit**:
   - Check the opponent's inner pit in the **same column**.
   - If it contains stones → you capture **both** pits in that column (inner + outer) and add them to your score.
   - Turn ends.
5. **If the last stone lands in an empty OUTER pit** → turn ends immediately (no capture).

### Game End
When a player runs out of stones in all their pits, the game ends. The player with the higher score wins.

---

## 🚀 Running Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/Dennismtg7/Mtg7-vault2.git
   cd Mtg7-vault2
