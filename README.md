# Robot Maze Solver

An interactive maze solver that uses the **A\* pathfinding algorithm** to find the shortest route from a robot to its goal.

Built with vanilla HTML, CSS, and JavaScript — no libraries, no install, just open and run.

---

## Live Demo

[View it live](https://YOUR_USERNAME.github.io/Robot-in-a-Maze)

---

## How it works

A\* finds the shortest path by scoring every cell it considers:

```
f(n) = g(n) + h(n)
```

- `g(n)` — exact number of steps taken from the start
- `h(n)` — estimated steps remaining (Manhattan distance to goal)

It always picks the cell with the lowest `f(n)` score, which guarantees the shortest path while exploring far fewer cells than a brute-force search.

---

## Features

- **A\* pathfinding** with live step-by-step animation
- **3 maze generators**
  - Random DFS — long winding corridors
  - Prim's Algorithm — dense branching dead-ends
  - Recursive Division — architectural, grid-like rooms
- **Adjustable speed** — watch it think slowly or finish instantly
- **Interactive** — click any cell to move the robot, Shift+Click to move the goal
- **Live metrics** — visited nodes, frontier size, path length, solve time

---

## Usage

No installation needed.

1. Download `index.html`
2. Open it in any browser

Or clone the repo:

```bash
git clone https://github.com/YOUR_USERNAME/Robot-in-a-Maze.git
cd Robot-in-a-Maze
open index.html
```

---

## Controls

| Action | Result |
|---|---|
| Click a cell | Move the robot there |
| Shift + Click a cell | Move the goal there |
| New Maze | Generate a fresh maze |
| Solve | Run A* and animate the solution |
| Reset | Clear the solution, keep the maze |
| Speed slider | Control animation speed |

---

## Project structure

```
Robot-in-a-Maze/
└── index.html    ← entire app in one file
└── README.md
```

---

## License

MIT
