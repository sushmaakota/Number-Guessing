# Number Guessing Game

This is a simple number guessing game implemented in Java. Below are the rules and the approach for this game.

## Rules

1. **Range of Numbers**: The computer randomly selects a number between 1 and 100.
2. **Number of Trials**: The player has 5 chances to guess the correct number.
3. **Hints**: After each incorrect guess, the game provides a hint:
   - If the guessed number is too low, the game informs the player that the correct number is greater.
   - If the guessed number is too high, the game informs the player that the correct number is smaller.
4. **Winning Condition**: The player wins if they guess the correct number within the allowed 5 attempts.
5. **Losing Condition**: If the player fails to guess the number after 5 attempts, the game ends, and the correct number is revealed.

## Approach

1. **Generate Random Number**: A random number is generated using `Math.random()`, scaled to the range of 1 to 100. This is the number the player must guess.

2. **Input from User**: The game uses `Scanner` to take the player's input in each attempt. The player enters their guessed number.

3. **Comparing the Guess**:
   - If the guessed number matches the random number, the player wins and the game ends.
   - If the guessed number is incorrect, the game provides a hint:
     - **Greater than the guess**: If the random number is greater than the player's guess, the game tells the player that the number is higher.
     - **Less than the guess**: If the random number is smaller, the game tells the player that the number is lower.

4. **Loop Control**: The loop runs for a maximum of 5 iterations (trials). If the player doesn't guess the correct number within 5 attempts, the game ends and reveals the correct number.

5. **Ending the Game**: The game either ends when the player guesses the correct number or when the maximum number of trials is reached, at which point it displays the correct number.

## Example Walkthrough:
- The program generates a random number, say 45.
- The player guesses 30.
- The game informs the player that the correct number is greater than 30.
- The player guesses 60.
- The game informs the player that the correct number is less than 60.
- The player guesses 45.
- The game congratulates the player for guessing correctly and ends.

