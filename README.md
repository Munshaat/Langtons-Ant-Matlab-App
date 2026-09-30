# Langton's Ant MATLAB Application

An interactive MATLAB App Designer project that simulates **Langton's Ant**, a cellular automaton that produces complex emergent patterns from a simple set of movement rules.

This project was developed for **EEE 4416 — Simulation Lab** at the Islamic University of Technology (IUT).

## Project Overview

The application simulates the movement of Langton's Ant on a two-dimensional grid. Users can define the **grid size** and **number of simulation steps**, then observe the ant's movement and the resulting changes in the grid in real time.

The application provides an interactive graphical interface with controls for:

* Starting the simulation
* Pausing and resuming
* Stopping the simulation
* Refreshing the simulation
* Setting grid size
* Setting the number of steps

## Langton's Ant Algorithm

The simulation follows two basic rules:

1. If the ant encounters one cell state, it turns 90° in one direction, changes the cell state, and moves forward.
2. If it encounters the other cell state, it turns 90° in the opposite direction, changes the cell state, and moves forward.

The grid is continuously updated as the ant moves, allowing complex patterns to emerge from these simple rules.

## Implementation

The application was developed using **MATLAB App Designer** and object-oriented programming principles. The application class inherits from `matlab.apps.AppBase`.

### Core Components

* 2D grid initialization
* Ant position tracking
* Ant direction tracking
* Step-by-step simulation
* Cell-state modification
* Direction control
* Boundary handling
* Real-time visualization
* Simulation pause/resume control
* GUI callbacks

### Grid and Movement

The ant is initially positioned at the center of the grid and begins facing upward. At every simulation step, the current cell is checked, the ant changes direction according to the cell state, the cell state is flipped, and the ant moves forward.

Boundary handling is implemented using modulo-based indexing so that the ant wraps around to the opposite side when it reaches a grid boundary.

## Graphical User Interface

The MATLAB application includes:

* Simulation display using `UIAxes`
* Start button
* Pause/Resume button
* Stop button
* Refresh button
* Grid-size input
* Number-of-steps input

The interface continuously updates the grid visualization during simulation.

## Visualization

The grid is visualized using MATLAB's `imagesc` function with a custom colormap representing the two cell states. The simulation display is updated after each movement of the ant.

## Key Concepts

* MATLAB programming
* MATLAB App Designer
* Object-oriented programming
* Cellular automata
* Algorithm design
* Matrix manipulation
* GUI development
* Event-driven programming
* Callback functions
* Real-time simulation
* Data visualization
* Debugging


## Course Information

**Course:** EEE 4416 — Simulation Lab
**Institution:** Islamic University of Technology (IUT)

## Repository Structure

```text
langtons-ant-matlab-app/
│
├── README.md
│
├── Langtons_Ant_App.mlapp
│
└── Langtons_Ant_Project_Report.pdf
```
