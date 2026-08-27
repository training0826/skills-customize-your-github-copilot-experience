
# 📘 Assignment: Hangman Game

## 🎯 Objective

Build a playable Hangman game in Python. Practice string manipulation, loops, conditionals, user input, and random selection while managing the game's state.

## 📝 Tasks

### 🛠️ Build the Game Setup

#### Description

Create the starting structure for a Hangman game. Store a predefined list of words, randomly select one word, and display hidden letters for the player to guess.

#### Requirements

Completed program should:

- Store at least five words in a predefined list.
- Randomly select one word at the start of each game.
- Display one underscore for each letter in the selected word.
- Ask the player to enter a letter guess.

### 🛠️ Implement Gameplay and Results

#### Description

Add the game loop so the player can continue guessing until the word is complete or no attempts remain. Track guesses and provide clear feedback after each turn.

#### Requirements

Completed program should:

- Reveal correctly guessed letters in their proper positions.
- Track incorrect guesses and display the number of attempts remaining.
- Prevent the game from ending while there are unguessed letters and attempts remaining.
- End with a win message when the player guesses the word.
- End with a loss message and reveal the word when attempts are exhausted.
