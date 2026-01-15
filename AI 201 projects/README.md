# A* Search Algorithm for the 8-Puzzle Problem

An implementation of the A* search algorithm to solve the classic 8-puzzle sliding tile problem, featuring three different heuristic functions for comparison.

## Overview

The 8-puzzle consists of a 3x3 grid with 8 numbered tiles and one empty space. The goal is to rearrange the tiles from a given start state to a target goal state by sliding tiles into the empty space.

This project demonstrates how different heuristics affect the efficiency of the A* search algorithm.

## Heuristics Implemented

### 1. Misplaced Tiles (h1)
Counts the number of tiles that are not in their goal position. Simple but less informed.

### 2. Manhattan Distance (h2)
Calculates the sum of horizontal and vertical distances each tile must travel to reach its goal position. More informed than misplaced tiles.

### 3. Nilsson's Sequence Score (h3)
Combines Manhattan distance with a sequence score that penalizes tiles not following the correct clockwise sequence:
```
h(n) = Manhattan Distance + 3 × Sequence Score
```

## Performance Comparison

| Heuristic | Nodes Generated | Solution Length |
|-----------|-----------------|-----------------|
| Misplaced Tiles | 1,747 | 18 moves |
| Manhattan Distance | 227 | 18 moves |
| Nilsson's Sequence | 1,449 | 18 moves |

Manhattan Distance proves to be the most efficient heuristic for this problem, generating significantly fewer nodes while finding an optimal solution.

## Usage

### Input File Format

Create an input file `astar_in.txt` with the following format:
```
s 2 1 6 4 0 8 7 5 3 ; g 1 2 3 8 0 4 7 6 5
```
- `s` followed by 9 numbers represents the start state (row by row)
- `g` followed by 9 numbers represents the goal state
- `0` represents the empty tile
- States are separated by a semicolon `;`

### Running the Algorithm

```python
python A_search.py
```

Or run the Jupyter notebook `A_search.ipynb` for an interactive experience.

### Output

For each heuristic, the program displays:
- Step-by-step solution path with board states
- `f(n)`: Total estimated cost (g + h)
- `g(n)`: Cost from start (number of moves)
- `h(n)`: Heuristic estimate to goal
- Search cost (total nodes generated)

## Project Structure

```
AI 201 projects/
├── A_search.ipynb    # Jupyter notebook implementation
├── astar_in.txt      # Input file with start and goal states
└── README.md         # This file
```

## Algorithm Details

The A* algorithm uses:
- **OPEN list**: Priority queue of nodes to be expanded (sorted by f-value)
- **CLOSED list**: Set of already expanded nodes
- **Path reconstruction**: Parent pointers to trace solution path

Key features:
- Handles revisiting nodes with better paths
- Returns optimal solution when using admissible heuristics
- Reports search cost for heuristic comparison

## Requirements

- Python 3.x
- No external dependencies (uses only standard library)

## Course

AI 201 - Artificial Intelligence

## License

This project is for educational purposes.
