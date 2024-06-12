# Rock-Paper-Scissors Game in Python

## Instructions

You are tasked with creating a simple Rock-Paper-Scissors game in Python. Follow the instructions below to implement the game:

### 1. Create a Python script

Start by creating a new Python script named `rock_paper_scissors.py`.

### 2. Game Logic

- Define a list named `computer_choices` containing the choices for the computer: 'rock', 'paper', and 'scissors'.
- Initialize three variables to keep track of the user's wins, computer's wins, and draws. You can name these variables as `user_wins`, `computer_wins`, and `draws`, respectively, and set them to 0.

### 3. Main Loop

Use a `while` loop to allow the user to play multiple rounds until they choose to exit.

### 4. User Input

- Inside the loop, prompt the user to input their choice: 'rock', 'paper', or 'scissors'. You can also provide an option to exit the game by entering 'exit'.

### 5. Input Validation

- Validate the user's input to ensure it's one of the valid choices ('rock', 'paper', 'scissors', or 'exit'). If the input is invalid, print an error message and continue to the next round.

### 6. Computer's Choice

- Determine the computer's choice by cycling through the `computer_choices` list. Use an integer variable, `computer_index`, initialized to 0, to keep track of the index of the last computer choice. Each time the computer needs to make a choice, access the element at index `computer_index` in the `computer_choices` list to get the computer's choice. Increment `computer_index` by 1 after each round, and use the modulo operator (%) to ensure that `computer_index` cycles back to 0 when it reaches the end of the list.

### 7. Result Determination

- Compare the user's choice and the computer's choice to determine the winner of the round. Update the score accordingly: increment the user's wins, computer's wins, or draws.

### 8. Score Display

- After each round, display the result of the round and the current score (number of user wins, computer wins, and draws).

### 9. Game Termination

- If the user chooses 'exit', end the game and display a farewell message.

## Sample Output

```
Enter rock, paper, or scissors (or 'exit' to quit): rock
Computer chose: paper
You lose this round.
Score - You: 0, Computer: 1, Draws: 0

Enter rock, paper, or scissors (or 'exit' to quit): paper
Computer chose: scissors
You lose this round.
Score - You: 0, Computer: 2, Draws: 0

Enter rock, paper, or scissors (or 'exit' to quit): scissors
Computer chose: rock
You lose this round.
Score - You: 0, Computer: 3, Draws: 0

Enter rock, paper, or scissors (or 'exit' to quit): exit
Thanks for playing!
```

## Note

- Ensure proper validation of user input to handle cases where the user enters an invalid choice.
- The computer's choices should cycle through the list repeatedly.
- Provide an option for the user to exit at any time.
