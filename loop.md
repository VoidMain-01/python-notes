for loop
---------
for loop only works with iterable objects but for non-iteration objects it raises an error (TypeError) [Object is not iterable].

Syntax: 

for <variable> in <iterable-objects>:
	statement
	[statements]

Examples of iterable - List, Tuple, Dictionary, range(), String

Iterables - It is an object that can be looped over (iterated) to return its element one at a time.

x = 2456
for i in x: 
	print(i)