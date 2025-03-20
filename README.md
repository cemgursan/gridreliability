# Energy Mix Optimization with Monte Carlo Simulation and Genetic Algorithms

This repository contains a Python project that optimizes the energy mix for a power grid. It integrates multiple techniques:
- **Monte Carlo Simulation:** Estimates grid reliability by simulating capacity variations.
- **Linear Programming:** Uses PuLP to minimize generation costs while meeting energy demand.
- **Genetic Algorithm Optimization:** Applies DEAP to further optimize the energy mix under cost and demand constraints.

## Overview

The script considers a set of energy sources (Solar, Wind, Gas, Hydro, Coal, Nuclear) with predefined costs and capacity limits. It:
- Simulates available capacity using Monte Carlo methods to assess grid reliability.
- Solves a cost-minimization problem with linear programming to determine an optimal energy mix.
- Uses a genetic algorithm to refine the energy allocation by balancing cost with a penalty for any unmet demand.

## Features

- **Monte Carlo Reliability Simulation:**  
  Estimates the probability that the total available capacity meets a specified demand.

- **Linear Programming Optimization:**  
  Finds the optimal allocation of energy sources to minimize cost while satisfying demand using PuLP.

- **Genetic Algorithm Optimization:**  
  Uses DEAP to further optimize the energy mix, ensuring robust performance under different scenarios.

## Requirements

The project depends on the following Python packages:

- `numpy`
- `pandas`
- `pulp`
- `matplotlib`
- `scipy`
- `deap`

## Installation

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/yourusername/energy-mix-optimization.git
    cd energy-mix-optimization
    ```

2. **Install Dependencies:**

   You can install all required packages using the provided `requirements.txt` file:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

Run the Python script to perform the optimization:

```bash
python main.py
