# State Machine Design

Finite state machines are widely used in embedded systems to structure behaviour.

They allow complex behaviour to be represented as transitions between well-defined states.

---

## Basic structure

A state machine typically includes:

- a set of states
- transitions between states
- events that trigger transitions

---

## Why they are useful

State machines make system behaviour:

- predictable
- modular
- easier to debug

---

## Example in robotics

Robots often implement behaviours such as:

SEARCH → APPROACH → GRAB → RETURN

Each stage can be represented as a state in the system.

---

## Embedded systems relevance

State machines are especially useful in embedded systems where deterministic behaviour is important.
