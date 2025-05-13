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
```python
print("Hello World")
```
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
```python
a=21
b=43
c=a+b
print(c) #this is one way for easy understanding
```
or 
```python
print(21+43)
```
**Flag**: THM{ADDITI0N}

**Q2**: Print the result of 142 - 52. What is the flag?
```python
print(142-52)
```
**Flag**: THM{SUBTRCT}

**Q3**: Print the result of 10 * 342. What is the flag?

```python
print(10*342)  #multiplication
```
**Flag**: THM{MULTIPLICATION_PYTHON}

**Q4**: Print the result of 5 squared. What is the flag?
```python
print(5**2)  
```
The double asterisk ** in Python serves primarily as the exponentiation operator. It calculates the result of raising the number on its left to the power of the number on its right. For instance, x ** y computes x raised to the power of y. 
**Flag**: THM{EXP0N3NT_POWER}

---

## Task 4: Variables and Datatypes
### Variables
Variables are containers that store information. You can store different types of data and modify them as needed throughout a Python program.
Example:

```python
food = "ice cream"  # String
money = 2000        # Integer
```
You can also update variables:
```python
age = 30
age = age + 1
print(age)  # Output: 31
```

### Datatypes
|Data Type|	Example	        |Python Syntax Example     |
|---------|-----------------|--------------------------|
|String	  |"Star Wars"	    |title = "Star Wars"       |
|Float	  |9.8	            |rating = 9.8              |
|Integer	|13	              |views = 13                |
|Boolean	|True, False	    |favorite = True           |
|List	    |["Alice", "Bob"]	|seen_by = ["Alice", "Bob"]|

**Questions:**
Step 1: Create a variable called height and set its value to 200
Step 2: On a new line, add 50 to height
Step 3: Print the value of height
```python
height = 200
height = height + 50
print(height)
```
**Q1**: In the code editor, create a variable called height and set its initial value to 200.
**A**: *No answer needed*

**Q2**: On a new line, add 50 to the height variable.
**A**: *No answer needed*

**Q3**: On another new line, print out the value of height. What is the flag that appears?
**Flag**: THM{VARIABL3S}

---

## Task 5: Logical and Boolean Operators
Logical and Boolean operators are essential for **decision-making** in Python. They help control the flow of your program using conditions.

### Logical Operators (Comparison)

| Operation              | Operator | Example      | Meaning                            |
|------------------------|----------|--------------|------------------------------------|
| Equal to               | `==`     | `x == 5`     | True if x equals 5                 |
| Less than              | `<`      | `x < 5`      | True if x is less than 5           |
| Less than or equal to  | `<=`     | `x <= 5`     | True if x is 5 or less             |
| Greater than           | `>`      | `x > 5`      | True if x is greater than 5        |
| Greater than or equal  | `>=`     | `x >= 5`     | True if x is 5 or more             |

### Boolean Operators (Logical)

| Operation | Keyword | Example                          | Meaning                                                |
|-----------|---------|----------------------------------|--------------------------------------------------------|
| AND       | `and`   | `x >= 5 and x <= 100`            | True if both conditions are True                      |
| OR        | `or`    | `x == 1 or x == 10`              | True if at least one condition is True                |
| NOT       | `not`   | `if not y`                       | True if `y` is False                                  |

### Example Code

```python
a = 1
if a == 1 or a > 10:
    print("a is either 1 or above 10")

name = "bob" 
hungry = True

if name == "bob" and hungry == True:
    print("bob is hungry")
elif name == "bob" and not hungry:
    print("Bob is not hungry")
else:
    print("Not sure who this is or if they are hungry")
```

*No flag was needed*

---

## Task 6: Introduction to If statements(Shipping Project)
In this task, we explore **conditional logic** using `if` statements in Python. These allow a program to **make decisions** and execute specific blocks of code based on certain conditions.

### What are If Statements?
```python
age = 16
if age < 17:
    print('You are NOT old enough to drive')
else:
    print('You are old enough to drive')
```
### Key Concepts
- if: starts the condition check.
- else: fallback if the if condition is not met.
- :: ends the condition line.
- Indentation: Everything indented after the condition runs if the condition is true.

**Questions:**
**Q1**: In this exercise, we will code a small application that calculates and outputs the shipping cost for a customer based on how much they've spent.
In the code editor, click on the "shipping.py" tab and follow the instructions to complete this task.
*No answer needed*

**Q2**: Once you've written the application in the code editor's shipping.py tab, a flag will appear, which is the answer to this question.
```python
customer_basket_cost = 34
customer_basket_weight = 44

# Write if statement here to calculate the total cost

if customer_basket_cost>100:
  total_cost=customer_basket_cost
else:
  shipping_cost=1.20*customer_basket_weight
  total_cost=customer_basket_cost+shipping_cost
print(total_cost)
```
**A**: THM{IF_STATEMENT_SHOPPING}

**Q3**: In shipping.py, on line 15 (when using the Code Editor's Hint), change the customer_basket_cost variable to 101 and re-run your code. You will get a flag (if the total cost is correct based on your code); the flag is the answer to this question.
```python
customer_basket_cost = 101
customer_basket_weight = 44

# Write if statement here to calculate the total cost

if customer_basket_cost>100:
  total_cost=customer_basket_cost
else:
  shipping_cost=1.20*customer_basket_weight
  total_cost=customer_basket_cost+shipping_cost
print(total_cost)
```
**A**: THM{MY_FIRST_APP}

---

## Task 7: Loops
In this task, we explore **loops**, which allow us to repeat actions in Python. Loops are crucial when we want to automate repetitive tasks like printing a sequence of numbers, iterating over lists, or checking conditions repeatedly.
### While loops
A `while` loop continues to run **as long as a condition is true**.

```python
i = 1
while i <= 10:
    print(i)
    i = i + 1
```
This code:
- Starts with i = 1
- Repeats printing i and increasing its value by 1
- Stops when i > 10

### For Loop 
A for loop is typically used to iterate over sequences, such as lists or ranges.
```python
websites = ["facebook.com", "google.com", "amazon.com"]
for site in websites:
    print(site)
```
This code:
- Loops through each website in the list
- Prints them one by one

### Using range()
The range() function is used to generate a sequence of numbers. This loop prints numbers from 0 to 4.
```python
for i in range(5):
    print(i)
```
**Q1**: On the code editor, click back on the "script.py" tab and code a loop that outputs every number from 0 to 50.
**A**: THM{L00PS_WHILE_FOR}

---

## Task 8: Introduction to Functions(Bitcoin Project)
In this task, I learned how to use **functions** in Python to organize and reuse code efficiently. Functions help avoid repetition and make code easier to manage and understand.

### What is a Function?
Functions are reusable blocks of code. A function:
- Begins with the `def` keyword
- Has a name
- May accept input parameters (inside `()`)
- Contains code that's indented
- Can optionally `return` a result

### Example Function
```python
def sayHello(name):
    print("Hello " + name + "! Nice to meet you.")

sayHello("Ben")  # Output: Hello Ben! Nice to meet you.
```
**Questions**
**Q1**: You've invested in Bitcoin and want to write a program that tells you when the value of Bitcoin falls below a particular value in dollars.

In the code editor, click on the bitcoin.py tab. Write a function called bitcoinToUSD with two parameters: bitcoin_amount, the amount of Bitcoin you own, and bitcoin_value_usd, the value of bitcoin in USD. The function should return usd_value, which is your bitcoin value in USD (to calculate this, in the function, you times bitcoin_amount variable by bitcoin_value_usd variable and return the value). The start of the function should look like this:
```python
def bitcoinToUSD(bitcoin_amount, bitcoin_value_usd):
```
Once you've written the bitcoinToUSD function, use it to calculate the value of your Bitcoin in USD, and then create an if statement to determine if the value falls below $30,000; if it does, output a message to alert you (via a print statement).
```python
investment_in_bitcoin = 1.2
bitcoin_to_usd = 40000

# 1) write a function to calculate bitcoin to usd
def bitcoinToUSD(bitcoin_amount, bitcoin_value_usd):
  return bitcoin_amount * bitcoin_value_usd
# 2) use function to calculate if the investment is below $30,000
usd_value = bitcoinToUSD(investment_in_bitcoin, bitcoin_to_usd)
if usd_value < 30000:
    print("Alert: Your Bitcoin investment is below $30,000!")
else:
    print("Your Bitcoin investment is above $30,000.")
print("Current USD Value:", usd_value)
```
**A**: THM{BITC0IN_INVESTOR}

---

## Task 9: File Handling in Python
In this task, we will learn how to read and write from files using Python. In cybersecurity, handling files is common, such as when you need to import or export lists of websites or store script output to a file.
## Reading from a File
To open a file and read its contents in Python, we use the `open()` function. Here is an example of how to read the contents of a file:

```python
# Open the file in read mode
with open("flag.txt", "r") as f:
    flag = f.read().strip() 
print(flag)
```
**Q**: In the code editor, write Python code to read the flag.txt file. What is the flag in this file?
**A**: THM{F1LE_R3AD}

---

## Task 10: Imports in Python
In this task, we learn how to **import libraries** in Python. Libraries are collections of pre-written code (functions and classes) that help us accomplish tasks without writing everything from scratch.

### Example: Importing the `datetime` Library
Python includes a standard library called `datetime` that allows us to work with dates and times. Below is a basic example:
```python
import datetime
current_time = datetime.datetime.now()
print(current_time)
```
### Explanation:
- import datetime brings the datetime module into your script.
- datetime.datetime.now() accesses the now() method from the datetime class inside the datetime module to get the current system time.
- print(current_time) displays the current date and time.

---

## Commonly Used Libraries for Pentesters
Below are some popular libraries frequently used in cybersecurity scripting:

|Library	 | Description                                                      |
|----------|------------------------------------------------------------------|
|requests  | Simple HTTP library to send web requests.                        |
|scapy	   | For crafting, sending, sniffing, and dissecting network packets. |
|pwntools  |	Useful for CTFs and exploit development.                        |

# Conclusion
Python imports make it easy to reuse powerful code libraries, whether for automation, pentesting, or general scripting. This task demonstrates how to work with the datetime library and introduces other useful libraries relevant to penetration testing.
