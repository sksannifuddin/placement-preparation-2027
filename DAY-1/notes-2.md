# INPUT / OUTPUT IN PYTHON – COMPLETE PLACEMENT NOTES

## What is Input?

Input means accepting data from the user during program execution.

Example:

```python
name = input("Enter your name: ")
```

User enters:

```text
Sunny
```

Stored as:

```python
"Sunny"
```

---

## What is Output?

Output means displaying information to the user.

Example:

```python
print("Hello World")
```

Output:

```text
Hello World
```

---

## Why Input and Output Are Important?

Without Input and Output:

```text
No User Interaction
No Data Collection
No Result Display
```

Every real-world application uses Input and Output.

Examples:

```text
ATM Machine
Banking Application
Amazon Website
Food Delivery App
Machine Learning Projects
```

---

## input() Function

Used to take input from the user.

Syntax:

```python
variable = input()
```

Example:

```python
name = input("Enter Name: ")
```

---

## Internal Working of input()

When Python executes:

```python
name = input()
```

Steps:

```text
1. Program waits for input.
2. User enters value.
3. Python receives value as text.
4. String object is created.
5. Variable references that object.
```

Memory:

```text
name ───► "Sunny"
```

---

## Most Important Rule

## input() Always Returns String

Example:

```python
age = input()
```

User enters:

```text
20
```

Datatype:

```python
type(age)
```

Output:

```python
<class 'str'>
```

---

## Why input() Returns String?

Python cannot determine whether:

```text
20
```

should become:

```python
int
float
str
```

Therefore Python safely stores all input as string.

---

## Taking Integer Input

Example:

```python
age = int(input())
```

Input:

```text
20
```

Datatype:

```python
<class 'int'>
```

---

## Taking Float Input

Example:

```python
salary = float(input())
```

Input:

```text
50000.50
```

Datatype:

```python
<class 'float'>
```

---

## Taking Multiple Inputs

## Method 1

```python
a = int(input())
b = int(input())
```

---

## Method 2 (Interview Favorite)

```python
a,b = map(int,input().split())
```

Input:

```text
10 20
```

Output:

```python
a = 10
b = 20
```

---

## print() Function

Used to display output.

Example:

```python
print("Python")
```

Output:

```text
Python
```

---

## Printing Multiple Values

Example:

```python
name = "Sunny"
age = 20

print(name, age)
```

Output:

```text
Sunny 20
```

---

## sep Parameter

Used to change separator between values.

Example:

```python
print("A","B")
```

Output:

```text
A B
```

Custom Separator:

```python
print("A","B",sep="-")
```

Output:

```text
A-B
```

---

## end Parameter

Used to change line ending.

Default:

```python
print("Hello")
print("World")
```

Output:

```text
Hello
World
```

Custom:

```python
print("Hello",end=" ")
print("World")
```

Output:

```text
Hello World
```

---

## f-Strings

Modern way of formatting strings.

Example:

```python
name = "Sunny"

print(f"Hello {name}")
```

Output:

```text
Hello Sunny
```

---

## Multiple Variables with f-Strings

```python
name = "Sunny"
age = 20

print(f"My name is {name} and I am {age} years old")
```

Output:

```text
My name is Sunny and I am 20 years old
```

---

## Number Formatting

Example:

```python
pi = 3.14159265

print(f"{pi:.2f}")
```

Output:

```text
3.14
```

---

## String Concatenation vs Addition

## String Concatenation

```python
a = "10"
b = "20"

print(a+b)
```

Output:

```text
1020
```

---

## Numeric Addition

```python
a = 10
b = 20

print(a+b)
```

Output:

```text
30
```

---

## Memory Concept

Example:

```python
x = input()
```

User enters:

```text
100
```

Memory:

```text
x ───► "100"
```

Python stores user input as a string object.

---

## Common Mistakes

## Mistake 1

```python
age = input()

print(age + 10)
```

Output:

```python
TypeError
```

Reason:

```text
str + int is not allowed
```

---

## Mistake 2

```python
num = input()

print(num * 3)
```

Input:

```text
5
```

Output:

```text
555
```

String repetition occurs.

---

## Mistake 3

```python
a = input()
b = input()

print(a+b)
```

Input:

```text
10
20
```

Output:

```text
1020
```

Because both are strings.

---

## FAANG Interview Traps

## Trap 1

```python
num = input()

print(num + num)
```

Input:

```text
10
```

Output:

```text
1010
```

---

## Trap 2

```python
num = int(input())

print(num + num)
```

Input:

```text
10
```

Output:

```text
20
```

---

## Trap 3

```python
x = input()

print(bool(x))
```

Input:

```text
0
```

Output:

```python
True
```

Reason:

```text
"0" is a non-empty string
```

---

## Trap 4

```python
x = input()

print(type(x))
```

Input:

```text
True
```

Output:

```python
<class 'str'>
```

---

## Trap 5

```python
x = input()

print(x * 3)
```

Input:

```text
5
```

Output:

```text
555
```

---

## Real World Examples

## User Registration

```python
name = input("Enter Name: ")
age = int(input("Enter Age: "))
```

---

## Product Billing

```python
price = float(input())
quantity = int(input())

bill = price * quantity
```

---

## Student Marks

```python
marks = float(input())

print(marks)
```



---

## One-Line Revision

```text
input() always returns string.
Use int() or float() for numerical calculations.
print() displays output.
f-strings are preferred for formatting.
sep changes separator.
end changes line ending.
map() and split() help take multiple inputs.
```
