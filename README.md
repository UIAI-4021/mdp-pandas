# University of Isfahan Cliff Walking Project

![animated gif](https://gymnasium.farama.org/_images/cliff_walking.gif)

## Authors
- Melika Shirian
- Kianoosh Vadaei

## Instructor
- Dr. Hossein Karshenas

## Date
- 2023-11-08

## Introduction
Welcome to the University of Isfahan's Cliff Walking Project! This project explores the application of Markov Decision Processes (MDPs) in solving complex decision-making problems, focusing on the challenging scenario of the "Cliff Walking Game." In this game, an intelligent agent navigates a grid-world environment filled with risks, resembling a treacherous cliff.

## Implementation
Implemented using the Gymnasium library, the project aims to determine an optimal policy for the environment, specifying the actions the agent should take in each state. The value iteration method is employed, recalculating rewards for each state based on a heuristic function derived from Manhattan distance.

## Functions Overview

### 1. `possible_actions(state)`
- Evaluates feasible actions for each state, considering possible future states for improved policy determination.

### 2. `possible_actions2(state)`
- A precautionary function restricting the agent from selecting infeasible actions.

### 3. `step(state, action)`
- Custom implementation of the Gymnasium library's step function, applying actions to states.

### 4. `Q(state, action)`
- Calculates the Q-value for a specific state and action using the Bellman equation, considering the environment's boundaries.

### 5. `value_iteration()`
- Initializes state values, performs dynamic updates using the value iteration method until convergence, and extracts the optimal policy.

## Main Code Section
The main section creates the game environment, identifies cliff positions, and calls the `value_iteration` function to calculate the optimal policy. A loop iterates 1000 times, applying the policy to determine the agent's actions and updating the environment accordingly.

## Usage
1. Install necessary libraries: `pip install gym`
2. Run the code: `python cliff_walking.py`

## Conclusion
Explore the fascinating world of Markov Decision Processes through the Cliff Walking Project! Feel free to customize and extend the code to further investigate AI and reinforcement learning.

## References
- [Stanford University - Markov Decision Processes](https://web.stanford.edu/class/cs234/CS234Win2019/lectures/cs234_lecture02.pdf)
- [OpenAI - ChatGPT](https://www.openai.com/)
- Russell, Stuart, and Norvig, Peter. "Artificial Intelligence: A Modern Approach." (Book)
