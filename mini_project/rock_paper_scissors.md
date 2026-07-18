# 🎮 Rock Paper Scissors Game (Python)

A simple command-line **Rock Paper Scissors** game built using Python. The user competes against the computer, which randomly selects its move.

---

## 📌 Features

- 🪨 Choose **Rock**
- 📄 Choose **Paper**
- ✂️ Choose **Scissors**
- 🤖 Computer selects a random choice
- 🏆 Displays whether you **Win**, **Lose**, or **Tie**

---

## 🛠️ Technologies Used

- Python 3
- Random Module

---

## source code 

```
import random

choices=["rock","paper","scissors"]

user= input("enter your choice:")

computer=random.choice(choices)

print("you choose:",user)
print("computer choose:",computer)

if user==computer:
    print("it's a tie")

elif (user=="rock" and computer=="scissors") or (user=="paper" and computer=="rock") or (user=="scissors" and computer=="paper"):
    print("you win!")
else:
    print("computer win!")
```


## 💻 Sample Output

```
Enter your choice: rock
You choose: rock
Computer choose: scissors
You win!
```

Another Example:

```
Enter your choice: paper
You choose: paper
Computer choose: paper
It's a tie
```

---

## 🧠 Game Rules

- Rock beats Scissors
- Scissors beats Paper
- Paper beats Rock
- If both choices are the same, the result is a Tie.

---

## 📚 Concepts Used

- Variables
- Lists
- User Input
- Conditional Statements (`if`, `elif`, `else`)
- Random Module
- Boolean Logic
