# Finite Automaton Acceptance Checker

This Python program allows users to define a Finite State Machine (FSM) and check the acceptability of strings within the specified FSM. Users can input details such as the number of states, inputs, transitions, and final states.

## Getting Started

### Prerequisites

Make sure you have Python installed. You can download it from [python.org](https://www.python.org/downloads/).

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/mahmoudelgoharyme/Finite-Automaton-Acceptance-Checker.git
    ```

2. Navigate to the project directory:

    ```bash
    cd Finite-Automaton-Acceptance-Checker
    ```

### Usage

Run the Python script:

```bash
python finite_automaton_checker.py
```

## Example

```python
# Example Input:
# Number of states: 4
# Enter the 1st state: 1
# Enter the 2nd state: 2
# Enter the 3rd state: 3
# Enter the 4th state: 4

# Number of inputs: 3
# Enter the 1st input: a
# Enter the 2nd input: b
# Enter the 3rd input: c

# Enter the initial state: 1

# Number of final states: 2
# Enter the 1st final state: 2
# Enter the 2nd final state: 4

# {1, a} = 2
# {1, b} = 3
# {1, c} = 1
# {2, a} = 1
# {2, b} = 3
# {2, c} = 4
# {3, a} = 2
# {3, b} = 4
# {3, c} = 1
# {4, a} = 3
# {4, b} = 3
# {4, c} = 2

# Result:
# δ     |     a b c
# ----------------------------------------
# 1     |     2 3 1
# 2     |     1 3 4
# 3     |     2 4 1
# 4     |     3 3 2

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: ccca
The string is acceptable for the Finite Automaton.

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: cbabc
The string is not acceptable for the Finite Automaton.

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: b
The string is not acceptable for the Finite Automaton.

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: bbbb
The string is acceptable for the Finite Automaton.

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: exit
