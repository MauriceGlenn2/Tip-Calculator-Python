# Tip-Calculator-Python

# 💸 Tip Calculator in Python

## 📝 Introduction
This project is a **Tip Calculator** built with Python. It allows users to:

- Enter the **total bill amount**
- Choose a **tip percentage** (e.g., 10%, 12%, 15%)
- Specify how many **people are splitting the bill**

The program calculates how much **each person should pay**, including their share of the tip.

---

## 🔍 What I Learned

### 🧮 Using `float` and `int`
- Learned how to convert user input:
  - `float()` for values like the total bill (which can include cents).
  - `int()` for whole number values like tip percentages and party size.
  - `round()` for rounding a number by inputting a number and specifying how many places you would like to round


```python
print("Welcome to the tip calculator!")
bill = float(input("What was the total bill? $"))
tip = int(input("What percentage tip would you like to give? 10%, 12%, 15% "))
people = int(input("How many people to split the bill? "))
tip_amount = round(((tip / 100) * bill + bill) / people, 2)

print(f"Each person should pay ${tip_amount:.2f}")
