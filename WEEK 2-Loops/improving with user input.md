# Improving User Input Validation in Python

- Input Validation Paradigm
Python commonly uses `while` loops to validate user input. This ensures the program only proceeds with acceptable data.

- Initial Validation Approach
```python
while True:
    n = int(input("What's n? "))
    if n < 0:
        continue  # Skip to next iteration
    else:
        break  # Exit loop

# After validation
for _ in range(n):
    print("meow")
```
- Notice that we’ve introduced two new keywords in Python, continue and break. continue explicitly tells Python to go to the next iteration of a loop. break, on the other hand, tells Python to “break out” of a loop early before it has finished all of its iterations. In this case, we’ll continue to the next iteration of the loop when n is less than 0—ultimately reprompting the user with “What’s n?”. If, though, n is greater than or equal to 0, we’ll break out of the loop and allow the rest of our program to run.
- It turns out that the continue keyword is redundant in this case. We can improve our code as follows:
```python
while True:
    n = int(input("What's n? "))
    if n > 0:
        break

for _ in range(n):
    print("meow")
```
- Notice how this while loop will always run (forever) until n is greater than 0. When n is greater than 0, the loop breaks.Bringing in our prior learning, we can use functions to further improve our code:
```python
def main():
    meow(get_number())


def get_number():
    while True:
        n = int(input("What's n? "))
        if n > 0:
            return n


def meow(n):
    for _ in range(n):
        print("meow")


main()
```
- Notice how not only did we change your code to operate in multiple functions, but we also used a return statement to return the value of n back to the main function.
