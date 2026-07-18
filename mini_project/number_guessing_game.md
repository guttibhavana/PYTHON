# 🎯 Number Guessing Game

A simple command-line Python game where the computer generates a random number between **1 and 100**, and the player tries to guess it.

---

## 📌 Features

- Random number generation
- User input
- Gives hints (Too High / Too Low)
- Unlimited attempts
- Ends when the correct number is guessed

---

## 🛠️ Technologies Used

- Python 3
- Random Module

---

## 💻 Source Code

```python
import random

secret_number = random.randint(1,100)

while True:
    guess = int(input("Guess a number between 1 to 100: "))

    if guess == secret_number:
        print("Congrats! You guessed it right.")
        break
    elif guess < secret_number:
        print("Too Low! Try again.")
    else:
        print("Too High! Try again.")
```

---

## 🖥️ Sample Output

```
Guess a number between 1 to 100: 45
Too Low! Try again.

Guess a number between 1 to 100: 78
Too High! Try again.

Guess a number between 1 to 100: 62
Congrats! You guessed it right.
```

---

## 🧠 Concepts Used

- Variables
- User Input
- While Loop
- Conditional Statements (`if`, `elif`, `else`)
- Random Module
- Break Statement

---
