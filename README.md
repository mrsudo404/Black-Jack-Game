# Blackjack Game README

## Overview

This is a Python implementation of the classic card game Blackjack. The game is played against a dealer, and the objective is to have a hand value as close to 21 as possible without exceeding it. This implementation features card shuffling, dealing, hand value calculation, and game logic for determining the winner.

## Installation

To play the game, you'll need to have Python installed on your computer. The game doesn't require any additional libraries outside of the standard library.

### Step-by-Step Setup

1. **Clone the repository:**
   If you have Git installed, you can clone the repository. Alternatively, you can copy the script into a Python file on your local machine.

2. **Run the Game:**
   Open your terminal or command prompt, navigate to the directory containing the script, and run the following command:
   ```bash
   python blackjack.py
   ```
   This will start the game, and you will be prompted to input the number of games you want to play.

## Game Rules

- **Objective:** The goal is to have a hand value of 21 or as close to 21 as possible without exceeding it.
- **Card Values:**
  - Number cards (2-10) are worth their face value.
  - Face cards (Jack, Queen, King) are worth 10 points each.
  - Aces can be worth 11 points unless that would cause the hand to exceed 21, in which case they are worth 1 point.
- **Blackjack:** A hand is considered a Blackjack if it consists of an Ace and any 10-point card.
- **Gameplay:**
  - At the beginning of each game, both the player and the dealer receive two cards. The player's cards are both revealed, but the dealer's first card is hidden.
  - The player can choose to either "Hit" (take another card) or "Stand" (keep the current hand).
  - The player continues to hit or stand until they either stand or bust (hand value exceeds 21).
  - After the player stands, the dealer reveals their hidden card and must continue to hit until their hand value is at least 17.

## Code Structure

The game is divided into several classes to organize the different components:

- **Card Class:** Represents a single playing card with a suit and rank.
- **Deck Class:** Represents a deck of 52 cards and provides methods for shuffling and dealing cards.
- **Hand Class:** Represents the player's or dealer's hand and includes methods for adding cards, calculating hand value, and checking for Blackjack.
- **Game Class:** Handles the game loop, user input, and determines the outcome of each round.

## How to Play

1. **Start the game:** When you run the script, you'll be prompted to enter the number of games you want to play.
2. **Gameplay:** Follow the on-screen instructions to either "Hit" or "Stand" until the game determines the winner.
3. **Winning Conditions:**
   - You win if your hand is closer to 21 than the dealer's hand without exceeding 21.
   - You lose if your hand exceeds 21 (bust) or if the dealer's hand is closer to 21.
   - A tie occurs if both you and the dealer have the same hand value.

4. **End of Game:** After the chosen number of games have been played, the game will thank you for playing.

## Example Output

```plaintext
******************************
Game 1 of 3
******************************
Your hand:
10 of hearts
5 of spades
Value: 15

Dealer's hand:
hidden
4 of clubs

Please choose 'Hit' or 'Stand': hit

Your hand:
10 of hearts
5 of spades
3 of diamonds
Value: 18

Dealer's hand:
hidden
4 of clubs

Please choose 'Hit' or 'Stand': stand

Dealer's hand:
8 of diamonds
4 of clubs
9 of hearts
Value: 21

Dealer wins. 😭
```

## Conclusion

This Blackjack game is a simple yet enjoyable command-line implementation that offers a fun way to play the classic card game. Feel free to modify the code to add more features or customize the gameplay experience. Enjoy the game!