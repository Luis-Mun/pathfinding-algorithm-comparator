# Pathfinding Algorithm Comparator

> **Status: planned. Not started yet.** This repository currently contains the project scaffold and roadmap only.

Compare Q-learning, A*, and Dijkstra on the same mazes, with benchmarks and visualizations.

## Overview

Extends the TreasureHuntGame pirate-NPC project (SNHU CS-370). One shared maze environment is solved three ways, then measured on execution time, nodes explored, path length, memory, and success rate across maze sizes from 10x10 to 100x100.

## Skills demonstrated

Python, graph algorithms, reinforcement learning, benchmarking, Matplotlib, Pygame

## Planned structure

```
pathfinding-algorithm-comparator/
├── environment/     # shared maze representation + generator
├── algorithms/      # dijkstra.py, astar.py, qlearning.py
├── benchmark.py     # runs all algorithms on identical mazes
├── visualize.py     # Pygame demo + Matplotlib charts
├── tests/
├── results/         # benchmark output (CSV + charts)
└── docs/            # complexity analysis
```

## Roadmap

- [ ] Recover the original Q-learning code and confirm it still trains
- [ ] Shared maze environment (0 = path, 1 = wall, start, treasure) and generator
- [ ] Dijkstra with `heapq`
- [ ] A* with Manhattan heuristic
- [ ] Q-learning cleanup: measure training time and path execution separately
- [ ] `benchmark.py`: time, nodes explored, path length, memory, success rate across 10/25/50/100 sizes
- [ ] Pygame demo and Matplotlib charts
- [ ] Complexity documentation: Dijkstra O((V+E) log V), A* heuristic-dependent, Q-learning O(T) time / O(S x A) space

## Getting started

Setup, run, and test instructions will be added as each roadmap item is completed.

## Screenshots

Will be added to `screenshots/` once there is something to show.

## Future improvements

To be added after the first working version.

---

*Needed to proceed:* The TreasureHuntGame source (maze, pirate NPC, Q-learning code). The zip received so far only contained the Android app..
