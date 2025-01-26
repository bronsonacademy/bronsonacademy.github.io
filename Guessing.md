# Number Guessing Game Flowchart


```mermaid
flowchart TD
    Start([Start]) --> InputRange[Input range for random number]
    InputRange --> GenerateRandom[Generate random number within range]
    GenerateRandom --> UserGuess[Prompt user to guess the number]
    UserGuess --> CompareGuess{Is the guess correct?}
    
    CompareGuess -->|Too High| FeedbackHigh[Inform "Too high"]
    FeedbackHigh --> UserGuess
    
    CompareGuess -->|Too Low| FeedbackLow[Inform "Too low"]
    FeedbackLow --> UserGuess
    
    CompareGuess -->|Correct| Congratulate[Congratulate the user]
    Congratulate --> PlayAgain{Play again?}
    
    PlayAgain -->|Yes| InputRange
    PlayAgain -->|No| End([End])
```


### How it Works
*The game begins by setting a range for the random number and generating the target number within that range. The user is prompted to guess the number, and the program evaluates whether the guess is correct. If the guess matches the target, a success message is displayed, and the game ends. If the guess is incorrect, the program determines whether it is too high or too low, provides feedback, and prompts the user to guess again. This process loops until the correct number is guessed, after which the game displays a congratulatory message and concludes.*