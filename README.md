# PRODIGY_SD_02

## Create a Guessing Game

### Problem Statement:
Build a program that generates a random number and challenges the user to guess it. The program should prompt the user to input their guess, compare it to the generated number, and provide feedback if the guess is too high or too low. It should continue until the user correctly guesses the number and then display the number of attempts it took to win the game.

### Solution:

#### Random Number Generation:
Uses srand(time(0)) to seed the random number generator with the current time, ensuring a different seed each time the program runs.
Generates a random number (secretNumber) between 1 and 100 using rand() % 100 + 1.

#### Game Loop:
Asks the user to input a guess within the range of 1 to 100.
Increments the attempts counter with each guess.

#### Feedback:
Provides feedback to the user based on their guess:
If the guess is lower than secretNumber, it displays "Too low! Try again."
If the guess is higher than secretNumber, it displays "Too high! Try again."
If the guess matches secretNumber, it congratulates the user and displays the number of attempts made.

#### Loop Termination:
Continues looping until the user correctly guesses secretNumber, at which point the loop ends.

#### End of Program:
Outputs a message indicating the game is over and exits.
