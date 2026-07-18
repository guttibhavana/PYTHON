# 🎓 Student Marks Calculator (Python)

A simple Python program that calculates a student's total marks, average, percentage, and pass/fail result based on marks entered for three subjects.

---

## 📌 Features

- Accepts student name.
- Takes marks for three subjects.
- Calculates:
  - Total Marks
  - Average Marks
  - Percentage
- Displays Pass or Fail based on percentage.

---

## 🛠️ Technologies Used

- Python 3

---

## source code 

```
name=input("student name")

sub1= int(input("subject 1 marks"))
sub2= int(input("subject 2 marks"))
sub3= int(input("subject 3 marks"))

total= sub1+sub2+sub3
average-total/3
percentage = (total/300) *100

print("\n student:")
print("Total:" , total)
print("Average:",average)
print("Percentage:",percentage)

if percentage>=35:
    print("Pass")

else:
    print("Fail")
```


## 💻 Sample Output

```
Enter student name: Bhavana
Enter Subject 1 marks: 85
Enter Subject 2 marks: 90
Enter Subject 3 marks: 95

Student Report
Student Name: Bhavana
Total: 270
Average: 90.0
Percentage: 90.0 %
Result: Pass
```

---

## 🧠 Concepts Used

- Variables
- User Input
- Arithmetic Operations
- Conditional Statements (`if`/`else`)
- Output Formatting

---
