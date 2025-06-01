#### Definition and Usage
The `range()` function returns a sequence of numbers with these characteristics:
- Starts from `0` by default
- Increments by `1` by default
- Stops **before** a specified number (exclusive)

#### Syntax
```python
range(start, stop, step)
```
| Parameter | Description |
|-----------|-------------|
| `start`   | Optional. An integer specifying the starting position (default = `0`) |
| `stop`    | **Required**. An integer specifying where to stop (this value is **not included** in the sequence) |
| `step`    | Optional. An integer specifying the increment value (default = `1`) |
#### Python range() Function Examples:
1.  Using Python range() to print a sequence of numbers
   - Let's start with a simple example of printing a sequence of ten numbers, which will cover your first range() parameter. To achieve this, you will be just passing in the stop value. Since Python works on zero-based indexing, hence, the sequence will start with zero and stop at the specified number, i.e., $n-1$, where $n$ is the specified number in the range() function.
     ```
     range(10) #it should return a lower and an upper bound value.
     range(0, 10)
     for seq in range(10):
     print(seq)
     
     ```
2. Using Python range() with list()
   - You could also use the range function as an argument to a list in which case it would result in a list of numbers with a length equal to the stop value as shown below:

    ```
     list(range(10))
    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
    len(list(range(10)))
    10
    ```
