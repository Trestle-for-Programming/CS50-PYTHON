#### Python range() Function Tutorial 
- The ```range()``` function is a very popular and widely used function in Python, especially when you are working with for loops, and sometimes also with while loops. The```range()``` function is worth knowing and mastering because doing so will open a lot of doors: ```range()``` is used in everything from controlling the flow of a program to looping through data sets that you are using for data analysis.
#### What is the range() Function in Python?
- The ```range()``` function returns a sequence of numbers and is immutable, meaning its value is fixed. The ```range()``` function takes one or at most three arguments, namely the start and a stop value along with a step size.
- ```range()``` was introduced in Python3. In Python2, a similar function, ```xrange()```, was used, which had somewhat different behavior. Among other things, ```xrange()``` returned a generator object and consumed less memory, while ```range()```, on the other hand, returns a list or sequence of numbers.
- Part of the reason the range() function is useful is because it only stores the start, stop, and step values, so it consumes less memory when compared to a list or tuple.
#### Python range() Function Syntax
- The ```range()``` function can be represented in three different ways, or you can think of them as three range() parameters:
- ```range(start_value, stop_value)```: This generates the sequence based on the start and stop value.
- ```range(start_value, stop_value, step_size)```: It generates the sequence by incrementing the start value using the step size until it reaches the stop value.
