#project
import random

def guess_game():
    number_to_guess = random.randint(1, 10)
    guess = None

    while guess != number_to_guess:
        guess = int(input("Guess a number between 1 and 10: "))

        if guess < number_to_guess:
            print("Too low, try again.")
        elif guess > number_to_guess:
            print("Too high, try again.")

    print(f"Congratulations! You guessed the right number: {number_to_guess}")

guess_game()
