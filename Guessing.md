# Number Guessing Game Flowchart


```mermaid
flowchart TD
 A([Generate random number and set the range]) --> B([Player guess input])
 B --> H@{ shape: diamond, label: "Is the guess a number?" }
 H -- Yes --> J
 H -- No --> I([Invalid input. Try again.]) --> B
 B --> J@{ shape: diamond, label: "Is the guess in range?" }
 J -- Yes --> C
 J -- No --> I
 B --> C@{ shape: diamond, label: "Is the guess correct?" }
 C -- Yes --> D([Congratulations! You got it right!])
 C -- No --> E@{ shape: diamond, label: "Is it too high or too low?" }
 E -- Too high --> F([Too high. Guess again.]) --> B
 E -- Too low --> G([Too low. Guess again.]) --> B
```


### How it Works
*The process begins with the computer generating a random number. The player inputs a guess, which the game checks is a number or not, then checks to see if it's correct. If the guess is correct, the player wins, and the game ends. If it's incorrect, the game determines if the guess is too high or too low and provides feedback. The player then guesses again, repeating the process until the correct number is guessed.*