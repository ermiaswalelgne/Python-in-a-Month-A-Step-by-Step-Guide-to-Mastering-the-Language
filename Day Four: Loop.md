###### ⬅[Home||](https://github.com/ermiaswalelgne/Python-in-a-Month-A-Step-by-Step-Guide-to-Mastering-the-Language)

# Welcome to Day 4 of the 30-day Python course! Today, we will cover loops in Python.

## Loops:
Loops are used to execute a block of code repeatedly. There are two types of loops in Python: "for" loops and "while" loops.

## For Loops:
A for loop is used to iterate over a sequence, such as a list or a string. The general syntax for a for loop is as follows:

```python
for variable in sequence:
    # code to be executed for each item in the sequence
````
For example, let's say we want to iterate over a list of numbers and print out each number. We can do this with a for loop like so:

```python
numbers = [1, 2, 3, 4, 5]
for num in numbers:
    print(num)
````

This will print out the numbers 1 through 5.

## While Loops:
A while loop is used to repeatedly execute a block of code as long as a certain condition is true. The general syntax for a while loop is as follows:

```python
while condition:
    # code to be executed while the condition is true
````

For example, let's say we want to repeatedly ask the user for input until they enter a valid response. We can do this with a while loop like so:


````python
valid_input = False
while not valid_input:
    user_input = input("Enter a number: ")
    if user_input.isdigit():
        valid_input = True
    else:
        print("Invalid input. Please enter a valid number.")
````

This will continue to prompt the user to enter a number until they enter a valid number.

## Loop Control Statements:
Sometimes, you may need to modify the behavior of a loop based on certain conditions. Python provides several loop control statements to help with this.

The "break" statement is used to exit a loop prematurely. For example, let's say we want to search for a particular value in a list and stop once we find it:

```python
numbers = [1, 2, 3, 4, 5]
search_value = 3

for num in numbers:
    if num == search_value:
        print("Found it!")
        break
````

This will print "Found it!" and exit the loop once the search value is found.

The "continue" statement is used to skip the current iteration of a loop and move on to the next one. For example, let's say we want to print out all the even numbers in a list:

```python
numbers = [1, 2, 3, 4, 5]

for num in numbers:
    if num % 2 != 0:
        continue
    print(num)
````

This will print out the even numbers 2 and 4.

Loops are an essential tool for any programmer, and can help you solve many different types of problems. 
With for loops and while loops, as well as loop control statements like break and continue, you can start to write more complex and interesting programs. Stay tuned for Day 5, where we will cover List in Python.

###### ⬅[Home||](https://github.com/ermiaswalelgne/Python-in-a-Month-A-Step-by-Step-Guide-to-Mastering-the-Language)
