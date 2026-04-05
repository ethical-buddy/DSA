#  Pathfinding Algorithm Duel - Territory Conquest Visualizer

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26.svg)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6.svg)](https://developer.mozilla.org/en-US/docs/Web/CSS)

##  Overview

**Watch 4 classic pathfinding algorithms battle in real-time to conquer territory!**

This interactive visualization pits **A\*, BFS, DFS, and Dijkstra** against each other on a procedurally generated maze. Each algorithm simultaneously explores the grid, coloring conquered cells as it goes. See which algorithm explores the most territory in the least time!

![Demo Preview](https://via.placeholder.com/800x400?text=Pathfinding+Algorithms+Duel)

##  Features

- **4 Algorithms Compete Simultaneously** - Watch them race side-by-side
- **Real-time Territory Visualization** - Colored cells = conquered area
- **Procedural Maze Generation** - Random walls with guaranteed path
- **Performance Metrics** - Track area conquered & completion time
- **Interactive Controls** - Start race or generate new maps
- **No Dependencies** - Pure HTML/CSS/JavaScript

##  Algorithms Explained

| Algorithm | Strategy | Territory Style | Speed |
|-----------|----------|----------------|-------|
| **A*** | Heuristic-driven (Manhattan distance) | Intelligent, goal-oriented |  Fast |
| **BFS** | Level-by-level exploration | Wave-like expansion | Fast |
| **DFS** | Deep exploration first | Branching, chaotic |  Variable |
| **Dijkstra** | Weighted shortest path | Systematic coverage |  Balanced |

##  How to Run

### Option 1: Direct Browser (Easiest)
```bash
# Download the HTML file and double-click it
open 2.html
````
# CUSTOMIZATION OPTIONS
  // In the HTML script, modify:
const SIZE = 150;  // Change to 100, 200, etc.

const OBSTACLE_DENSITY = 0.18;  // 0.0 to 0.5

// Add to algorithms array:
{ name: "Your Algo", key: "algo", color: "#yourcolor" }

// Implement generator function
function* yourAlgoGenerator(grid, start, target) {
    // Your logic here
    yield { type: "visit", visited: visitedSet };
}

// Change delay in runPathfinder function:
await new Promise(r => setTimeout(r, 2));  // Lower = faster

