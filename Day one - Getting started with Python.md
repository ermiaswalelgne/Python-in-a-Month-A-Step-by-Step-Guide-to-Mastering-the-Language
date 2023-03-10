###### ⬅[Home||](https://github.com/ermiaswalelgne/Python-in-a-Month-A-Step-by-Step-Guide-to-Mastering-the-Language)

# Welcome to Day 1 of the 30-day Python course! 
Today, we will cover the basics of Python programming, including installation and setup, and writing your first Python program.

## Installation and Setup:
To begin, you will need to install Python on your computer. Python can be downloaded for free from the official Python website (https://www.python.org/downloads/). Once you have installed Python, you can start writing and running Python programs using a text editor or an integrated development environment (IDE). Some popular choices for Python IDEs include PyCharm, Visual Studio Code, and Spyder.
### Installing Python on Mac:
##### Without a Virtual Environment:
<ol> 
<li>Open a web browser and navigate to the official Python website: https://www.python.org/downloads/mac-osx/ </li>
<li>Download the latest version of Python for Mac by clicking on the "Download Python X.X.X" button.</li>
<li>Run the installer and follow the prompts to complete the installation.</li>
<li>To verify the installation, open the Terminal application and type python3 --version and press Enter. This should output the version of Python that you just installed.</li>
 </ol>
 
##### With a Virtual Environment:
<ol> 
<li>Open the Terminal application and type python3 --version and press Enter. If Python is not installed, follow the steps above to install it.</li>
<li>Type pip3 install virtualenv and press Enter. This will install virtualenv, which is a tool to create virtual environments.</li>
<li>Type mkdir myproject and press Enter. This will create a directory for your project.</li>
<li>Type cd myproject and press Enter. This will change your working directory to the project directory.</li>
<li>Type virtualenv venv and press Enter. This will create a virtual environment in the "venv" directory.</li>
<li>Type source venv/bin/activate and press Enter. This will activate the virtual environment.</li>
<li>Type pip install package-name to install packages inside the virtual environment.</li>
</ol>

### Installing Python on Windows:
##### Without a Virtual Environment:
<ol> 
<li>Open a web browser and navigate to the official Python website: https://www.python.org/downloads/windows/</li>
<li>Download the latest version of Python for Windows by clicking on the "Download Python X.X.X" button.</li>
<li>Run the installer and follow the prompts to complete the installation.</li>
<li>To verify the installation, open the Command Prompt and type python --version and press Enter. This should output the version of Python that you just installed.</li>
</ol>

##### With a Virtual Environment:
<ol>
<li>Open the Command Prompt and type python --version and press Enter. If Python is not installed, follow the steps above to install it.</li>
<li>Type pip install virtualenv and press Enter. This will install virtualenv, which is a tool to create virtual environments.</li>
<li>Type mkdir myproject and press Enter. This will create a directory for your project.</li>
<li>Type cd myproject and press Enter. This will change your working directory to the project directory.</li>
<li>Type virtualenv venv and press Enter. This will create a virtual environment in the "venv" directory.</li>
<li>Type venv\Scripts\activate and press Enter. This will activate the virtual environment.</li>
<li>Type pip install package-name to install packages inside the virtual environment.</li>
</ol>

### Using Visual Studio Code:
Once Python is installed, you can use Visual Studio Code as your code editor. Here are the steps to set it up:

<ol>
<li>Download and install Visual Studio Code from the official website: https://code.visualstudio.com/</li>
<li>Open Visual Studio Code.</li>
<li>Open the Command Palette by pressing Ctrl+Shift+P (Windows) or Cmd+Shift+P (Mac).</li>
<li>Type "Python: Select Interpreter" and press Enter.</li>
<li>Choose the interpreter for your project (either the global Python installation or the virtual environment you created).</li>
<li>To create a new Python file, click on "File" > "New File" and save it with a .py extension.</li>
<li>Start coding in Python!</li>
</ol>
That's it! You now have Python installed on your computer and Visual Studio Code



<hr>

## Hello World Program:
The "Hello World" program is a classic first program for learning any programming language. It simply prints the text "Hello, World!" to the screen. Let's write our own "Hello World" program in Python!

Open your text editor or IDE and create a new file. Type the following code:

```
print("Hello, World!")
```

Save the file as "hello_world.py". The ".py" extension indicates that this is a Python program.

To run the program, open a terminal or command prompt and navigate to the directory where you saved the file. Type the following command:

```
python hello_world.py
```
This will run your Python program and print the message "Hello, World!" to the screen.

## Basic Data Types:
Python supports several basic data types, including strings, numbers, and booleans.

A string is a sequence of characters enclosed in quotes. For example, "Hello, World!" is a string.

Numbers can be integers (whole numbers) or floats (decimal numbers). For example, 42 is an integer, and 3.14 is a float.

Booleans are true/false values. They are represented by the keywords "True" and "False" (without quotes).

In Python, you can use the "type" function to determine the data type of a value. For example:

```python
print(type("Hello, World!")) # output: <class 'str'>
print(type(42)) # output: <class 'int'>
print(type(3.14)) # output: <class 'float'>
print(type(True)) # output: <class 'bool'>
```
Congratulations, you have now written your first Python program and learned about some of the basic data types in Python. Stay tuned for Day 2, where we will cover variables and operators in more detail.

###### ⬅[Home||](https://github.com/ermiaswalelgne/Python-in-a-Month-A-Step-by-Step-Guide-to-Mastering-the-Language)
