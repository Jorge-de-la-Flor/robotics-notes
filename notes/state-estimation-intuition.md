# State Estimation: Inferring Reality from Noise

In robotics, the "State" represents the set of hidden variables—such as position, velocity, and orientation—that define a system's condition. The fundamental challenge of robotics is that state is never directly observable; it must be inferred from incomplete and noisy data.

## The Reality of Partial Observability

Physical sensors do not provide "truth"; they provide noisy evidence with inherent limitations:

- **External Sensors (GPS/Lidar):** Provide absolute references but suffer from interference, occlusions, and low sampling rates.
- **Internal Sensors (IMU/Encoders):** Essential for high-frequency updates, but prone to integration drift over time.

## The Recursive Bayesian Framework

State estimation is treated as a recursive process. we maintain a probability distribution (belief) over the state and refine it as information arrives:

1. **Prediction:** We use a motion model to project where the robot should be. This step naturally increases uncertainty as the system moves.
2. **Correction:** We fuse new sensor observations to pull the estimate toward reality, effectively reducing the system's uncertainty.

## Importance in Autonomy

Robust state estimation is the prerequisite for high-level autonomy. Whether it is a surgical tool or an autonomous vehicle, the ability to fuse inconsistent data into a single, reliable "Source of Truth" is what defines a mission-critical robotic system.
