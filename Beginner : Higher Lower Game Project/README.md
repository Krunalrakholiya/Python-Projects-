Here’s the README content converted from Markdown to plain text:

---

Higher or Lower Search Game

Welcome to the Higher or Lower Search Game! This is a Python-based guessing game where players compare two accounts based on their search volume and guess which one has more followers. Test your intuition and see how high you can score!

Overview

In this game:
- Two accounts (A and B) are presented with their names, search volumes, and authors.
- You guess whether account A or B has more followers.
- Earn points for correct guesses and aim for a high score!
- The game continues until you make an incorrect guess.

This project is designed to be run in a Python environment like Google Colab or a local setup.

Features
- Random selection of accounts from a predefined dataset.
- Score tracking to monitor your progress.
- Feedback on each guess ("You're Right!" or "Sorry, That's wrong").
- Replayable game loop with shifting account comparisons.

Setup Instructions

Prerequisites
- Python 3.x installed.
- A dataset file (`game_data.py`) containing account information.

Running in Google Colab
1. Open the notebook in Google Colab.
2. Upload the `game_data.py` file to your Colab environment.
3. Run the following commands in a code cell to organize the files:
   !mkdir /content/content
   !mv /content/game_data.py /content/content/game_data.py
4. Execute the main game code.

Running Locally
1. Clone or download this repository.
2. Place the `game_data.py` file in a `content/` subdirectory.
3. Install Python (if not already installed).
4. Run the script in your terminal or IDE.

Usage

1. Import the required modules and data:
   from content.game_data import data
   import random
2. Run the game loop:
   - The game will display two accounts (A and B).
   - Type 'A' or 'B' to guess which has more followers.
   - Receive feedback and your updated score.
3. The game ends when you guess incorrectly, showing your final score.

Sample Output
Compare A: True Detective, a 450000, from Code Computerlove
Against B: Flamengo, a 9140000, from Agência Brasília
Who has more followers? Type 'A' or 'B':

File Structure
- `game_data.py`: Contains the `data` list with account details in the format:
  data = [
      {"keyword": "True Detective", "searchVolume": 450000, "author": "Code Computerlove", "follower_count": <number>},
      {"keyword": "Flamengo", "searchVolume": 9140000, "author": "Agência Brasília", "follower_count": <number>},
      ...
  ]
- `main.py` (or your script): The game logic and user interaction code.

How It Works
1. Random Account Selection: Two accounts are chosen randomly from `data`. Account B becomes Account A after each round.
2. Formatting: The `format_data()` function displays account details in a readable format.
3. Guessing: The user inputs 'A' or 'B' to guess which account has more followers.
4. Scoring: Correct guesses increment the score; an incorrect guess ends the game.

To-Do List
- [x] Display account details in a formatted way.
- [x] Generate random accounts from the dataset.
- [x] Ask the user for a guess.
- [ ] Fix the `is_correct` logic (currently undefined in the code).
- [ ] Add a welcome message or ASCII art (e.g., using `art` library).
- [ ] Allow the game to restart after completion.

Contributing
Feel free to fork this repository, submit pull requests, or suggest improvements via issues!

License
This project is open-source and available under the MIT License.

---
