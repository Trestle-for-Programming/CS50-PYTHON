# While Loops

The `while` loop is a fundamental control structure found in nearly all programming languages. It repeatedly executes a block of code as long as a specified condition remains true.

## Key Characteristics
- Repeats code until its condition becomes false
- Requires careful setup to avoid infinite loops
- Universally implemented across programming languages

## Example: Infinite Loop (Bug)
```python
i = 3
while i != 0:
    print("meow")
```
## Understanding Infinite Loops

⚠️ **Critical Observation**:  
The initial loop example will run **forever** despite appearing to have an exit condition:  
```python
i = 3
while i != 0:
    print("meow")
```
#### Why This Loops Forever
- Initial state: i = 3

- Condition check: i != 0 → True

- Loop execution: Prints "meow"

- Missing update: i remains 3 forever
- → Condition stays True indefinitely

#### How while Loops Work
**1. Before every iteration, the interpreter asks:**
- "Does the condition still evaluate to True?"
- In this case: "Is i not equal to 0?" → Always yes
  
**2. Breaking Out of Infinite Loops**
- When trapped in an endless loop:
i. Keyboard interrupt: Press Ctrl + C
(Sends termination signal to program)
ii. Terminal behavior:
- Returns command prompt
- Shows KeyboardInterrupt error

| Iteration | `i` Value | Condition `i != 0` | Result          |
|-----------|-----------|--------------------|-----------------|
| 1         | 3         | True               | Prints "meow"  |
| 2         | 3         | True               | Prints "meow"  |
| ...       | ...       | ...                | ...            |
| ∞         | 3         | Always True        | Infinite "meow"|

graph TD
    A([Start]) --> B["i = 0"]
    B --> C{"i < 3 ?"}
    C -- True --> D["print 'meow'"]
    D --> E["i += 1"]
    E --> C
    C -- False --> F([Stop])

    
