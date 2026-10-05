# OrbitGuard AI

## Space Debris Collision Detection and Avoidance

OrbitGuard AI is a decision-support dashboard for monitoring orbital objects and evaluating potential collision scenarios.

The project focuses on combining orbital mechanics with data-driven risk analysis so that an operator can identify potentially dangerous conjunctions early and evaluate possible avoidance actions.

## Project Overview

With the increasing number of satellites and the amount of debris in low Earth orbit, conjunction monitoring is becoming an important part of mission operations. A collision-avoidance workflow has to consider more than just the distance between two objects. Relative motion, orbital parameters, uncertainty in tracking data and the available maneuver options also affect the final decision.

OrbitGuard is designed around this workflow:

```text
Orbital / TLE Data
        |
        v
Orbit Propagation (SGP4)
        |
        v
Conjunction Screening
        |
        v
Miss Distance and Relative Geometry
        |
        v
Risk Assessment
        |
        v
Uncertainty Analysis
        |
        v
Maneuver Evaluation
        |
        v
Operator Decision Support
```

The system is intended as a decision-support tool. The final maneuver decision remains with the mission operator.

## Main Components

### 1. Orbital Data Processing

TLE and orbital parameters are used as the starting point for propagating the position of tracked objects.

### 2. Orbit Propagation

SGP4 propagation is used to estimate the position and velocity of an object at a given time.

### 3. Conjunction Analysis

Potentially close approaches are screened using relative position, miss distance and other available orbital information.

### 4. Risk Assessment

The dashboard presents the available parameters and risk assessment in a form that can be reviewed by an operator.

### 5. Uncertainty Analysis

Monte Carlo analysis can be used to evaluate how uncertainty in the input data can affect the predicted conjunction outcome.

### 6. Maneuver Planning

For a high-risk scenario, possible avoidance actions can be evaluated with respect to maneuver cost and safety constraints.

## Dashboard

The current working dashboard is hosted separately.

**Live Dashboard:**
https://v0-orbit-guard-ai-dashboard.vercel.app/

The dashboard provides the project workflow, risk information, analysis stages and maneuver-related decision support in an interactive interface.

## Design

The interface and visual design reference are available here:

**Figma:**
https://orbitguard-ai.figma.site/

## Technology

- Python
- NumPy
- Pandas
- SciPy
- SGP4
- PyTorch
- FastAPI
- React
- Three.js
- Monte Carlo simulation
- GitHub
- Vercel

The exact components used in a deployment may vary depending on the implementation stage.

## Project Goals

The main goals of OrbitGuard AI are:

1. Detect potentially risky conjunctions at an early stage.
2. Present orbital and collision-related information in a single interface.
3. Reduce the amount of repetitive manual analysis.
4. Evaluate uncertainty instead of relying on a single deterministic prediction.
5. Assist operators in comparing possible avoidance maneuvers.
6. Support safer and more sustainable satellite operations.

## Limitations

OrbitGuard AI is a prototype/decision-support concept. It should not be treated as an autonomous spacecraft control system.

Real mission operations require validated tracking data, certified orbital-dynamics software, mission-specific constraints, independent verification and human approval before any maneuver is executed.

## Project Credit

**VISION**

Made by **Priyanka Gupta**

## Repository Note

This repository currently serves as the documentation and project showcase for the OrbitGuard AI prototype. The working dashboard is hosted separately and is linked above.

The repository does not claim to contain source code that is not part of the supplied project files.
