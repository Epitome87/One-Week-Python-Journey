# One Week Python

A Udemy course by Colt Steele

## Section 1: Welcome & Introduction

##### `Originally Started & Completed: 05/11/2023`

### Welcome to the Course

This Course Is...

- Fast, effective pathway to learn Python
- Full of exercises, challenges, quizzes
- Made for normal people who can't stand 20 minute videos. Average video is 4 minutes!
- An ideal on-ramp to data science, Machine Learning, or web development courses

### What This Course Is Not

- A 60 hour Python encyclopedia course that covers every possible feature of Python
- An advanced level Python course for experts
- A web development, data science, or machine learning oriented course

### Why You Should Learn Python

High Demand

- There are more Python jobs today than ever before
- Salaries for them are at an all-time high
- If you could pick only one language to learn, many argue it should be Python!

Huge Community

- Python has been around for 30+ years now, and in that time a massive, supportive online community has formed
- You can always get help and find answers (relatively) easily

Libraries

- There are thousands of Python libraries, frameworks and tools available
- From Django to Matplotlib to Scikitlearn, there's usually something for every need

Easy to Learn

- Python is one of the easiest programming languages to learn
- It has far fewer quirks and oddities than languages like JavaScript

Versatility

- You can use Python for simple scripting tasks
- You can use it to build huge web applications
- You can use it for data processing and analysis
- And you can, of course, use it for machine learning -- where it is _the_ language of choice!

### What We Can Do With Python

Game Dev

- Hugely popular games including The Sims 4, Civilization, EVE Online, and many others are built using Python

Web Dev

- Companies ranging from tiny startups to massive unicorns use Python to build web applications
- Reddit, Instagram, Youtube (using Python with other languages, but backend is largely written in Python)

Data Stuff

- Python is hugely popular in the world of data science and data analysis
- Python tools like numpy, pandas, and matplotlib are widely used

Machine Learning

- Python is _the_ language for machine learning
- Tools include TensorFlor, Scikitlearn, OpenCV, and Natural Language Toolkit

Science

- Python is used across academia and the science world
- From biology research labs to NASA engineering teams

Computer Apps

- Dropbox, Anki, Cinema 4D, BitTorrent

## Section 2: Installation & Setup

##### `Originally Started & Completed: 05/11/2023`

### Python Versions: They Actually Matter!

Python 3 was a _major change_ when released:

- It was not backwards compatible with Python 2
- It included some syntax changes
- Featured major changes under the hood
- It took 10+ years for Python 2 to be officially declared dead

At this point, there is no real reason to learn Python 2, but it's worth knowing the history because:

- Lots of tutorials online are for Python 2
- Your computer may have 2.x pre-installed
- Some dead libraries / tools still have not been updated to work with Python 3.x

### 2 Ways of Running Python

There are two different options when we want to run some Python code:

**Interactive Python**

In interactive mode, any code you enter is immediately run.
Python executes each line as you enter it and then displays the output.
Great for learning and trying things out, but not great for real applications.
We start interactive python by typing `python` in a command prompt, or opening Python 3 from our Windows start menu

**Python Scripts**

Alternatively, you can (and should, typically) write Python code in a file.
And then you can separately execute that script with Python.
The code only runs when you manually tell it to.

We can run a Python script by putting the code in a .py file, and running the following command:

```
python script_name.py
```

### Installation for Windows Users

We can download the latest version of Python from the official site. Simply run the executable and follow the rather straightforward instructions.

### The No-Installation Option: REPL.it

Another way to write Python is by using `repl.it`, an online REPL (Read, Evaluate, Print, Loop). It is an online application that allows us to create coding environments (not just Python) completely in the browser.

## Section 3: Python Numbers

##### `Originally Started & Completed: 05/11/2023`

### Intro to Data Types

Some data types found within Python include:

- Strings
- Integers
- Booleans
- Floats
- Bytes
- Dictionary
- List
- Tuple
- Set
- Complex
- Range
- Frozenset

We will start by exploring four of the more fundamental data types:

- Strings
- Integers
- Booleans
- Floats

### Integers and Floats

Two important numeric data types are `Integers` and `Floats`.

**Integers**

- Whole numbers only
- Positive or negative
- No decimal points!
- Examples: 9, 378, -21

**Floats**

- Floating-point numbers
- Written with a decimal point
- Positive or negative
- Examples: 1.5, 9.99, -2.0, 1.2349e12

In Python 3, integers are **unbounded**; they can be as large as we want. Floats, however, are _not unbounded_; they have a limited precision.

We can use `type()` to return the _type_ of something. So we can see that Python does, indeed, distinguish between Integer and Float. They are stored in memory differently, with floats taking up more memory, and mathematical operations are more complicated when used on floats.

### Numeric Notations

When writing an Integer or Float value, we can use underscores to separate every 3 numbers (like how we would with a comma in English). Using commas is _not valid_ for numeric types, and is actually treated as something entirely different in Python. An integer cannot start with leading zeros.

```py
1000 # Valid
1_000 # Valid
1,000 # Not valid!
01 # Not Valid!
01.00 # Valid
1_000_000.55 # Valid
```

We can also scientific notation with a Float:

```py
1286e+19
1286e19
6.7e-3
```

### Basic Operators

`Operators` are special characters in Python that perform **operations** on values (**operands**). Below are some of the most common:

- +, -, \*, /, %, \*\*
- \> , <, >=, <=, ==, !=
- and, or, not, is, in
- !=, =, +=, -=, \*=, /=, |=

Mathematical Operators:

```py
1 + 4 # Addition operator
4 - 1 # Subtraction operator
5 * 2.5 # Multiplication operator
4 / 2 # Division operator
```

**Note:** We can perform operations when the operand is a combination of a Float and an Integer. The result will always be a Float.

**Order of Operations**

- Parenthesis: ()
- Multiplication and Division: \*, /, //
- Addition and Subtraction: +, -

We can manipulate the typical PEMDAS order of operations by surrounding code we want to evaluate first in parenthesis.

```py
6 * 3 - 10      # Result: 8
6 * (3 - 10)    # Result: -42
```

### Lesser Known Operators

Some other numeric operators that are a little lesser known:

**Integer Division**: `//`

- This is how we do division where the result is _rounded down_ to nearest integer
- This can be confusing for negative numbers, where rounding down means to a number _further away from 0_, rather than closer to 0 when working with positive numbers.

```py
10 / 3  # Result: 3.3333333
10 // 3 # Result: 3

4 / 5   # Result: 0.8
4 // 5  # Result: 0

10 // -3 # Result: -4
```

**Exponentiation**: `**`

- This is how we raise one power to another power

```py
4 ** 3 # Result: 4 * 4 * 4 => 64
```

**Modulo**: `%`

- Also known as the remainder operator
- The right side operand is divided into the left side operand as many times as possible. The remainder is the result of the modulo operator

```py
38 % 10     # Result: 8 -- 10 divides 38 three full times, leaving 8 as the remainder
10 % 7      # Result 3
25 % 9      # Result: 7
```

Commonly used to determine if a number is even or odd: If we can divide cleanly by 2 (no remainder), the number must be even.

### Python Comments

Python will ignore any lines starting with the `#` symbol. This is a `comment`: this text will never be executed, and is intended to allow authors to leave useful notes in a program.

```py
# This line never runs
1 + 1 # To the left of this line will run!
```

## Section 4: Variables Basics

##### `Originally Started & Completed: 07/29/2023`

### Introducing Variables

`Variables` are what we use to store values and give them a label. This is useful so that we can:

- Refer back to it later
- Use that value to do stuff
- Change it later on

To **declare** a variable, we write:

```py
age = 36
```

Here, _age_ is the name of the variable, and _36_ is its value. The _=_ symbol is the `assignment operator`, and is used to assign a value (on its right) to a variable (on its left).

We can now refer back to _age_ to check its value, or update its value. For example, we could add to the _age_:

```py
age = age + 1 # Birthday happened!
```

### Variable Naming

When naming variables, there are a few rules to follow:

- Variable names can **contain** numbers, _but_ they cannot **start** with a number
- Variable names cannot contain spaces
  - Use `snake case` instead by using the **underscore** character
- Variable names cannot be a Python **keyword / reserved word**, like class, finally, continue.

```py
variable123 # Valid
first_name  # Valid
player_1    # Valid
123variable # Invalid!
first name  # Invalid!
False       # Invalid!
def         # Invalid!
```

Use names that make it clear what the variable is storing. Rather than `i`, use `score`, for example.

Typically, we write `constants` (values that will not change) in all uppercase letters.

### Assignment Operators

Besides the equal sign, other assignment operators allow us to change the value that is currently in an existing variable **using that variable's current value**.

The following are some of the assignment operators:

- +=, -=, \*=, /=, //=, \*\*=, %=

```py
score = 2
score = score + 1

score += 1 # Equivalent to score = score + 1
score -= 1 # Equivalent to score = score - 1
```

### Numbers & Variables In the Wild

In this lecture we examined the use of numbers and variables in the wild! For example, the Frets on Fire game (written in Python) uses many variables to help keep track of the player's score.

### The Print() Function

The `print()` function prints out any values we pass to it to "standard output". It does not return anything.

```py
print("Hello, World!")
```

While this function is not related to variables, we will need to use it in the upcoming challenge.

### Magic Trick Exercise

This little exercise will require you to use assignment operators like `+=`, `-=`, and `*=` Download the starter code and follow the instructions in the file. You’ll pick a secret number, save it in a variable, and update that variable according to the steps detailed in the file. At the bottom of the file you’ll find my magical prediction (it’s really not impressive or magical at all).

```py
# Create a variable called secret_num and set it to any number you'd like:
secret_num = 7

# Increase secret_num by 1:
secret_num += 1

# Next, take the new number and double it:
secret_num *= 2

# Next, take the new number and add four to it:
secret_num += 4

# Next, take the new number and divide it by two:
secret_num /= 2

# Next, take the new number and subtract your original secret from it:
secret_num -= 7

# Print the final result:
print(secret_num)
```

## Section 5: String Basics

##### `Originally Started: 12/08/2023`

### Introducing Strings

A `String` is another basic data type in Python. Strings are a textual datatype and must be wrapped in quotes (either single or double). They are "strings of characters."

An example of a string:

```py
'hello word'
'hi"  # Invalid - opening and closing quotes must match in type!
type('69') # str
type(69) # int
```

Note that if we want our strings to have `'` or `"` in them, we have to choose our opening and closing quotes appropriately (by using the opposite).

```py
"She said 'hello'" # Valid
"She said "hello"" # Invalid
'You're not the boss!' # Invalid
```

### String Variables

Remember, in Python the _type_ of a variable can be changed at any time. Also, like with numbers, we can store strings in variables:

```py
color = "Magenta" # Note the single quotes
twitter_handle = '@Epitome87' # Note the double quotes
```

### String Operators

**Addition (Concatenation)**

When we work with strings, the `+` operator still works, but it does not add strings (like with numbers). Rather, it `concatenates` (joins) strings together.

```py
first_name = "Matthew"
last_name = "McGrath"
"hello " + first_name + " " + last_name # "hello Matthew McGrath"

"4" + "5" # "45"
```

**Multiplication (Repeat)**

We can also multiply a string by a number, which will repeat that string.

```py
'ha' * 4 # 'hahahaha'
4 * 'ha' # 'hahahaha'
'ha' * 'ha' # Invalid - must have one operand be a number
```

### String Indexing

Every single string is ordered. Every single string is indexed, starting at 0.

```py
msg = 'I <3 Cats'
msg[0] # 'I'
msg[5] # 'C'

'Hello'[1] # 'e'
'Hello'[69]' # Error: string index out of range
```

We can also use negative indices, which will be counted backward starting from the end of the string:

```py
'Matthew'[-1] # 'w'
```

### The Special Value - None

`None` is a special value in Python that denotes the **lack of value**. It is not the same as zero or an empty string (those are still values). Think of it as Python's version of `null` in other programming languages.

```py
active_user = None # We don't know this information yet, so set to None

# Later on...
active_user = 'Matthew'
```

It even has its own type:

```py
type(None) # NoneType
```

## Section 6: A Little More On Strings

##### `Originally Started: 12/09/2023`

### String Slices

We've seen how to access a single character of a string using indices. We can access a portion of a string -- a `slice` if you will. We use the notation `string[startIndex:stopIndex]`:

```py
msg = 'I <3 Cats'
msg[2:6] # '<3 C'

animal = 'catdog'
animal[3:6]
```

Note that the stopIndex is _exclusive_ -- it is up to, but not including, that index.

We can omit the start or stop index if we wish to start from the beginning or slice until the end, respectively:

```py
animal[:3] # 'cat'
animal[3:] # 'dog'
```

We can provide a 3rd argument, the `step`, which will only slice every step of the string:

```py
'123456'[0:6] # '135' - Include every 2nd character
```

### Revisiting Print()

The `print()` function prints out any values we pass to it to "standard output." It does not return anything.

```py
print('Hello')
```

### Escape Characters

`Escape character1` are special sequences inside of Python strings that start with a backslash. Their regular characters will be _escaped_. Some common escape characters are:

- Newline: `\n`
- Tab: `\t`
- Double Quote: `\"`
- Single Quote: `\'`
- Backslash: `\\`

```py
greeting = 'hello \tworld' # 'hello   world'
greeting = "He said \"Hello\"" # "He said "Hello""
```

### Triple Quoted Strings

We can use three single or double quotes to allow us to write strings that span across multiple lines. It's for readability sake, as Python still will produce the underlying newline characters in the output.

```py
'''
Hello, World!
Today is a great day!
We can have single quotes as well as double quotes,
like in he said "Let's go!"
'''

# Output:
'\nHello, World!\n Today is a great day!'\nWe can have single quotes as well as double quotes,\nlike in he said "Let\'s go!"

address = """
Chicken Little
123 Chicken Wing Lane
Denver Colorado 21736
"""

print(address) # Result of the above print is human readable address
```

### Strings in the Wild

Strings are used everywhere in Python programming! If we are working with text and output, it is safe to assume strings are used in some form.

### Nico Hülkenberg Exercise

It's time to practice what you've learned about strings!

```py
first = "Nico"
last = "Hülkenberg"

# - Create a variable called "full_name" that combines first and last with a space between them.
full_name = first + ' ' + last;

# - Print it out
print(full_name)

# - Create an "initials" variable that holds the first character of first name followed by the first character of last.
initials = first[0] + last[0]

# - Print it out
print(initials)

# - Create an "initials_2" variable that holds the first character of first followed by the first character of last, with periods after each letter.
initials_2 = first[0] + '.' + last[0] + '.'

# - Print it out
print(initials_2)

# - Create a nickname variable that holds the first 4 characters of "last"
nickname = last[:4]

# - Print it out
print(nickname)
```

## Section 7: Strings & Built-Ins

##### `Originally Started: 12/11/2023`

### Introducing Functions

A `function` is a reusable piece of code that has a name. To execute a function, we use parenthesis after its name. Python comes with many built-in functions, such as `help`, `type`, `print`, etc.

```py
help("string")
type("int")
print("Hello, World!")
```

`Arguments` are the _inputs_ to a function.

### The Len Function

The `len()` function will return the length of whatever item we pass to it. So far Strings are the only sequence we have seen, but soon there will be others!

```py
word = "Chicken"
len(word) # 7
```

Note that we can pass the name of other built-in functions to the `help` function:

```py
help(len) # Help is output: "Return the number of items in a container"
```

### The Input Function

The `input()` function will prompt a user to enter some input, convert it into a string, and then return it. We can use it to gather user input in our programs. The argument we pass into it will be the text that is output while waiting for the user's input.

```py
age = input("How old are you?") # Age will store whatever the user inputs
```

The result of input is _always_ a string -- even if the user enters a number.

### Type Casting

In order to cast a variable of one type to another, we use **casting types**.

```py
int(age)      # 19
float("6.9")  # 6.9
str(44.5)     # "44.5"
int(6.9)      # 6 - truncated the float

age = "19"
days_old = age * 365 #'19191919...' etc. Doesn't work how we want!
days_old = int(age) * 365 # Correct!
```

### Age Calculator Exercise

Create a program that asks a user how many years old the user is. Output the number of days the user is old.

```py
years_old = input("How many years old are you?")
days_old = float(years_old) * 365
print("You are " + days_old + " days old!")
```

### F-Strings

`F-Strings` (formatted string) are an easy way to generate strings that contain interpolated expressions. Any code between two curly braces will be evaluated and then the result will be turned into a string and inserted into the overall string. This feature is new to Python 3!

```py
f"There are {24 * 60 * 60} seconds in a day"
# There are 86400 seconds in a day"
```

```py
age = input("How old are you?)
days = float(age) * 365
print("You are " + days + " days old") # Invalid! Cannot concatenate a number with a string
print("You are " + str(days) + " days old") # Could solve it this way, or...
print(f"You are {days} old") # Using F-Strings - much cleaner!
```

### F-Strings & Type Casting in the Wild

F-Strings and type castings can be found everywhere. From video games, e-commerce apps, and data science.

### Shopping Cart Exercise

Write a Python script that does the following:

- Prints out a "banner" to welcome users to our shop
- Asks the user for the name of the item they are buying
- Asks the user for the price of that item
- Asks the user for the quantity they are purchasing
- Prints out a message that includes their subtotal (quantity x price)

Here's an example of that script running:

```
Welcome to our useless store!
*****************************
What item are you purchasing? (taco)
What is the price of taco? (59.99)
How many (pillow) are you buying? (4)

Added 4 pillow(s) to shopping cart
Subtotal: $239.96
```

Solution:

```py
print("Welcome to Matthew's Store!")
print("*" * 30)

item = input("What item are you purchasing: ")
price = float(input(f"What is the price of {item}: "))
qty = int(input(f"How many {item} are you buying: "))

print(f"Added {qt} pillow(s) to shopping cart")
print(f"Subtotal: ${price * qt}")
```
