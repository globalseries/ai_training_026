# 🐍 Week 2: Python Basics for AI

Welcome to **Week 2** of the **AI Foundations to Generative AI** course.

This week, you'll learn Python—the most popular programming language in Artificial Intelligence and Data Science. By the end of the week, you'll be able to write simple programs, make decisions with code, use loops, create functions, and build your first mini project.

---

# 🎯 Learning Objectives

By the end of this week, you will be able to:

* Understand why Python is widely used in AI
* Write and run Python programs
* Use variables and data types
* Accept user input and display output
* Apply conditional statements (if-else)
* Use loops for repetition
* Create reusable functions
* Work with strings and lists
* Build a simple Python project

---

# 📚 Why Python?

Python is the most popular language for AI because it is:

* Easy to read and write
* Beginner-friendly
* Open source and free
* Supported by a massive AI ecosystem
* Used by companies like Google, OpenAI, Netflix, NASA, and Meta

### Popular Python Libraries

* NumPy
* Pandas
* Matplotlib
* Scikit-Learn
* TensorFlow
* PyTorch

---

# 🚀 Setup Options

Choose one of the following:

## Option 1: Google Colab (Recommended)

* Runs in your browser
* No installation required
* Free access to GPUs
* Perfect for beginners

## Option 2: Python + VS Code

* Install Python from python.org
* Install Visual Studio Code
* Professional development setup

## Option 3: Anaconda

* Includes Python and Jupyter Notebook
* Popular among Data Scientists

---

# 👋 Your First Python Program

```python
print("Hello, AI World!")

name = "Your Name"

print(f"Hello, {name}!")
print("You are now a programmer.")
```

### Concepts Learned

* `print()` displays output
* Comments start with `#`
* Variables store information
* f-strings allow dynamic text formatting

---

# 📦 Variables

Variables are containers that store data.

```python
name = "Sita"
age = 21
height = 5.4
is_student = True

print(f"{name} is {age} years old.")
```

### Naming Rules

✅ Good

```python
student_name
total_marks
```

❌ Avoid

```python
1name
student name
```

---

# 🔢 Data Types

## String (str)

```python
name = "Python"
```

Used for text.

---

## Integer (int)

```python
age = 25
```

Used for whole numbers.

---

## Float

```python
price = 99.99
```

Used for decimal values.

---

## Boolean (bool)

```python
is_active = True
```

Used for True or False values.

---

# ⌨️ Input and Output

```python
name = input("Enter your name: ")

print(f"Hello, {name}")
```

### Converting Input

```python
age = int(input("Enter your age: "))

years_to_50 = 50 - age

print(f"You will be 50 in {years_to_50} years.")
```

---

# 🔀 Conditional Statements

Python can make decisions using if-else.

```python
age = int(input("Enter age: "))

if age >= 18:
    print("You can vote.")
else:
    print("Not eligible.")
```

### Multiple Conditions

```python
score = 85

if score >= 90:
    grade = "A"
elif score >= 75:
    grade = "B"
elif score >= 60:
    grade = "C"
else:
    grade = "F"

print(grade)
```

---

# 🔁 Loops

Loops allow us to repeat tasks.

## For Loop

```python
for i in range(5):
    print(i)
```

Output:

```text
0
1
2
3
4
```

---

## Loop Through a List

```python
fruits = ["apple", "banana", "mango"]

for fruit in fruits:
    print(fruit)
```

---

## While Loop

```python
guess = 0

while guess != 7:
    guess = int(input("Guess a number: "))

print("Correct!")
```

---

# ⚙️ Functions

Functions help us reuse code.

```python
def greet(name):
    return f"Hello, {name}"

print(greet("Ram"))
```

---

## Function with Multiple Parameters

```python
def calculate_tip(bill, percent):
    tip = bill * (percent / 100)
    return round(tip, 2)

print(calculate_tip(500, 10))
```

---

# 📝 Strings

Strings are one of the most important data types in AI.

```python
text = "Hello AI World"
```

### Common String Methods

```python
text.upper()
text.lower()
text.title()
```

### Length

```python
len(text)
```

### Split

```python
words = text.split()
```

### Replace

```python
text.replace("AI", "ML")
```

### Search

```python
"AI" in text
```

---

# 📋 Lists

Lists store multiple values.

```python
fruits = ["apple", "banana", "mango"]
```

### Access Items

```python
fruits[0]
fruits[-1]
```

### Add Items

```python
fruits.append("kiwi")
```

### Remove Items

```python
fruits.remove("banana")
```

### Length

```python
len(fruits)
```

### Loop Through List

```python
for fruit in fruits:
    print(fruit)
```

---

# 🔐 Mini Project: Password Strength Checker

```python
def check_password(password):

    if len(password) < 6:
        return "Weak"

    has_digit = any(c.isdigit() for c in password)
    has_upper = any(c.isupper() for c in password)
    has_special = any(c in "!@#$%^&*" for c in password)

    score = sum([has_digit, has_upper, has_special])

    if score == 3:
        return "Strong"
    elif score == 2:
        return "Medium"
    else:
        return "Weak"
```

### Concepts Used

* Functions
* Conditions
* Loops
* Strings
* Boolean Logic

---

# ❌ Common Beginner Mistakes

| Mistake                    | Fix                                     |
| -------------------------- | --------------------------------------- |
| Missing colon `:`          | Always end if, for, while, def with `:` |
| Using `=` instead of `==`  | `=` assigns, `==` compares              |
| Mixed tabs and spaces      | Use 4 spaces consistently               |
| Forgetting type conversion | Use `int()` or `float()`                |
| Range confusion            | `range(5)` → 0,1,2,3,4                  |

---

# 🐞 Reading Errors

Common Python Errors:

* SyntaxError
* NameError
* TypeError
* IndentationError

### Tip

Read the error message from bottom to top. The last line usually tells you what went wrong.

---

# 🚀 Modern Python in 2026

## AI-Assisted Coding

Popular tools:

* GitHub Copilot
* Claude Code
* Cursor
* ChatGPT

These tools can:

* Suggest code
* Explain errors
* Generate functions
* Improve productivity

Remember:

> AI is a copilot, not an autopilot.

---

## Modern Notebook Workflows

Popular tools:

* Google Colab
* Jupyter Notebook
* Marimo
* Deepnote

---

## Modern Python Tooling

### uv

Fast Python package manager.

### Ruff

Fast linter and formatter.

### Type Hints

Helps detect bugs before execution.

---

# 📝 Week 2 Assignment: Mini Project

Choose ONE project and submit your Colab or GitHub link before Week 3.

## 🟢 Beginner: Calculator

Build a calculator that supports:

* Addition
* Subtraction
* Multiplication
* Division

### Bonus

Handle division by zero.

---

## 🔵 Intermediate: Grade System

Input marks from 3 subjects.

Output:

* Total
* Percentage
* Grade
* Remarks

### Bonus

Support multiple students.

---

## 🟠 Advanced: Password Checker

Create a password strength checker.

Check for:

* Minimum length
* Uppercase letters
* Numbers
* Special characters

### Bonus

Detect common weak passwords.

---

# 📅 Submission

Submit before the start of **Week 3**.

Share:

* Google Colab Link
  OR
* GitHub Repository Link

---

# 🔑 Key Takeaways

1. Python is simple, readable, and powerful.
2. Five core building blocks:

   * Variables
   * Data Types
   * Conditionals
   * Loops
   * Functions
3. Errors are learning opportunities.
4. AI can assist coding, but understanding code is essential.

---

# ⏭️ Next Week

## Week 3: Data Analysis with Python

Coming up:

* NumPy
* Pandas
* Data Cleaning
* CSV Files
* Data Visualization
* Real-world Datasets

Get ready to make data come alive! 📊🚀
