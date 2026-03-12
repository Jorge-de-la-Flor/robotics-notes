# Occupancy Grid Mapping

Occupancy grids are a probabilistic method used by robots to represent their environment.

The world is divided into a grid of cells, and each cell stores the probability of being occupied.

---

## Concept

Each grid cell represents:

- free space
- occupied space
- unknown space

The robot updates these probabilities using sensor measurements.

---

## Why it works well

Occupancy grids allow robots to build maps incrementally while moving.

They are commonly used with sensors such as:

- lidar
- sonar
- depth cameras

---

## Applications

Occupancy grids are widely used in:

- mobile robot navigation
- SLAM systems
- path planning
- obstacle avoidance

---

## Key advantage

They allow robots to reason about uncertainty in the environment rather than assuming perfect measurements.
