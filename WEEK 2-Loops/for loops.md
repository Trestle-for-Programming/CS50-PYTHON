#### For Loops
- A for loop is a different type of loop.
- To best understand a for loop, it’s best to begin by talking about a new variable type called a list in Python. As in other areas of our lives, we can have a grocery list, a to-do list, etc.
- A for loop iterates through a list of items. For example, in the text editor window, modify your cat.py code as follows:
  
```
for i in[0,1,2]:
    print("meow")
```
- Notice how clean this code is compared to your previous while loop code. In this code, i begins with 0, meows, i is assigned 1, meows, and, finally, i is assigned 2, meows, and then ends.
- While this code accomplishes what we want, there are some possibilities for improving our code for extreme cases. At first glance, our code looks great. However, what if you wanted to iterate up to a million? It’s best to create code that can work with such extreme cases. Accordingly, we can improve our code as follows:
```
for i in range(3):
    print("meow")
```
