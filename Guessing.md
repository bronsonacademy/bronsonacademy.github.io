# Number Guessing Game Flowchart


```mermaid
flowchart TD
 A([Generate random number]) --> B([Player guess input]) 
 B --> C@{ shape: diamond, label: "Is the guess correct?" }
 C -- Yes --> D([Congratulations! You got it right!])
 C -- No --> E@{ shape: diamond, label: "Is it too high or too low?" }
 E -- Too high --> F([Too high. Guess again.]) --> B
 E -- Too low --> G([Too low. Guess again.]) --> B
```


### How it Works
*The process begins with the computer generating a random number. The player inputs a guess, which the game checks to see if it's correct. If the guess is correct, the player wins, and the game ends. If it's incorrect, the game determines if the guess is too high or too low and provides feedback. The player then guesses again, repeating the process until the correct number is guessed.*