# 401 Class 4 Reading Notes

## Summary: This class is about Classes, Objects, Tests in Python 

### Classes and objects are important in object-oriented programming as they enable developers to organize code into reusable components, encapsulate data and behavior, and facilitate code reuse, leading to more efficient and scalable code.

**Qp**: What are the key differences between classes and objects in Python, and how are they used to create and manage instances of a class?

**A**:In Python, a class is a blueprint or a template that defines the properties and behavior of an object. An object is an instance of a class that contains specific values for the properties defined by the class. Here are the key differences between classes and objects:

- Definition: A class is a code template that defines a set of properties and methods that are common to all objects of that class. An object is an instance of a class that contains specific values for the properties defined by the class.

- Memory: A class is a logical entity, whereas an object is a physical entity. A class is stored in the program's memory once, and many objects can be created from it.

- Access: A class defines the attributes and methods that an object can have, but it does not have any specific values for those attributes. An object has specific values for the attributes defined by the class, and these values can be accessed using dot notation.

- Instantiation: A class can be instantiated to create an object. Instantiation is the process of creating an instance of a class.

To create an instance of a class, you need to follow these steps:

Define the class: You first need to define the class that you want to instantiate.

Instantiate the class: To instantiate a class, you create an object of the class by calling the class name followed by parentheses.

Access the object: You can then access the object's properties and methods using dot notation.

Here's an example of how to create and manage instances of a class in Python:

python
Copy code
# Define the class
class Car:
    def __init__(self, make, model, year):
        self.make = make
        self.model = model
        self.year = year
    
    def start(self):
        print("The car is starting")

# Instantiate the class
car1 = Car("Toyota", "Corolla", 2022)
car2 = Car("Honda", "Civic", 2021)

# Access the object's properties
print(car1.make)
print(car1.model)
print(car1.year)

# Access the object's method
car1.start()
In this example, we define a Car class with make, model, and year properties, as well as a start() method. We then instantiate the class twice, creating car1 and car2 objects. We can access the properties of the objects using dot notation, and we can call the start() method of car1 using the same notation.





**Qp**: Explain the concept of recursion and provide an example of how it can be used to solve a problem in Python. What are some best practices to follow when implementing a recursive function?

**A**:Recursion is a programming concept that involves solving a problem by breaking it down into smaller, simpler versions of the same problem until the smallest possible version of the problem is reached. Recursion can be thought of as a function that calls itself.

When a function calls itself, it creates a new instance of the function on the stack. Each instance of the function has its own set of variables and executes independently. When the function returns, it pops the current instance off the stack and continues executing from where it left off in the previous instance.

Recursion is often used to solve problems that can be broken down into smaller, simpler versions of the same problem. For example, calculating the factorial of a number involves multiplying the number by the factorial of the number minus one. This can be expressed recursively as:

arduino
Copy code
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)
This function calculates the factorial of n recursively by multiplying n by the factorial of n - 1. The base case of the recursion is when n equals 0, in which case the function returns 1.

When implementing a recursive function, there are a few best practices to follow:

Define a base case: The base case is the condition in which the recursion ends. Without a base case, the function will continue to call itself indefinitely.

Ensure progress is made towards the base case: Each recursive call should make progress towards the base case. If progress is not made, the function will continue to call itself indefinitely.

Use the call stack appropriately: Recursion uses the call stack to store function calls. If the call stack becomes too deep, it can cause a stack overflow error.

Consider efficiency: Recursion can be less efficient than iterative solutions. In some cases, it may be better to use an iterative solution instead of a recursive one.

Overall, recursion can be a powerful tool for solving certain types of problems in Python. By breaking a problem down into smaller, simpler versions of the same problem, recursion can lead to elegant and efficient solutions. However, it is important to follow best practices to avoid issues like stack overflow and ensure that the function works as expected.


**Qp**: What is the purpose of pytest fixtures and code coverage in testing Python code? Explain how they can be used together to improve the quality and maintainability of a project.

**A**:Pytest fixtures and code coverage are two important concepts in testing Python code that can be used together to improve the quality and maintainability of a project.

Pytest fixtures are functions that provide a fixed baseline for a test. They are used to set up preconditions for the test, such as creating a test database or initializing a web client. Fixtures can be reused across multiple tests, making them a powerful tool for reducing duplication and improving the maintainability of test code.

Code coverage, on the other hand, is a measure of how much of the code in a project is executed during testing. It can be used to identify areas of the code that are not being tested, which can help improve the overall quality of the project.

By using pytest fixtures and code coverage together, you can ensure that your tests are comprehensive and that they cover as much of the code as possible. Here's an example of how this can be done:

python
Copy code
# test_sample.py
import pytest
from myproject import sample

@pytest.fixture
def some_data():
    return [1, 2, 3, 4, 5]

def test_sum(some_data):
    assert sample.sum_list(some_data) == 15

def test_average(some_data):
    assert sample.average_list(some_data) == 3

# conftest.py
import pytest
from myproject import sample

@pytest.fixture
def some_data():
    return [1, 2, 3, 4, 5]

# pytest --cov=myproject
# pytest --cov=myproject --cov-report=html

In this example, we define two tests in test_sample.py that use a fixture called some_data to provide a list of numbers to the functions being tested. We also define a fixture in conftest.py that does the same thing.

By running pytest --cov=myproject, we can generate a code coverage report that shows which lines of code were executed during the tests. This can help us identify areas of the code that are not being tested and may need additional testing.

By using pytest fixtures and code coverage together, we can ensure that our tests are comprehensive, efficient, and maintainable. Fixtures help reduce duplication in test code and improve the readability of tests, while code coverage helps us identify areas of the code that may need additional testing.



## Sources:

ChatGPT4

https://www.learnpython.org/en/Classes_and_Objects

https://realpython.com/python-thinking-recursively/

https://www.learnpython.org/en/Classes_and_Objects

https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage


## Things I want to know more about:

Anatomy of a test: 

You can think of a test as being broken down into four steps:

 - Arrange

- Act

- Assert

- Cleanup

Arrange is where we prepare everything for our test. This means pretty much everything except for the “act”. It’s lining up the dominoes so that the act can do its thing in one, state-changing step. This can mean preparing objects, starting/killing services, entering records into a database, or even things like defining a URL to query, generating some credentials for a user that doesn’t exist yet, or just waiting for some process to finish.

Act is the singular, state-changing action that kicks off the behavior we want to test. This behavior is what carries out the changing of the state of the system under test (SUT), and it’s the resulting changed state that we can look at to make a judgement about the behavior. This typically takes the form of a function/method call.

Assert is where we look at that resulting state and check if it looks how we’d expect after the dust has settled. It’s where we gather evidence to say the behavior does or does not aligns with what we expect. The assert in our test is where we take that measurement/observation and apply our judgement to it. If something should be green, we’d say assert thing == "green".

Cleanup is where the test picks up after itself, so other tests aren’t being accidentally influenced by it.

At its core, the test is ultimately the act and assert steps, with the arrange step only providing the context. Behavior exists between act and assert.

https://docs.pytest.org/en/latest/explanation/anatomy.html#test-anatomy


https://www.learnpython.org/
