# 401 Advanced Python: Class 42 Reading Notes

## Summary: This class reading is about: Pythonisms

What are dunder methods in Python, and how do they allow for the customization of built-in behavior in classes? Provide an example of a common dunder method and its purpose.

Dunder methods, also known as magic methods or special methods, are predefined methods in Python classes that allow customization of the built-in behavior of objects. They are identified by their double underscore (dunder) naming convention.
- enable the customization of operations such as arithmetic, comparisons, string representations, and more.
- One common dunder method is `__str__`, used to provide a string representation of an object. It overrides the default behavior of the `str()` function.
- Dunder methods provide a way to define how objects of a class interact with Python's built-in operations and functions, allowing for a more intuitive and consistent interface.

Explain the concept of an iterator in Python. How do you create a custom iterator using the iter() and next() methods, and why are they important for enabling iteration in a class?

- An iterator in Python allows you to traverse a collection of elements or customize iteration over an object.
- Iterators implement the iterator protocol, which involves the use of `iter()` and `next()` methods.
- The `iter()` method returns an iterator object from an iterable, and `next()` retrieves the next element from the iterator.
- To create a custom iterator, define a class that implements `__iter__()` and `__next__()` methods.
- The `__iter__()` method should return the iterator object itself (`self`), and `__next__()` should return the next element or raise `StopIteration`.
- Custom iterators allow you to control the iteration logic within your class.
- The iterator protocol is important for enabling iteration in a class as it allows objects to be used in `for` loops and other constructs that require iteration.
- It provides a standardized way to iterate over different types of objects and facilitates the creation of iterable and iterable objects in Python.

What is a generator in Python, and how does it differ from a regular function? Illustrate your answer with an example of a generator function using the ‘yield’ keyword.
- A generator in Python is a special type of function that generates a sequence of values, one at a time, using the `yield` keyword.
- Generators use lazy evaluation, generating values on-demand instead of calculating and returning all values at once like regular functions.
- Generator functions retain their state between calls, allowing them to resume execution from where they left off.
- Generators are iterable objects and can be used in `for` loops or other constructs that expect an iterable.
- Generators are memory-efficient, especially for large datasets or infinite sequences.
- Example: A generator function `fibonacci_generator()` generates Fibonacci numbers using an infinite loop and the `yield` keyword. It can be iterated over to retrieve Fibonacci numbers one at a time.

Define decorators in Python and explain their primary use case. How can you create and apply a custom decorator to a function or method? Provide a simple example to demonstrate this concept.

- Decorators in Python allow you to modify the behavior of functions or classes without changing their source code.
- A decorator is a function that takes another function as input, adds functionality to it, and returns a modified version of the original function.
- Decorators are primarily used to separate cross-cutting concerns and enhance the functionality of existing code.
- Decorators can be created by defining a decorator function that takes the target function as an argument and returns a modified version of it.
- To apply a decorator, use the `@decorator_name` syntax above the target function or method definition.
- Decorators provide a way to add features like logging, timing, input validation, or caching to functions or methods.
- Example: The `log_function_call` decorator logs the name and arguments of a function when it is called, enhancing the original function's behavior.


## Re/Sources:

ChatGPT

https://realpython.com/lessons/what-are-python-generators/

https://dbader.org/blog/python-dunder-methods

https://realpython.com/primer-on-python-decorators/



## Things I want to know more about
stuff behind the built in code 