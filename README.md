# Using-variable-loops-and-functions-to-create-a-basic-game
i have used variable loops and functions in the c programming language to make a basic game

use a c compiler to run this game and enjoy it

#include <stdio.h>

int main() {
    int secretNumber = 42; // You can change this to any number of your choice
    int guess;
    int attempts = 0;

    printf("Welcome to the Guessing Game!\n");
    printf("I have selected a secret number between 1 and 100. Try to guess it.\n");

    do {
        printf("Enter your guess: ");
        scanf("%d", &guess);

        attempts++;

        if (guess > secretNumber) {
            printf("Too high! Try again.\n");
        } else if (guess < secretNumber) {
            printf("Too low! Try again.\n");
        } else {
            printf("Congratulations! You guessed the correct number %d in %d attempts.\n", secretNumber, attempts);
        }
    } while (guess != secretNumber);

    return 0;
}
