# for loop
-
for loop only works with iterable objects but for non-iteration objects it raises an error (TypeError) [Object is not iterable].

## Syntax: 

```Python
for (variable) in (iterable-objects):
	statement
	[statements]
```
Examples of iterable - List, Tuple, Dictionary, range(), String

Iterables - It is an object that can be looped over (iterated) to return its element one at a time.

```Python
x = 2456
for i in x: 
	print(i) # It will throw error
```
```Python
st = "LIT INDIA"
for i in st:
	print(i)
```
range() - It will internally generate an mutable object which is a list.

range(stop_value) - It will start from 0 end at stop - 1
range(start_vale, stop_value) - It will start from start_value and end at stop_value - 1
range(start_value, stop_value, step_value) - It will start from given value and end at stop_value - 1 and it will increase to given step_value.

#### Example: 
###### WAP to print whole number till 15.
```Python
for x in range(15 + 1):
	print(x, end = ", ")
```
---
```Python
for i in range(5, 51):
	print(i, end = ", ")
```
Default step value is *1*.

```Python
for x in range(25, 0, -1):
	print(x, end = ", ")
```
###### Wap to display the sum of the numbers from 5 to 100 increase each value by 2
```Python
sum = 0
for x in range(5, 101, 2):
	sum += x

print(sum)
```
