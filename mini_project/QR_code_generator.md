# 📱 QR Code Generator (Python)

A simple Python application that generates a QR code from any text or URL entered by the user and saves it as a PNG image.

---

## 📌 Features

- Generate QR codes from text or URLs.
- Save the QR code as a PNG image.
- User-defined file name.
- Fast and easy to use.
- Command-line interface.

---

## 🛠️ Technologies Used

- Python 3
- `qrcode` Library
- Pillow (PIL)

---

## 💻 Source Code

```python
import qrcode

print("--- QR CODE GENERATOR ---")

data = input("Enter text or URL: ")

img = qrcode.make(data)

file_name = input("Enter file name: ")

img.save(file_name + ".png")

print("QR CODE GENERATED SUCCESSFULLY!")
print(f"Saved as: {file_name}.png")
```

---

## 📸 Sample Output

```
--- QR CODE GENERATOR ---

Enter text or URL: https://github.com/guttibhavana
Enter file name: github_qr

QR CODE GENERATED SUCCESSFULLY!
Saved as: github_qr.png
```

---

## 🧠 How It Works

1. The user enters any text or URL.
2. The program generates a QR code using the `qrcode` library.
3. The user provides a file name.
4. The QR code is saved as a PNG image in the current directory.

---

## 📚 Concepts Used

- User Input
- Variables
- Python Modules
- File Handling
- QR Code Generation
- Image Saving

---

## 📦 Required Library

Install the required library before running the program:

```bash
pip install qrcode[pil]
```
