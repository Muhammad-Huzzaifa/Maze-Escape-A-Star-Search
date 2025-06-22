# Maze Escape: Save the Scientist 🧪

A Python implementation of an A* pathfinding algorithm to help a scientist escape from a maze with various obstacles and challenges.

## 🎯 Project Overview

This project implements an intelligent maze escape system using the A* search algorithm. The scenario involves helping a trapped scientist find the optimal escape route through a maze filled with various obstacles and challenges.

## 🔑 Key Features

- **Dynamic Maze Generation**: Randomly generates 15×15 mazes with:
  - Walls (30% of cells)
  - Traps with variable costs (10% of cells)
  - High-cost locks (5% of cells)
  - 1-2 exit points
  - Guaranteed solvability check

- **A* Search Implementation**:
  - Optimal pathfinding with cost considerations
  - Support for multiple heuristics (Manhattan/Euclidean)
  - Complete path reconstruction
  - Performance metrics tracking

- **Visualization**:
  - Color-coded maze representation
  - Path visualization
  - Trap cost display
  - Interactive matplotlib plots

## 🛠️ Technical Components

### 1. Maze Elements
- **Empty cells**: Base cost traversal
- **Walls**: Impassable obstacles
- **Traps**: Variable cost (1-9) cells
- **Locks**: High-cost barriers (cost: 1000)
- **Exit**: Goal state(s)
- **Start**: Initial position

### 2. Classes
- `GenerateMaze`: Handles maze creation and visualization
- `Node`: Represents search tree nodes for A* algorithm
- `AStarSearch`: Implements the A* pathfinding algorithm
- `Simulation`: Orchestrates the overall maze-solving process

## 📊 Performance Metrics

The implementation tracks several key performance indicators:
- Path cost
- Path length
- Search time
- Number of nodes explored
- Maximum frontier size

## 🔧 Dependencies

- numpy
- matplotlib
- collections (deque)
- heapq
- typing
- time

## 💻 Usage

```python
# Create a simulation instance
solution = Simulation(size=15, huristic='manhattan')

# Run multiple test cases
solution.run_all_tasks(num=3)
```

## 🎨 Visualization Example

The project provides two types of visualizations:
1. Initial maze state with all components
2. Solution path overlay showing the optimal route

## 📈 Performance Analysis

The A* implementation consistently finds optimal paths with:
- Millisecond-level solving times
- Efficient node exploration (20-200 nodes typically)
- Memory-efficient frontier management
- Optimal path costs considering all obstacles

## 👥 Contributing

Feel free to contribute to this project by:
1. Forking the repository
2. Creating your feature branch
3. Committing your changes
4. Creating a pull request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.
