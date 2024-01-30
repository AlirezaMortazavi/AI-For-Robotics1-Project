# Seyed Alireza Mortazavi(S6136275)/Professor:Armando Tacchella

# Gridworld Monte Carlo Simulation

## Overview
The "Gridworld Monte Carlo Simulation" is a reinforcement learning project focused on a 5x5 grid environment known as gridworld. This environment serves as a testing ground for understanding the dynamics of state values and agent actions. Unique states, A and B, offer diverse outcomes through specific transitions and rewards. The project's core lies in applying the Monte Carlo method for state-value estimation, pivotal in reinforcement learning, achieved by analyzing numerous episodes and their accrued rewards.

## Features

- **Gridworld Environment**: A basic 5x5 grid representing the environment in which an agent operates.
- **Special States**: Two special states (`A` and `B`) with deterministic transitions to `A'` and `B'` and associated rewards.
- **Actions**: Four possible actions - north, south, east, and west - that the agent can take in each state.
- **Monte Carlo Simulation**: Implementation of the first-visit Monte Carlo method for estimating state values.
- **Visualization**: Heatmap and bar chart visualization of state-value functions after running the simulation.
  
### Visualization

- **Heatmap**: Shows the value of each state in the grid after the simulation.
 
![1](https://github.com/AlirezaMortazavi/Artificial-Intelligence-1/assets/69080319/de4a0ffb-93fa-4f00-af7d-d34b72a5e63a)

- **Bar Chart**: Displays the same state values as a bar chart for a different perspective.
  
![2](https://github.com/AlirezaMortazavi/Artificial-Intelligence-1/assets/69080319/75bb9c49-82fb-424b-838d-d01dd955e790)

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
   - Execute the script `S6136275.ipynb`:
     ```
     python S6136275.ipynb
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



