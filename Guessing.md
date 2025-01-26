# Number Guessing Game Flowchart


```mermaid
flowchart TD
 A([Generate random number]) --> B([Player guess input]) 
 B --> C@{ shape: diamond, label: "Is the guess correct?" }
 C -- Yes --> D([Congratulations! You got it right!])
 C -- No --> E@{ shape: diamond, label: "Is it too high or too low? }
 E -- Too high --> F([Too high. Guess again.]) --> B
 E -- Too low --> G([Too low. Guess again.]) --> B
```


### How it Works
*The game begins by setting a range for the random number and generating the target number within that range. The user is prompted to guess the number, and the program evaluates whether the guess is correct. If the guess matches the target, a success message is displayed, and the game ends. If the guess is incorrect, the program determines whether it is too high or too low, provides feedback, and prompts the user to guess again. This process loops until the correct number is guessed, after which the game displays a congratulatory message and concludes.*