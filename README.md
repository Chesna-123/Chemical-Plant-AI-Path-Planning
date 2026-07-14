# Chemical-Plant-AI-Path-Planning
A Python-based simulation of intelligent robot path planning in a chemical plant using the A algorithm, 8-directional movement, and hazard-aware navigation
# Simulation of Intelligent Robot Path Planning in a Chemical Plant Using AI

## Overview

This project simulates an autonomous mobile robot navigating safely through a 2D chemical plant environment using the **A\*** (A-Star) path planning algorithm. The robot intelligently finds an optimal path from a start position to a target destination while avoiding walls, machinery, storage tanks, and hazardous zones.

The simulation is implemented in **Python** using **NumPy** and **Matplotlib**, and can be executed in **Google Colab** or a Jupyter Notebook.

---

## Project Objectives

- Simulate a chemical plant using a 2D grid environment.
- Implement intelligent robot navigation using the A* path planning algorithm.
- Enable 8-directional robot movement.
- Avoid static obstacles such as walls, storage tanks, and machinery.
- Minimize travel through hazardous areas using a cost-based navigation approach.
- Visualize the robot's planned path and movement.

---

## Features

- 2D Chemical Plant Environment
- A* Path Planning Algorithm
- 8-Directional Robot Movement
- Hazard-Aware Navigation
- Static Obstacle Avoidance
- Path Visualization
- Robot Movement Animation
- Cost-Based Decision Making

---

## Technologies Used

- Python 3
- Google Colab / Jupyter Notebook
- NumPy
- Matplotlib
- Heapq
- Math

---

## Plant Layout

The simulated plant consists of:

- Boundary Walls
- Chemical Storage Tanks
- Processing Machinery
- Hazard Zones (Gas Leak / Fire / Chemical Spill)
- Robot Start Position
- Goal Location

---

## Cell Representation

| Value | Description |
|-------|-------------|
| 0 | Empty Floor |
| 1 | Wall |
| 2 | Storage Tank |
| 3 | Hazard Zone |
| 4 | Robot |
| 5 | Goal |
| 6 | Machinery |
| 7 | Planned Path |

---

## Algorithm

The robot uses the **A\*** search algorithm.

### Cost Function

- Empty Cell = 1
- Hazard Zone = Higher Cost
- Walls = Not Traversable
- Tanks = Not Traversable
- Machinery = Not Traversable

The algorithm combines:

- Actual Travel Cost (g)
- Heuristic Cost (h)
- Total Cost (f = g + h)

to determine the safest and most efficient path.

---

## Project Workflow

1. Create the chemical plant grid.
2. Add boundary walls.
3. Add storage tanks.
4. Add machinery.
5. Add hazard zones.
6. Place the robot and destination.
7. Compute the optimal path using A*.
8. Visualize the planned path.
9. Animate the robot moving toward the goal.

---

## Future Improvements

- Dynamic obstacle detection
- Real-time hazard generation
- Automatic path replanning
- 3D simulation using ROS 2 and Gazebo
- Multiple robots
- Sensor simulation (LiDAR/Camera)
- Reinforcement Learning based navigation

---

## Repository Structure

```
Chemical-Plant-AI-Path-Planning/
│
├── Chemicalplant_AI_path_planning.ipynb
├── README.md
└── images/ (optional)
```

---

## Author

**Chesna**

B.Tech Robotics and Automation

---

## License

This project is intended for educational and academic purposes.
