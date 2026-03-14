# Probabilistic Occupancy Grids: Mapping the Unknown

Robotic mapping is the process of transforming sensor streams into a spatial representation of the world. Occupancy Grids provide a robust, probabilistic framework for this task.

## Representation of Uncertainty

The environment is divided into a grid of cells. Each cell stores the probability of being occupied. This allows for:

- **Efficient Updates:** New measurements (from Lidar or Sonar) are added to the existing probability.
- **Handling Unknowns:** Cells can represent "Unknown" space when we haven't explored them yet, typically starting at a 50% probability.

## Mapping as Information Gain

From a sensing perspective, mapping is about reducing uncertainty in the spatial domain.

- **Unknown Space:** High uncertainty.
- **Mapped Space:** Information gain (we know if it's free or occupied).

As the robot explores, it converts raw, noisy range data into a structured map that can be used for path planning and obstacle avoidance.
