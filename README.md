#Seyed Alireza Mortazavi(S6136275)/Profesor:Armando Tacchella
#Gridworld Monte Carlo Simulation

# Gridworld Monte Carlo Simulation

## Overview

This repository contains a Python implementation of a simple reinforcement learning environment known as Gridworld, using the Monte Carlo method for estimating state values. The Gridworld is a 5x5 grid where an agent moves based on defined actions. The Monte Carlo simulation is used to estimate the value of each state in the grid by running multiple episodes and averaging the returns.

## Features

- **Gridworld Environment**: A basic 5x5 grid representing the environment in which an agent operates.
- **Special States**: Two special states (`A` and `B`) with deterministic transitions to `A'` and `B'` and associated rewards.
- **Actions**: Four possible actions - north, south, east, and west - that the agent can take in each state.
- **Monte Carlo Simulation**: Implementation of the first-visit Monte Carlo method for estimating state values.
- **Visualization**: Heatmap and bar chart visualization of state-value functions after running the simulation.

## Files in the Repository

- `gridworld_monte_carlo.py`: Main Python script containing the implementation of the Gridworld environment and Monte Carlo simulation.

## Dependencies

- Python 3.x
- NumPy: For numerical operations.
- Matplotlib: For generating visualizations of the state-value functions.

## Setup and Running the Simulation

1. **Installation**:
   - Ensure that Python 3.x is installed on your system.
   - Install the required Python packages:
     ```
     pip install numpy matplotlib
     ```

2. **Running the Simulation**:
   - Execute the script `gridworld_monte_carlo.py`:
     ```
     python gridworld_monte_carlo.py
     ```
   - This will run the Monte Carlo simulation for 5000 episodes and display the resulting state-value function visualizations.

## Implementation Details

### `Gridworld` Class

- **Purpose**: Defines the gridworld environment.
- **Special States**: State `A` with transition to `A'` and a reward of 10, and state `B` with transition to `B'` and a reward of 5.
- **Boundaries**: If an action leads to moving outside the grid, the state remains the same with a penalty reward of -1.

### `MonteCarloSimulation` Class

- **Purpose**: Implements the Monte Carlo simulation to estimate state values.
- **Method**: First-visit Monte Carlo method, where the return for each state is calculated as the sum of discounted rewards from that state until the end of the episode.
- **Episodes**: By default, the simulation runs for 5000 episodes.

### Visualization

- **Heatmap**: Shows the value of each state in the grid after the simulation.
- **Bar Chart**: Displays the same state values as a bar chart for a different perspective.


