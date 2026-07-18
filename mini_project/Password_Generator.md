# 🔐 Random Password Generator (Python)

A simple Python program that generates a secure random password of a user-specified length using letters, digits, and special characters.

---

## 📌 Features

- Generates a random password.
- User specifies the password length.
- Includes:
  - 🔤 Uppercase & Lowercase Letters
  - 🔢 Digits
  - 🔣 Special Characters
- Uses Python's built-in `random` and `string` modules.

---

## 🛠️ Technologies Used

- Python 3
- Random Module
- String Module

---

## 💻 Source Code

```python
import random
import string

length = int(input("Enter password length: "))

characters = string.ascii_letters + string.digits + string.punctuation

password = ""

for i in range(length):
    password += random.choice(characters)

print("Generated password:", password)
```

---

## 💻 Sample Output

```
Enter password length: 12
Generated password: A@7kP#2x!Lm9
```

Another Example:

```
Enter password length: 8
Generated password: t$8Qw!2Z
```

---

## 🧠 How It Works

1. The user enters the desired password length.
2. The program combines uppercase letters, lowercase letters, digits, and special characters into a single character set.
3. It randomly selects characters from this set based on the specified length.
4. The generated password is displayed to the user.

---

## 📚 Concepts Used

- Variables
- User Input
- `for` Loop
- String Concatenation
- Random Module
- String Module

---
