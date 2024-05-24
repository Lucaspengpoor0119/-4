# -4
target = int(input("Think of a number between 1 and 100: "))
attempts = 0
max_attempts = 5

print("Welcome to the Guessing Game!")
print("You have 5 attempts to guess the number.")

while attempts < max_attempts:
    guess = int(input("Enter your guess: "))
    attempts += 1

    if guess == target:
        print("Congratulations, you guessed it!")
        break
    
    if guess < target:
        print("Too low, guess higher.")
    else:
        print("Too high, guess lower.")

if attempts == max_attempts:
    print("You've run out of guesses, the number was:", target)

