# match-case statement
---
The match case statement in Python was introduced in 3.10 version. This feature allow you to perform pattern matching and make decision based on values of variable.

It supports complex pattern matching (e.g. sequences)

The syntax:
```Python
match <variable or expression>:
	case pattern1:
		#code block in pattern1
	case pattern2:
		#code block in pattern2
	.
	.
	case patternN:
		#code block in patternN
	case _ :
		#default code block
```
###### Example
---
```Python
day = int input("Enter a day: ")
switch day:
	case 1:
		print("Monday")
	case 2:
		print("Tuesday")
	case 3: 
		print("Wednesday")
	case _:
		print("Other day")
```

The value _ is to be placed at the last case to make it behave as a default case.

## Combine Value
---
Use the pipe (|) symbol as an or operator in the case evaluation to check for more than one value in one case.

###### Example
---
```Python
day = int(input("Enter a day: "))
match day:
	case 1 | 2 | 3 | 4 | 5:
		print("Weekday")
	case 6 | 7:
		print("Weekend")
	case _:
		print("Other day")
```

If statement as Guards
You can add if statement in the case evaluation as an extra condition-check.

###### Example
---
```Python
month = int(input("Enter a month number: "))
day = int(input("Enter a day number: "))

match day:
	case 1 | 2 | 3 | 4 | 5 if month == 8:
		print("Weekday in August")
	case 6 | 7 if month == 8:
		print("Weekend in August")
	case _:
		print("Wrong Choice")
```