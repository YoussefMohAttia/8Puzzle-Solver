<div align="center">

# 8-Puzzle Solver

### Interactive Search Visualizer for BFS, DFS, and A* Algorithms

[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Pygame](https://img.shields.io/badge/Pygame-Interactive%20UI-2E8B57)](https://www.pygame.org/)

</div>

## Overview

An interactive 3 x 3 sliding-puzzle application that lets a player shuffle, solve, and step through puzzle states. The solver implements breadth-first search, depth-first search, and A* search with Manhattan-distance and Euclidean-distance heuristics.

## Features

- Play the puzzle directly through a Pygame interface
- Shuffle and reset the board
- Detect unsolvable arrangements before search
- Animate a full solution or step forward and backward through it
- Compare BFS, DFS, and two A* heuristic variants with `analyze.py`

## Repository Structure

```text
.
├── main.py                              # Pygame interface
├── Solver.py                            # Puzzle model and search implementations
├── analyze.py                           # Search comparison script
├── left.png / right.png                 # Solution navigation icons
├── algorithm_comparison*.png            # Generated comparison charts
└── algorithm_comparison*.png            # Search performance visualizations
```

## Getting Started

```bash
python -m venv .venv
source .venv/bin/activate
pip install pygame numpy matplotlib
python main.py
```

To reproduce the algorithm comparison charts:

```bash
python analyze.py
```

## Search Methods

| Method | Strategy |
| --- | --- |
| BFS | Explores the state space level by level |
| DFS | Explores a path deeply before backtracking |
| A* Manhattan | Uses tile Manhattan distance as the heuristic |
| A* Euclidean | Uses Euclidean tile distance as the heuristic |

## Author

**Youssef Mohamed Attia**  
[GitHub](https://github.com/YoussefMohAttia) · [LinkedIn](https://www.linkedin.com/in/youssefmohattia/)
