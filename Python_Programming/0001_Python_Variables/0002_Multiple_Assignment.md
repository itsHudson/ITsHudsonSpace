# Python Lesson — Multiple Assignment

---

# 1. What is Multiple Assignment?

This section explains what multiple assignment means in Python.

Multiple Assignment means assigning multiple values to multiple variables in a single line of code.

Instead of writing:

```python
a = 1
b = 2
```

Python allows:

```python
a, b = 1, 2
```

This makes code shorter and cleaner.

---

## 1.1 Basic Definition

This section explains the simplest meaning.

Multiple Assignment:

- Assign multiple variables at once
- Assign multiple values at once
- Python matches values based on position

Example:

```python
name, age = "Ali", 20
```

Meaning:

- `name → "Ali"`
- `age → 20`

---

## 1.2 Why It Exists

This section explains why Python provides this feature.

Without multiple assignment:

```python
x = 10
y = 20
z = 30
```

With multiple assignment:

```python
x, y, z = 10, 20, 30
```

Benefits:

| Benefit | Explanation |
| --- | --- |
| Less code | Fewer lines |
| Faster assignment | Assign many values quickly |
| Better readability | Cleaner structure |
| Easy swapping | Swap values easily |

---

# 2. Syntax of Multiple Assignment

This section explains the syntax structure.

General syntax:

```python
var1, var2 = value1, value2
```

Structure:

| Part | Explanation |
| --- | --- |
| Left side | Multiple variable names |
| Comma `,` | Separates variables |
| Right side | Multiple values |
| Equal sign `=` | Assignment operator |

Example:

```python
a, b = 1, 2
```

---

## 2.1 Three Variables Example

```python
x, y, z = 10, 20, 30
```

Output:

```python
print(x)
print(y)
print(z)
```

Output:

```python
10
20
30
```

---

# 3. How Multiple Assignment Works Internally

This section explains what happens behind the scenes.

Example:

```python
a, b = 1, 2
```

Step-by-step:

| Step | Process | Explanation |
| --- | --- | --- |
| 1 | Python reads assignment | Detects multiple variables |
| 2 | Creates values | Creates `1` and `2` |
| 3 | Matches by position | First variable gets first value |
| 4 | Links references | `a → 1`, `b → 2` |
| 5 | Stores variables | Assignment completed |

Final result:

```python
a = 1
b = 2
```

Equivalent to:

```python
a = 1
b = 2
```

---

# 4. Output Flow

This section explains how output works after multiple assignment.

Example:

```python
a, b = 1, 2

print(a)
print(b)
```

Step-by-step:

| Step | Code | Result |
| --- | --- | --- |
| 1 | `a, b = 1, 2` | Store values |
| 2 | `print(a)` | Print first variable |
| 3 | `print(b)` | Print second variable |

Output:

```python
1
2
```

---

# 5. Rules of Multiple Assignment

This section explains important rules.

---

## 5.1 Number Must Match

The number of variables must equal the number of values.

Correct:

```python
a, b = 1, 2
```

Wrong:

```python
a, b = 1
```

Error:

```python
ValueError
```

---

## 5.2 Order Matters

Python assigns based on position.

Example:

```python
a, b = 10, 20
```

Result:

| Variable | Value |
| --- | --- |
| `a` | 10 |
| `b` | 20 |

---

## 5.3 Use Commas

Correct:

```python
a, b = 1, 2
```

Wrong:

```python
a b = 1 2
```

---

## 5.4 Variables Must Follow Naming Rules

Correct:

```python
age1, age2 = 20, 30
```

Wrong:

```python
1age, 2age = 20, 30
```

---

# 6. Common Multiple Assignment Scenarios

This section explains real coding scenarios.

---

## 6.1 Basic Multiple Assignment

```python
a, b = 1, 2

print(a)
print(b)
```

Output:

```python
1
2
```

---

## 6.2 Assign Three Variables

```python
x, y, z = 10, 20, 30

print(x)
print(y)
print(z)
```

Output:

```python
10
20
30
```

---

## 6.3 Assign Different Data Types

Python allows different types.

```python
name, age, price = "Ali", 20, 99.9

print(name)
print(age)
print(price)
```

Output:

```python
Ali
20
99.9
```

---

## 6.4 Assign Boolean Values

```python
is_active, is_admin = True, False

print(is_active)
print(is_admin)
```

Output:

```python
True
False
```

---

## 6.5 Assign Using Expressions

```python
a, b = 2 + 3, 4 * 5

print(a)
print(b)
```

Step-by-step:

- `2 + 3 = 5`
- `4 * 5 = 20`

Output:

```python
5
20
```

---

## 6.6 Assign From User Input

```python
name, age = input("Enter name: "), input("Enter age: ")

print(name)
print(age)
```

Output:

Depends on user input.

---

# 7. Swapping Variables

This section explains one of Python’s most powerful multiple assignment features.

Traditional method:

```python
a = 10
b = 20

temp = a
a = b
b = temp
```

Python shortcut:

```python
a = 10
b = 20

a, b = b, a
```

Step-by-step:

| Step | Value |
| --- | --- |
| Before swap | `a=10`, `b=20` |
| Swap operation | `a,b = b,a` |
| After swap | `a=20`, `b=10` |

Output:

```python
20
10
```

---

# 8. Common Errors

This section explains beginner mistakes.

---

## 8.1 Too Few Values

```python
a, b = 1
```

Error:

```python
ValueError: not enough values to unpack
```

---

## 8.2 Too Many Values

```python
a, b = 1, 2, 3
```

Error:

```python
ValueError: too many values to unpack
```

---

## 8.3 Missing Commas

Wrong:

```python
a b = 1 2
```

Error:

```python
SyntaxError
```

---

## 8.4 Invalid Variable Names

Wrong:

```python
1a, 2b = 10, 20
```

Error:

```python
SyntaxError
```

---

# 9. Real-World Usage

This section explains where multiple assignment is used in real applications.

| Industry | Example |
| --- | --- |
| Gaming | `x, y = player_position` |
| Banking | `income, expense = data` |
| Data Science | `rows, cols = dataframe.shape` |
| Web Development | `username, password = login_data` |
| Machine Learning | `train_x, test_x = split_data` |

Example:

```python
username, password = "admin", "1234"

print(username)
print(password)
```

Output:

```python
admin
1234
```

---

# 10. Full Multiple Assignment Workflow

This section explains the full process.

Example: Student registration system

---

## Step 1 Input

```python
name, age, course = "Ali", 20, "Python"
```

---

## Step 2 Processing

Store values into separate variables.

| Variable | Value |
| --- | --- |
| `name` | Ali |
| `age` | 20 |
| `course` | Python |

---

## Step 3 Output

```python
print(name)
print(age)
print(course)
```

Output:

```python
Ali
20
Python
```

---

## Full Flow

```text
Input Values
→ Multiple Assignment
→ Variable Storage
→ Processing
→ Output
```

---

# 11. Evaluation Checklist

This section explains how to verify your code.

| Check | Question |
| --- | --- |
| Matching count | Same number of variables and values? |
| Correct syntax | Used commas properly? |
| Proper order | Values assigned correctly? |
| Good names | Variables meaningful? |
| Output correct | Printed expected results? |

---

# 12. Multiple Assignment vs Single Assignment

This section compares both approaches.

| Feature | Single Assignment | Multiple Assignment |
| --- | --- | --- |
| Number of variables | One at a time | Multiple at once |
| Lines of code | More | Less |
| Readability | Good | Cleaner for grouped values |
| Swapping support | Harder | Easier |

Example:

Single:

```python
a = 1
b = 2
```

Multiple:

```python
a, b = 1, 2
```

---

# 13. Summary

This section summarizes everything.

| Key Point | Explanation |
| --- | --- |
| Assign multiple variables | In one line |
| Order matters | Position-based assignment |
| Counts must match | Equal variables and values |
| Supports swapping | Very useful |
| Cleaner code | Reduces repetition |

Final concept:

```text
Multiple Values
→ Match Positions
→ Assign Variables
→ Use Variables
→ Output
```

Example:

```python
a, b = 1, 2
print(a)
print(b)
```

Output:

```python
1
2
```
