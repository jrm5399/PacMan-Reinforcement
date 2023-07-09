# PacMan Reinforcement Learning Code

This repository contains code for implementing reinforcement learning algorithms in PacMan, a classic arcade game. The code is written in Python and uses the `mdp` and `util` libraries for Markov decision process and utility functions.

## ValueIterationAgent

The `ValueIterationAgent` class is responsible for running value iteration on a given MDP (Markov decision process) for a specified number of iterations. It computes the optimal value function and stores the values for each state.

### Usage# PacMan Reinforcement Learning Code

This repository contains code for implementing reinforcement learning algorithms in PacMan, a classic arcade game. The code is written in Python and uses the `mdp` and `util` libraries for Markov decision process and utility functions.

## ValueIterationAgent

The `ValueIterationAgent` class is responsible for running value iteration on a given MDP (Markov decision process) for a specified number of iterations. It computes the optimal value function and stores the values for each state.

### Usage

```python
agent = ValueIterationAgent(mdp, discount, iterations)
```

- `mdp`: The Markov decision process instance
- `discount`: The discount factor for future rewards
- `iterations`: The number of iterations to run value iteration

### Methods

- `getValue(state)`: Returns the value of a given state
- `getPolicy(state)`: Returns the best action to take in a given state
- `getAction(state)`: Returns the best action to take in a given state (no exploration)
- `getQValue(state, action)`: Returns the Q-value of a given state-action pair

## AsynchronousValueIterationAgent

The `AsynchronousValueIterationAgent` class is a subclass of `ValueIterationAgent` that runs cyclic value iteration. It updates the value of one state in each iteration, cycling through the states list. If the chosen state is terminal, no updates are made.

### Usage

```python
agent = AsynchronousValueIterationAgent(mdp, discount, iterations)
```

- `mdp`: The Markov decision process instance
- `discount`: The discount factor for future rewards
- `iterations`: The number of iterations to run cyclic value iteration

## PrioritizedSweepingValueIterationAgent

The `PrioritizedSweepingValueIterationAgent` class is a subclass of `AsynchronousValueIterationAgent` that runs prioritized sweeping value iteration. It incorporates a prioritized sweeping technique to update the value of each state based on the most significant changes.

### Usage

```python
agent = PrioritizedSweepingValueIterationAgent(mdp, discount, iterations, theta)
```

- `mdp`: The Markov decision process instance
- `discount`: The discount factor for future rewards
- `iterations`: The number of iterations to run prioritized sweeping value iteration
- `theta`: The convergence threshold value

## Getting Started

To run the PacMan reinforcement learning code:

1. Install the required libraries: `mdp`, `util`.
2. Import the required modules: `mdp`, `util`, `learningAgents`.
3. Create an instance of the desired agent class (e.g., `ValueIterationAgent`).
4. Customize the agent settings if needed (e.g., discount factor, number of iterations).
5. Run the agent on the PacMan game environment.

Feel free to explore and modify the code to experiment with different reinforcement learning algorithms and settings.

**Note:** The code provided in this repository is a sample implementation and may require further customization and integration with the PacMan game environment for a complete working solution.

For more information and detailed usage instructions, please refer to the inline comments in the code files.

Enjoy exploring PacMan with reinforcement learning!

```python
agent = ValueIterationAgent(mdp, discount, iterations)
```

- `mdp`: The Markov decision process instance
- `discount`: The discount factor for future rewards
- `iterations`: The number of iterations to run value iteration

### Methods

- `getValue(state)`: Returns the value of a given state
- `getPolicy(state)`: Returns the best action to take in a given state
- `getAction(state)`: Returns the best action to take in a given state (no exploration)
- `getQValue(state, action)`: Returns the Q-value of a given state-action pair

## AsynchronousValueIterationAgent

The `AsynchronousValueIterationAgent` class is a subclass of `ValueIterationAgent` that runs cyclic value iteration. It updates the value of one state in each iteration, cycling through the states list. If the chosen state is terminal, no updates are made.

### Usage

```python
agent = AsynchronousValueIterationAgent(mdp, discount, iterations)
```

- `mdp`: The Markov decision process instance
- `discount`: The discount factor for future rewards
- `iterations`: The number of iterations to run cyclic value iteration

## PrioritizedSweepingValueIterationAgent

The `PrioritizedSweepingValueIterationAgent` class is a subclass of `AsynchronousValueIterationAgent` that runs prioritized sweeping value iteration. It incorporates a prioritized sweeping technique to update the value of each state based on the most significant changes.

### Usage

```python
agent = PrioritizedSweepingValueIterationAgent(mdp, discount, iterations, theta)
```

- `mdp`: The Markov decision process instance
- `discount`: The discount factor for future rewards
- `iterations`: The number of iterations to run prioritized sweeping value iteration
- `theta`: The convergence threshold value

## Getting Started

To run the PacMan reinforcement learning code:

1. Install the required libraries: `mdp`, `util`.
2. Import the required modules: `mdp`, `util`, `learningAgents`.
3. Create an instance of the desired agent class (e.g., `ValueIterationAgent`).
4. Customize the agent settings if needed (e.g., discount factor, number of iterations).
5. Run the agent on the PacMan game environment.

Feel free to explore and modify the code to experiment with different reinforcement learning algorithms and settings.

**Note:** The code provided in this repository is a sample implementation and may require further customization and integration with the PacMan game environment for a complete working solution.

For more information and detailed usage instructions, please refer to the inline comments in the code files.

Enjoy exploring PacMan with reinforcement learning!
