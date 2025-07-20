# 🏎️ Mario Kart Race Simulator

A fun, turn-based console simulation of a Mario Kart-style race, written entirely in JavaScript! Two characters — Mario and Luigi — face off in a 5-round challenge involving straightaways, curves, and direct confrontations. Dice rolls, character stats, and a bit of luck determine who crosses the finish line victorious.

## 🎮 Features

* 🎲 Dice-based random events
* 🚧 Random track blocks: **STRAIGHT**, **CURVE**, or **CONFRONTATION**
* 🧠 Different stats for each character: speed, maneuverability, and power
* ⚔️ Combat events that reduce points
* 🏆 Points system and automatic winner declaration
* 🧪 Fully asynchronous game engine using `async/await`

## 🧱 Project Structure

```
project-root/
└── index.js   # All game logic is contained here
```

## 👾 Characters

### Mario

* Speed: 4
* Maneuverability: 3
* Power: 3

### Luigi

* Speed: 3
* Maneuverability: 4
* Power: 4

Each character starts with 0 points. They earn points by winning challenges and lose them during confrontations.

## 🧠 How It Works

1. The race lasts **5 rounds**.
2. Each round randomly draws a **track block**:

   * `RETA` (Straight): Speed is tested
   * `CURVA` (Curve): Maneuverability is tested
   * `CONFRONTO` (Confrontation): Power is tested in a duel
3. Each player rolls a die (1–6) and adds the result to their relevant stat.
4. The highest total earns 1 point.
5. In confrontations, the loser may lose a point.
6. At the end, the total points are tallied and a winner is declared!

## 📸 Example Output

```bash
🏁 🚨 Corrida entre Mario e Luigi começando...

🏁 Rodada 1
Bloco: CONFRONTO
Mario confrontou Luigi 🥊!
Mario 🎲 rolou um dado de poder 5 + 3 = 8
Luigi 🎲 rolou um dado de poder 2 + 4 = 6
Mario venceu o confronto! Luigi perdeu 1 ponto 🐢!

...

Resultado final:
Mario : 3
Luigi : 2

Mario venceu a corrida! Parabéns! 🏆
```

## 🚀 Getting Started

### Prerequisites

* [Node.js](https://nodejs.org/) (v14 or higher)

### Running the Game

```bash
node index.js
```

Enjoy the race in your terminal!

## 🛠️ Technologies Used

* [JavaScript (ES6+)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
* Native async/await
* Node.js runtime

## 🧩 Future Improvements

* Add character selection
* Add power-ups and banana traps 🍌
* Graphical interface with HTML Canvas or CLI styling
* Multiplayer input via CLI or web

## 👤 Author

**Gustavo Silva**
📧 [gugahenriquebatista@gmail.com](mailto:gugahenriquebatista@gmail.com)

---
