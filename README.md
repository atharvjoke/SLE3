# SLE3
# AI Refrigerator Agent

## Overview
The **AI Refrigerator Agent** is an intelligent agent designed to monitor and manage conditions inside a smart refrigerator. It receives information such as temperature, door status, and food/item condition through sensors or user input. It analyses the current state and selects an appropriate action, such as increasing cooling, reducing cooling, raising an alert, or notifying the user.

The main goal is to maintain suitable food-storage conditions while reducing unnecessary energy use.

## SLE-3: Architectural Design (Full C4 Model)
**Course:** 02AML204 – Introduction to Artificial Intelligence  
**Student:** Atharv Jindatta Joke  
**PRN:** 25UAM047  
**Division:** A  
**System:** AI Refrigerator Agent

This repository documents the system architecture using the four C4 model levels:

1. **Context (Level 1):** Shows how the user and smart refrigerator/sensors interact with the AI Refrigerator Agent.
2. **Container (Level 2):** Describes the Input/Sensor Module, State Manager, Decision Engine, Action Controller, and Alert/Output Module.
3. **Component (Level 3):** Breaks down the Decision Engine into the State Evaluator, Rule/Condition Checker, Goal/Safety Checker, and Action Selector.
4. **Code (Level 4):** Outlines the main classes and functions that represent refrigerator state, sensor input, state updates, condition evaluation, action selection, and action execution.

## Main Workflow
1. Collect temperature, door-status, and item-condition information.
2. Update the refrigerator's current state.
3. Evaluate conditions and select a suitable action.
4. Execute or request the selected refrigerator action.
5. Display the status and notify the user when attention is needed.

## Main Classes and Functions
| Class / Function | Responsibility |
|---|---|
| `RefrigeratorState` | Stores temperature, door status, and item-condition information. |
| `SensorInput` | Represents input received from refrigerator sensors. |
| `update_state()` | Updates the current refrigerator state. |
| `evaluate_conditions()` | Checks the current state against operating conditions. |
| `decide_action()` | Selects cooling, reduce-cooling, alert, or no-change action. |
| `execute_action()` | Sends the selected action to the refrigerator/controller. |

## Design Decisions
- Keep the architecture small and easy to understand and test.
- Separate decision-making from input collection and action handling.
- Use a State Manager so decisions are based on the current refrigerator state.
- Keep the C4 levels clear, from the overall system to its internal logic.

## AI Contribution Note
ChatGPT was used to help structure the C4 architecture, organize report sections, prepare concise explanations, and check that all four C4 levels were represented. The student selected the AI Refrigerator Agent, reviewed the architecture, chose the main containers and components, and is responsible for understanding and explaining the design.

## Project Status
This repository presents the **SLE-3 architectural design**. The classes and functions listed above are a code-level overview; this document does not claim that a complete working implementation is included.

## Reference
The architecture and descriptions are based on the SLE-3 report submitted for the course **02AML204 – Introduction to Artificial Intelligence**.
