# TryHackMe- Python Basics
> Room Link: [TryHackMe - Python Basics](https://tryhackme.com/room/pythonbasics)
This room is a great intro to Python for beginners. It covers Variables, Loops, Functions, Data Structures, If statements and Files through short tasks. Here’s a walkthrough of each section with answers and brief explanations.

## Task 1: Introduction to Python 

In this room you will be introduced to python scripting needed for cyber security.
**Nothing to submit here, it is just showing the basic website for coding. You can explaore that website and you can even write a introductory code and submit.**

---

## Task 2: Hello World
In this task we will run the program using print() function.
'print()' function in Python displays output to the console or other standard output devices. It can output strings, numbers, and other data types, converting them to string representations if necessary.
On code editor we will type "print("Hello World")" to get the flag needed for solving the question. Strings must be kept in quotation marks.
**Question**: On the code editor, print "Hello World". What is the flag?
**Answer**: THM{PRINT_STATEMENTS}

---

## Task 3: Mathematical Operators
This task introduces **basic arithmetic and comparison operators** in Python — similar to what you'd use in a calculator, but more powerful when combined with logic.

### Arithmetic Operators

| Operation      | Symbol | Example           | Result |
|----------------|--------|-------------------|--------|
| Addition       | `+`    | `1 + 1`           | `2`    |
| Subtraction    | `-`    | `5 - 1`           | `4`    |
| Multiplication | `*`    | `10 * 10`         | `100`  |
| Division       | `/`    | `10 / 2`          | `5.0`  |
| Modulus        | `%`    | `10 % 2`          | `0`    |
| Exponentiation | `**`   | `5 ** 2` (5²)     | `25`   |

### Comparison Operators
| Condition                     | Symbol |
|------------------------------|--------|
| Greater than                 | `>`    |
| Less than                    | `<`    |
| Equal to                     | `==`   |
| Not equal to                 | `!=`   |
| Greater than or equal to     | `>=`   |
| Less than or equal to        | `<=`   |
These operators are especially useful in `if` statements and loops.

**Questions:**
**Q1**: In the code editor, print the result of 21 + 43. What is the flag?
So we will assign the given intergers to the variables like a, b and c to solve the problem.
a=21
b=43
c=a+b
print(c) //this is one way for easy understanding
or directly by typing "print(21+43)"
**Flag**: THM{ADDITI0N}

**Q2**: Print the result of 142 - 52. What is the flag?
print(142-52)
**Flag**: THM{SUBTRCT}

**Q3**: Print the result of 10 * 342. What is the flag?

```python
print(10*342)  #multiplication
```
**Flag**: THM{MULTIPLICATION_PYTHON}

**Q4**: Print the result of 5 squared. What is the flag?
print(5**2)  //The double asterisk ** in Python serves primarily as the exponentiation operator. It calculates the result of raising the number on its left to the power of the number on its right. For instance, x ** y computes x raised to the power of y. 
**Flag**: THM{EXP0N3NT_POWER}

---

## Task 4: Variables and Datatypes
Variables are containers that store information. You can store different types of data and modify them as needed throughout a Python program.
Example:

```python
food = "ice cream"  # String
money = 2000        # Integer
```
