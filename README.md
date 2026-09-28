# 🎰 Python Slot Machine

A simple **console-based Slot Machine game built with Python**.
The project demonstrates Python fundamentals such as functions, loops, dictionaries, random numbers, input validation, and basic game logic.

## 📌 Project Overview

This project simulates a 3×3 slot machine where the player:

1. Deposits an amount of money.
2. Selects how many lines to bet on.
3. Chooses the bet amount.
4. Spins the slot machine.
5. Checks whether the selected lines contain matching symbols.
6. Receives winnings based on the matching symbol and bet amount.

## 🎮 Features

* 💰 Deposit money into the game
* 🎯 Select 1–3 betting lines
* 💵 Set a bet between ₹100 and ₹1000 per line
* 🎰 Random slot machine generation
* 🏆 Automatic winning calculation
* 📊 Different values for different symbols
* ✅ Input validation
* 🐍 Built completely with Python

## 🛠️ Technologies Used

* **Python 3**
* `random` module
* Functions
* Loops
* Dictionaries
* Conditional statements
* Input validation


## ⚙️ How It Works

### 1. Symbol Count

The game uses four symbols:

```python
symbol_count = {
    "A": 2,
    "B": 4,
    "C": 6,
    "D": 8
}
```

The number represents how frequently each symbol appears.

### 2. Symbol Value

Each symbol has a different winning value:

```python
symbol_value = {
    "A": 5,
    "B": 4,
    "C": 3,
    "D": 2
}
```

The rarer symbols have higher values.

### 3. Betting

The player can select between **1 and 3 lines**.

The bet per line must be between:

```text
₹100 - ₹1000
```

The total bet is calculated as:

```python
total_bet = bet * lines
```

### 4. Slot Machine Spin

The program randomly generates a 3×3 slot machine using Python's `random` module.

Example:

```text
A | D | B
C | D | A
B | D | C
```

### 5. Winning Logic

The program checks each selected row.

For example:

```text
A | A | A
B | C | D
C | C | C
```

If the player selected 3 lines, lines **1 and 3** are winning lines.

The winnings are calculated using:

```python
winnings += values[symbol] * bet
```

## 💻 Example

```text
What would you like to deposit: ₹ 1000

Enter the number of lines to bet on (1-3)? 2

What would you like to bet on line? : ₹ 100

You are betting ₹100 on 2 lines.
Total bet is equal to ₹200

Your slot machine:

A | D | B
C | D | A
B | D | C

You won ₹0.
You won on lines: []
```

## 🚀 Future Improvements

Possible improvements for future versions:

* [ ] Add multiple rounds
* [ ] Deduct the bet from the player's balance
* [ ] Allow the player to play again
* [ ] Add a quit option
* [ ] Add more symbols
* [ ] Add sound effects
* [ ] Add a graphical user interface
* [ ] Add animations
* [ ] Add a betting history
* [ ] Add a final balance display

## 📚 What I Learned

While building this project, I learned how to combine Python fundamentals to create a small interactive application.

The project particularly helped me understand **functions, loops, dictionaries, random number generation, input validation, and program flow**.

