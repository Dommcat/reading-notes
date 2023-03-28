# 401 Class 7 Reading Notes

## Summary: This class is about Ten Thousand 2 

In Python, **global** and nonlocal are keywords used to specify the scope of a variable within a function.

**global** is used to indicate that a variable is defined in the global scope, i.e., outside the function, and is accessible throughout the program. If you want to modify the value of a global variable from within a function, you need to use the global keyword to tell Python that you are referring to the global variable, rather than creating a new local variable with the same name.

Here's an example:

csharp
Copy code
x = 10

def foo():
    global x
    x += 1
    print(x)

foo()  # prints 11


In this example, **global** x tells Python to use the global variable x instead of creating a new local variable with the same name. x += 1 modifies the value of the global variable, and print(x) prints the new value of x.

**nonlocal** is used to indicate that a variable is defined in the enclosing scope of the current function, but not in the global scope. This is useful when you have nested functions and want to modify the value of a variable in the outer function from within the inner function.

Here's an example:

python
Copy code
def outer():
    x = 10
    def inner():
        nonlocal x
        x += 1
        print(x)
    inner()

outer()  # prints 11


In this example, **nonlocal** x tells Python to use the variable x defined in the outer() function, rather than creating a new local variable with the same name in the inner() function. x += 1 modifies the value of the variable defined in the outer function, and print(x) prints the new value of x.


Big O notation is a way to describe the time complexity of an algorithm, i.e., how long it takes to run as a function of the size of the input. It is a measure of the worst-case scenario, which means the maximum amount of time an algorithm could take to run.


To simulate a dice roll using Python, we can use the random module, which provides functions for generating random numbers. Specifically, we can use the randint function, which generates a random integer between a specified range.

python
Copy code
import random

# simulate a dice roll
dice_roll = random.randint(1, 6)

print(dice_roll)
In this example, we use the randint function to generate a random integer between 1 and 6, which represents the possible outcomes of rolling a dice.

To calculate the probability of rolling a specific number over a large number of trials, we can use a loop to simulate multiple dice rolls and count the number of times the specific number is rolled. We can then divide the number of times the specific number is rolled by the total number of rolls to calculate the probability.

Here is an example of calculating the probability of rolling a 6 over 1000 dice rolls:

python
Copy code
import random

num_rolls = 1000
specific_number = 6
count = 0

for i in range(num_rolls):
    dice_roll = random.randint(1, 6)
    if dice_roll == specific_number:
        count += 1

probability = count / num_rolls

print(f"The probability of rolling a {specific_number} is {probability}")
In this example, we use a loop to simulate 1000 dice rolls and count the number of times a 6 is rolled. We then divide the count by the total number of rolls to calculate the probability of rolling a 6.





## Sources/tools used:
Chat GPT
W3 Schools
https://realpython.com/python-scope-legb-rule/