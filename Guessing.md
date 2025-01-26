## Number Guessing Game Flowchart


```mermaid
flowchart TD
    A[Start] --> B[Set range for random number]
    B --> C[Generate random number within range]
    C --> D[Initialize user guess]
    D --> E[Prompt user for guess]
    E --> F{Is the guess correct?}
    F -->|Yes| G[Display "Correct! You guessed the number!"]
    F -->|No| H{Is the guess too high?}
    H -->|Yes| I[Display "Your guess is too high"]
    H -->|No| J[Display "Your guess is too low"]
    I --> K[Prompt user for another guess]
    J --> K[Prompt user for another guess]
    K --> F
    G --> L[End]
```


### How it Works
*The game begins by setting a range for the random number and generating the target number within that range. The user is prompted to guess the number, and the program evaluates whether the guess is correct. If the guess matches the target, a success message is displayed, and the game ends. If the guess is incorrect, the program determines whether it is too high or too low, provides feedback, and prompts the user to guess again. This process loops until the correct number is guessed, after which the game displays a congratulatory message and concludes.*