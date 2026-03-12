# Kalman Filter Intuition

The Kalman filter is an algorithm used to estimate the state of a dynamic system from noisy measurements.

It is widely used in robotics, navigation systems, and embedded sensing applications.

---

## Core idea

A system typically has:

- a **prediction model**
- **noisy measurements**

The Kalman filter combines both sources of information to estimate the most probable state.

---

## Two phases

### Prediction

The system model predicts the next state:

- position
- velocity
- system variables

This prediction is based on previous estimates and the system dynamics.

---

### Update

When a measurement arrives, the filter updates the estimate by combining:

- predicted state
- sensor measurement

The algorithm assigns weight depending on the **uncertainty** of each source.

---

## Why it works

The filter works because it models:

- process uncertainty
- measurement uncertainty

Using covariance matrices, it determines how much trust to place in prediction versus measurement.

---

## Why it matters in robotics

Robots rarely observe the world perfectly.

Sensors are noisy, delayed, and sometimes unreliable.

Kalman filters allow robots to maintain stable estimates of:

- position
- velocity
- orientation
- system state
