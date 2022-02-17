# Introduction to Python

## Reading

As a reminder, keeping up with reading in the Practical Computing book (and reviewing outside resources) provides valuable added perspective about the topics we are covering. For this topic, please review chapters 7 and 8. Additional resources are linked below.

## What is Python?

- Interpreted, high-level language (means it does memory management, takes care of details, opposite of interpreted language is complied, easy to learn and write)
- Very popular among computational biologists (libraries exist for us to use already)
- One of the most "human readable" programming languages 
- One of the few languages where line indentation is actually interpreted as part of the code (spacing tells when codes should be executed)
- Python is _much_ less picky than bash about spacing within lines, though
- Dynamically typed (don't worry, we'll get to this later) 

## Three Ways to Run Python
>>> means we cannot do bash commands
>>> quit() to exit


### Python Interpreter

- Unlike many programming languages (e.g., C++ and Java), Python can be executed interactively.
- To start the Python interpreter, simply open up a Terminal window and type `python`.
- Once the Python prompt (`>>>`) appears, type:
    - `a = 3`
    - `print(a)`
- What do you see?
- To exit the Python interpreter, type `quit()`.

### Command-line Python

- Now, put those same commands in a text file ending with a `.py` extension (e.g., `test.py`).
- At the bash command prompt, type `python test.py`.
- What do you see?
- The `.py` extension isn't required, but is conventional for Python code.

### Jupyter Notebooks

- Jupyter notebooks are a special type of file that allows formatted notes to be mixed with Python code.
- These notebooks can be run on smic through OnDemand.
- To open a Jupyter notebook, go to the "Interactive Apps" menu at the top and select "Jupyter Notebook".

## Basic Python Data Types

- Numbers
    - Note that, unlike bash, Python can handle _both_ integers and floating point (decimal) numbers.
    - Integers - `myInt = 10`
    - Floating point numbers (decimals) - `myFloat = 3.21312`
    - If running Python interactively, variable values can be seen just by typing the name of the variable - `myFloat`.
    - If running Python in a script, variable values can be printed by using the `print()` funtion - `print(myFloat)`.
    - Define myInt and myFloat as above. Now calculate `myInt / myFloat`. What type of number is the result?
    - Now try `float(myInt)` and `int(myFloat)`. What are the results? Look back at the values of `myInt` and `myFloat`. Have they changed?
    - Changing numbers from one type to another is one form of "type casting".

- Strings - `myStr = "This is a string."`
    - Strings can be of any length, but are always defined with quotes.
    - Individual characters, or subsets of characters, can be accessed using square brackets - []
      - String indices (and all indices in Python) start at 0
      - `myStr = "biology"`
      - `myStr[0]`
      - A range of indices can be defined with a colon
      - `myStr[2:5]`
    - Strings can be concatenated together with the `+` operator.
      - `myStr = "biology"`
      - `newString = myStr + "_is_super_interesting"`
      - `newString`

- Booleans - `True` or `False`
    - These variables can take the values `True` or `False` only.
      - `myBool = True`
    - These are the data types used in things like `if...else` statements and `while` loops.
    - Logical statements, like `myNum > 3` or `myStr == "test"`, return a boolean variable indicating the result of the comparison
    - In Python, the value of a Boolean can be reversed by preceding it with `not`.
