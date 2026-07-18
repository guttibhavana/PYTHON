# 🎯 Number Guessing Game (Python)

A fun command-line Python game where the computer randomly selects a number between **1 and 100**, and the player tries to guess it with hints after each attempt.

---

## 📌 Features

- Generates a random number between **1 and 100**.
- Accepts user guesses.
- Provides hints:
  - 📉 Too Low
  - 📈 Too High
- Continues until the correct number is guessed.
- Congratulates the player upon winning.

---

## 🛠️ Technologies Used

- Python 3
- Random Module

---

## 💻 Sample Output

```
Guess a number between 1 and 100: 45
Too Low! Try again.

Guess a number between 1 and 100: 78
Too High! Try again.

Guess a number between 1 and 100: 62
Congratulations! You guessed it right.
```

---

## 🧠 How It Works

1. The computer generates a random number between **1 and 100**.
2. The user enters a guess.
3. If the guess is:
   - Less than the secret number → "Too Low!"
   - Greater than the secret number → "Too High!"
   - Equal to the secret number → The user wins.
4. The game continues until the correct number is guessed.

---

## 📚 Concepts Used

- Variables
- User Input
- `while` Loop
- Conditional Statements (`if`, `elif`, `else`)
- Random Module
- Loop Control (`break`)

---
