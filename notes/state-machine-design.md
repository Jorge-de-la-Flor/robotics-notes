# State Machine Design: Structuring Complex Behaviour

In embedded robotics, unpredictable behaviour is a failure. Finite State Machines (FSMs) are used to organize complex logic into well-defined, predictable transitions.

## Why FSMs Matter in Robotics

Robots often operate in stages (e.g., Search -> Identify -> Grab -> Return). A state machine ensures that:

- **Predictability:** The robot can only be in one state at a time.
- **Modularity:** New behaviours can be added as new states without breaking existing logic.
- **Safety:** We can define "Safe" or "Error" states that the system defaults to in case of sensor failure.

## Designing for Determinism

By using state machines, we move away from "spaghetti code" (nested if-else statements) toward an architectural design. This makes the system easier to debug, test, and verify—a requirement for any mission-critical autonomous platform.

## Integration with Control

While a PID loop handles the "how to move," the State Machine handles the "what to do." Together, they form the bridge between high-level intelligence and low-level execution.
