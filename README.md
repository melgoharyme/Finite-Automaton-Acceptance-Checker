# Finite Automaton Acceptance Checker

## Overview

This Python program allows users to define a Finite State Machine (FSM) and check the acceptability of strings within the specified FSM. Users can input details such as the number of states, inputs, transitions, and final states.

## Usage

1. Clone the repository:

    ```bash
    git clone https://github.com/mahmoudelgoharyme/Finite-Automaton-Acceptance-Checker.git
    ```

2. Navigate to the project directory:

    ```bash
    cd Finite-Automaton-Acceptance-Checker
    ```

3. Run the Python script:

    ```bash
    python main.py
    ```

4. Follow the on-screen prompts to define the FSM and test strings for acceptability.

## Example

```python
# Example Input:
# Number of states: 2
# Enter the 1st state: A
# Enter the 2nd state: B

# Number of inputs: 2
# Enter the 1st input: 0
# Enter the 2nd input: 1

# Enter the initial state: A

# Number of final states: 1
# Enter the 1st final state: B

# {A, 0} = B
# {A, 1} = A
# {B, 0} = A
# {B, 1} = B

# Result:
# δ   |      0 1
# ---------------
# A   |  B A
# B   |  A B
