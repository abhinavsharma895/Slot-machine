# 🎰 Python Slot Machine

A simple **console-based Slot Machine game built with Python**.
The project demonstrates Python fundamentals such as functions, loops, dictionaries, lists, randomization, input validation, and basic game logic.

## 📌 Features

* 💰 Deposit an initial balance
* 🎰 3 × 3 slot machine
* 🎯 Choose how many lines to bet on
* 💵 Set a bet amount for each line
* 🏆 Calculate winnings based on matching symbols
* 📊 Display winning lines
* 🔄 Play multiple rounds
* 🚪 Quit the game whenever you want
* ✅ Input validation for deposits, lines, and bets
* 💸 Prevents betting more than the available balance


## 🎮 How the Game Works

The slot machine contains four symbols:

| Symbol | Count | Value |
| ------ | ----- | ----- |
| A      | 2     | ₹5    |
| B      | 4     | ₹4    |
| C      | 6     | ₹3    |
| D      | 8     | ₹2    |

The game uses these symbols to generate a random **3 × 3 slot machine**.

### Winning Rule

A line is considered a winning line when all symbols in that row are the same.

For example:

```text
A | A | A
B | C | D
C | B | D
```

The first row is a winning line because all three symbols are `A`.

The winnings are calculated using:

```text
Symbol Value × Bet
```

For example:

```text
A = ₹5
Bet = ₹100

Winnings = ₹5 × ₹100
         = ₹500
```

## 💰 Betting System

The game has the following limits:

```python
MAX_LINES = 3
MAX_BET = 10000
MIN_BET = 100
```

This means:

* Minimum bet per line: **₹100**
* Maximum bet per line: **₹10,000**
* Maximum betting lines: **3**

If you choose 3 lines and bet ₹100 per line:

```text
Total Bet = ₹100 × 3
          = ₹300
```

The game also checks whether your balance is sufficient before allowing the bet.



## 🧠 Concepts Learned

This project helped practice several important Python concepts:

### Variables

```python
MAX_LINES = 3
MAX_BET = 10000
MIN_BET = 100
```

### Dictionaries

```python
symbol_count = {
    "A": 2,
    "B": 4,
    "C": 6,
    "D": 8
}
```

### Functions

```python
def deposit():
    ...
```

```python
def get_bet():
    ...
```

```python
def spin(balance):
    ...
```

### Loops

The project uses both `for` and `while` loops for:

* Generating slots
* Validating input
* Running multiple game rounds

### Randomization

The Python `random` module is used to generate random slot results:

```python
value = random.choice(current_symbols)
```

### Input Validation

The program checks whether the user enters valid numbers and whether the bet is within the allowed range.

## 🔮 Future Improvements

Possible improvements for this project:

* [ ] Add colorful terminal output
* [ ] Add a spinning animation
* [ ] Add multiple types of winning combinations
* [ ] Add diagonal winning lines
* [ ] Add jackpot rewards
* [ ] Add sound effects
* [ ] Add game statistics
* [ ] Add a leaderboard
* [ ] Add a graphical user interface using Tkinter
* [ ] Add unit tests
* [ ] Improve the betting and reward system

