# Welcome to Day 5 of the 30-day Python course! Today, we will cover lists in Python.

## Lists:
A list is a collection of items that are ordered and changeable. Lists are one of the most commonly used data structures in Python, and are used to store collections of related items.

## Creating a List:
To create a list in Python, you simply enclose the items in square brackets, separated by commas. For example, here is a list of integers:

```
numbers = [1, 2, 3, 4, 5]
````
You can also create a list of strings:

```
fruits = ["apple", "banana", "orange"]
```

## Accessing List Items:
You can access individual items in a list using their index. The index of a list starts at 0, so the first item in the list has an index of 0, the second item has an index of 1, and so on. For example, to access the first item in the fruits list above, you would use the following code:

```
first_fruit = fruits[0]
print(first_fruit)
```
This will print "apple".

You can also access items from the end of the list using negative indexing. The last item in the list has an index of -1, the second to last item has an index of -2, and so on. For example, to access the last item in the fruits list above, you would use the following code:

```
last_fruit = fruits[-1]
print(last_fruit)
```

This will print "orange".

## Changing List Items:
Lists are mutable, which means that you can change the values of individual items in a list. For example, to change the second item in the fruits list to "pear", you would use the following code:

```
fruits[1] = "pear"
```
Now the fruits list would look like this:

```
fruits = ["apple", "pear", "orange"]
```

Adding and Removing List Items:
You can add items to the end of a list using the append() method. For example, to add "kiwi" to the fruits list, you would use the following code:

```
fruits.append("kiwi")
```
Now the fruits list would look like this:

```
fruits = ["apple", "pear", "orange", "kiwi"]
```

You can also insert items into a specific position in the list using the insert() method. For example, to insert "grape" at the second position in the fruits list, you would use the following code:

```
fruits.insert(1, "grape")
```

Now the fruits list would look like this:

```
fruits = ["apple", "grape", "pear", "orange", "kiwi"]
```
To remove an item from a list, you can use the remove() method. For example, to remove "pear" from the fruits list, you would use the following code:

```
fruits.remove("pear")
```

Now the fruits list would look like this:

```
fruits = ["apple", "grape", "orange", "kiwi"]
```

Lists are a powerful tool for organizing and working with data in Python. With their ability to store collections of related items, 
as well as their built-in methods for adding, removing, and modifying items, lists are an essential data structure for any Python programmer. 
Stay tuned for Day 6, where we will cover strings in Python.

<br>
<hr>
# Mini Project 1: 
Mini Project: Simple To-Do List

For this mini project, we will create a simple to-do list application that allows the user to add, remove, and view items on a to-do list.

Day 1: Introduction to Python
We will use Python to create the application, and we will start by learning the basic syntax and structure of the language.

Day 2: Variables and Operators
We will use variables to store the to-do list items, and operators to manipulate the list.

Day 3: Conditional Statements
We will use conditional statements to check if the user wants to add, remove, or view items on the list.

Day 4: Loops
We will use loops to iterate through the list and display the items to the user.

Day 5: Lists
We will use Python lists to store the to-do list items.

### Solution:

Here is the code for our simple to-do list application:

```
# initialize an empty list to store the to-do list items
todo_list = []

# define a function to add items to the list
def add_item():
    item = input("Enter item to add to the list: ")
    todo_list.append(item)

# define a function to remove items from the list
def remove_item():
    item = input("Enter item to remove from the list: ")
    if item in todo_list:
        todo_list.remove(item)
    else:
        print("Item not found in the list.")

# define a function to view the items on the list
def view_list():
    print("To-Do List:")
    for item in todo_list:
        print(item)

# main loop to prompt the user for input
while True:
    print("Enter 'add' to add an item to the list.")
    print("Enter 'remove' to remove an item from the list.")
    print("Enter 'view' to view the items on the list.")
    print("Enter 'exit' to quit the application.")
    
    choice = input("Enter your choice: ")
    
    if choice == "add":
        add_item()
    elif choice == "remove":
        remove_item()
    elif choice == "view":
        view_list()
    elif choice == "exit":
        break
    else:
        print("Invalid choice. Please try again.")
'''
When the user runs the application, they will be prompted to enter one of four choices: "add", "remove", "view", or "exit". If they choose "add", they will be prompted to enter an item to add to the list. If they choose "remove", they will be prompted to enter an item to remove from the list. If they choose "view", the items on the list will be displayed. If they choose "exit", the application will exit.

This simple to-do list application demonstrates the power of Python's built-in data structures and control structures, and provides a great starting point for anyone looking to learn more about the language.
<br>
<hr>
# Mini Project 2: Guess the Number Game

For this mini project, we will create a simple "Guess the Number" game, which will incorporate the topics we have covered from Day 1 to Day 5.

## Game Description:
The game will generate a random number between 1 and 20, and the user will have 3 attempts to guess the number. For each guess, the game will provide feedback on whether the guess was too high or too low. If the user guesses the number correctly within the given number of attempts, the game will congratulate the user and end. If the user does not guess the number correctly within the given number of attempts, the game will end and reveal the correct number.

#### Hint use the follwing code as a start point 
* Note import  random package and use randinit(1, 20) funcion to randomly generate number from 1 to 20
```
import random

print("Welcome to the Guess the Number Game!")
print("I am thinking of a number between 1 and 20.")

number = random.randint(1, 20)
guesses_left = 3

while guesses_left > 0:
   # TODO finish the rest of the code 
```
Solution:

Here is the solution to the Guess the Number Game, incorporating the concepts from Day 1 to Day 5.

```
import random

print("Welcome to the Guess the Number Game!")
print("I am thinking of a number between 1 and 20.")

number = random.randint(1, 20)
guesses_left = 3

while guesses_left > 0:
    print("You have " + str(guesses_left) + " guesses left.")
    guess = input("Guess the number: ")
    try:
        guess = int(guess)
    except:
        print("Invalid input. Please enter a number between 1 and 20.")
        continue
    if guess < 1 or guess > 20:
        print("Invalid input. Please enter a number between 1 and 20.")
        continue
    if guess == number:
        print("Congratulations! You guessed the number!")
        break
    elif guess < number:
        print("Your guess is too low. Try again.")
    else:
        print("Your guess is too high. Try again.")
    guesses_left -= 1

if guesses_left ...
   #TODO complete the rest of the code
 

```
