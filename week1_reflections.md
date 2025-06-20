# Week One Reflections
What I have learned in the first week of this course.
## What is a Computer?
Before we learned anything about programming, we had to first learn what a computer really is. A computer is a programmable device that can be made to perform mathematical and logical operations (Dictionary.com). A computer is made of many hardware components including but not limited to: A mainboard, monitor, CPU, and RAM, with the latter half being the most important components.
## What is Programming?
The second thing we learned is what programming really is. It is a set of instructions given to a computer to execute. At a base level, programming is configuring the tiny switches on the computer to turn either on or off, represented by ones and zeros. These switches on the computer are considered "Executable Machine code," while Python is considered a "High-level program." This simply means Python is easier for us to read. A level higher than Python could be Artificial Intelligence, which can create code from simple human sentences.
## Computer Science
Computer Science is the science of giving a computer a set of steps to compute. There are levels to each type of component that makes up one of these steps. The smallest component is a token. A token includes variable names, numbers, and operators. The next level is an expression, which puts tokens together to produce a value. An example of this is x + 5. Next from the expression is a statement. This is something Python can execute. For example, our first program, `print("Hello World!")`, is a statement. While there are more levels to the components that make up Python, we are able to write code using just the three levels learned. 
### Algorithms
These steps put all together are called an algorithm. An algorithm must be precise as a computer has no brain. If an algorithm is not precise, there may be an unwanted outcome. A very memorable example of this was programming the Fibonnaci sequence. The proper sequence of steps is shown below:
```python
num1 = 0
num2 = 1
fibNum = num1 + num2
print(fibNum)

num1 = num2
num2 = fibNum
fibNum = num1 + num2
print(fibNum)
```
As seen in the second set of steps, we change the variable `num1` to `num2` before we change `num2` to the current `fibNum`. This line of code can be repeated to print the output: 1, 2, 3, 5, 8, 13...
However, when we only move a couple lines on the second section of code,
```python
num2 = fibNum
num1 = num2
fibNum = num1 + num2
print(fibNum)
```
The steps shown here are in the wrong order. when using this block of code to attempt to generate the Fibonacci sequence, instead the following sequence is returned: 1, 2, 4, 8, 16...
### Variables
As seen in the Fibonacci sequence example, there are some tokens that are not normalized. These tokens are called variables. A variable can be assigned a value and stored on a computer for future use. There is a convention for naming these variables. Some of the rules include keeping the first letter lowercase, capitalizing the first letter of any following words, no spaces, and being descriptive. A variable `x` should be avoided as it does not describe what it is storing. This can be confusing to your future self. A better variable can be `triangleHeight`.
### Data Types
There are many data types, however we have only used three in the first week of the course. The first of these data types are an integer. These are numbers that have no decimal, for example, 5. A similar data type is a floating point. These are also numbers, however they contain a decimal value (0 included). An example of a float is 6.7. Finally, words would be called a string. A string contains characters and must be in quotation marks. An example of a string is "15 apples."
| Data Type     | Shortened  | Example     |
|---------------|:----------:|:------------|
| Integer       | int        | 5, 10, 42   |
| Floating Point| float      | 5.0, 6.7    |
| String        | str        | "Hello World!" |
### Inputs
Inputs are a way to be able to edit tokens while running the code. A simple program utilizing an input looks like this:
```python
name = input("What is your name? ")
lastName = input("And your last name? ")
print("Welcome, " + name + " " + lastName)
```
By running this code, the user will be prompted with the following:

![image](https://github.com/user-attachments/assets/bfa28eff-9788-4b58-b060-6230d657f92e)

Upon entering their first name, the use will then be prompted with entering their last name, resulting in the final output:

![image](https://github.com/user-attachments/assets/bc4e2394-c42b-4b9d-8f9a-3d5e5b0c986d)

A useful application of inputs is doing calculations or conversions for a user. For practice, we wrote a program to convert kilometers to miles.
```python
kilometer = float(input("How many kilometers? (ex: 10) "))
conversionFactor = 1.60934
mile = kilometer/conversionFactor
print(str(kilometer) + " kilometers is equal to " + str(mile) + " miles")
```
By inputting a kilometer distance, for example 10, the program outputs an equivalent distance in miles.

![image](https://github.com/user-attachments/assets/105cd3dd-1fe3-43ab-bdd3-91e2be7ad136)
### Files 
There are many different file types, however we focused on text files, specifically `.txt`. There are three commands related to files. Read, write, and append. Reading a file is simply opening the file without the ability to edit, think of it like viewing a google doc in view only mode. Writing a file will overwrite whatever is already on there with the information given to write. Finally, appending a file will add on information to the end. For practice with files, we took inputs from a user and sent them to a `.txt` file to store information. 
```python
name = input("What is your name? ")
age = input("How old are you? ")

idFile = open("userID.txt", "w")
idFile.write(name + ", " + age)
idFile.close()
```
The age and name of the user were sent to a `.txt` file.

![image](https://github.com/user-attachments/assets/0bb564bb-80f7-4eb8-9562-d5c29c071541)

### Debugging
Debugging is the most important aspect of coding. It is guaranteed something will go wrong, and it is essential to be able to understand what happened to be able to fix it. There are three types of errors as shown:
| Error Type     | Cause  | Show Message?     |
|---------------|:----------:|:------------|
| Syntax Error | invalid syntax, for example trying to add a string and integer | yes |
| Runtime Error| error happens while code is running, for example printing a variable that doesn't exist      | yes |
| Semantic Error| code doesn't run as expected, for example Fibonacci sequence        | no |

While a syntax and runtime error will display a message and a line where the error went wrong, a semantic error will not. A semantic error is nicknamed a 40 cm error as the error is 40 centimeters in front of the screen. It is also the hardest to find as there is no message displaying which line the error happened. The programmer has to look through all their code to attempt to identify the error.

## Conclusion
I am very excited to continue the class and learn more about how to program with Python. I feel like I grasped the knowledge of the very basics of programming with Python very well and I am ready to learn more things about coding.
