# Finite Automaton Acceptance Checker

This Python program allows users to define a Finite State Machine (FSM) and check the acceptability of strings within the specified FSM. Users can input details such as the number of states, inputs, transitions, and final states.

## Demo
![Demo Image](https://github.com/mahmoudelgoharyme/Finite-Automaton-Acceptance-Checker/raw/main/demo.png)


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

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Example

```python
# Example Input:
- Number of states: 4
Enter the 1 state: 1
Enter the 2 state: 2
Enter the 3 state: 3
Enter the 4 state: 4

- Number of inputs: 3
Enter the 1 input: a
Enter the 2 input: b
Enter the 3 input: c

- Enter the initial state: 1

- Number of final states: 2
Enter the 1 final state: 2
Enter the 2 final state: 4
{1, a} = 2
{1, b} = 3
{1, c} = 1
{2, a} = 1
{2, b} = 3
{2, c} = 4
{3, a} = 2
{3, b} = 4
{3, c} = 1
{4, a} = 3
{4, b} = 3
{4, c} = 2
δ | a b c
-----------------------------------------
1 | 2 3 1
2 | 1 3 4
3 | 2 4 1
4 | 3 3 2

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: abc
1 -a-> 2
2 -b-> 3
3 -c-> 1
Final state: ['2', '4']
The string is rejected for the Finite Automaton. Current state: 1

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: bcacba
1 -b-> 3
3 -c-> 1
1 -a-> 2
2 -c-> 4
4 -b-> 3
3 -a-> 2
Final state: ['2', '4']
The string is accepted for the Finite Automaton. Current state: 2

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: ccca
1 -c-> 1
1 -c-> 1
1 -c-> 1
1 -a-> 2
Final state: ['2', '4']
The string is accepted for the Finite Automaton. Current state: 2

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: cbaabc
1 -c-> 1
1 -b-> 3
3 -a-> 2
2 -a-> 1
1 -b-> 3
3 -c-> 1
Final state: ['2', '4']
The string is rejected for the Finite Automaton. Current state: 1

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: b
1 -b-> 3
Final state: ['2', '4']
The string is rejected for the Finite Automaton. Current state: 3

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: bbbb
1 -b-> 3
3 -b-> 4
4 -b-> 3
3 -b-> 4
Final state: ['2', '4']
The string is accepted for the Finite Automaton. Current state: 4

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: aa
1 -a-> 2
2 -a-> 1
Final state: ['2', '4']
The string is rejected for the Finite Automaton. Current state: 1

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: ab
1 -a-> 2
2 -b-> 3
Final state: ['2', '4']
The string is rejected for the Finite Automaton. Current state: 3

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: aba
1 -a-> 2
2 -b-> 3
3 -a-> 2
Final state: ['2', '4']
The string is accepted for the Finite Automaton. Current state: 2

Enter a string or type 'exit' to stop the program or enter 'again' to run the program again: abc
1 -a-> 2
2 -b-> 3
3 -c-> 1
Final state: ['2', '4']
The string is rejected for the Finite Automaton. Current state: 1
