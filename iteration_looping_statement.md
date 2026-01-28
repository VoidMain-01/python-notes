# Iteration / Looping Statements
---
Iteration statements are commonly known as loops. Iteration statements executes a set of statements / a block of code repeatedly until a specified condition returns false.
There are mainly two types of loop in Python
- while loop
- for loop

Syntax of while loop:

<initialization>
while <test-expression>:
    statement
    [statement]
    <update-expression>

Example: 
WAP to print first 15 natural numbers
```Python
while x <= 15:
    print(x, end = ", ")
    # x = x + 1
    # x++ [Invalid Syntax]
    x += 1
else:
    print("Loop ended successfully")
    print("Ok Thank you")
```
Both the for and while loop have an else clause, which is different from the if and if-else statements. The else of the loop executes only when the loop ends normally. (i.e only when the loop's test-expression evaluates to false)

Pyhton's pass statement - Python's pass statement does nothing when executed. pass statement is generally required when the code block is to be added later on.

You can use pass statement inside a function where you want to leave it empty to avoid errors.

```Python
age = int(input("Enter your age: "))
if age < 18:
    pass
elif age > 18:
    print("Elligible")