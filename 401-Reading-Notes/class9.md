# 401 Class 9 Reading Notes

## Summary: This class is about Ten Thousand 4, Statistics, Coding Guru Ethics   

Q: What is the purpose of dunder methods in Python? Provide an example of a commonly used dunder method.

Dunder methods, short for "double underscore" methods, are special methods in Python that are used to define behaviors for built-in operations. These methods are also called "magic methods" or "special methods". They are usually written with two underscores before and after the method name, like __init__().

Dunder methods are used extensively in Python to define custom classes, allowing objects of those classes to behave in ways similar to built-in types like lists or dictionaries. Some examples of commonly used dunder methods include:

__init__(): This method is called when an object of a class is created and is used to initialize the attributes of the object.

__str__(): This method is called when an object is converted to a string using the str() function. It should return a string representation of the object.

__len__(): This method is called when the built-in len() function is called on an object. It should return the length of the object.

__getitem__(): This method is called when an item is accessed using square brackets ([]) on an object. It should return the value of the item at the given index.

Here is an example of using the __str__() method:

python
Copy code
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def __str__(self):
        return f"{self.name} is {self.age} years old."
    
person = Person("Alice", 30)
print(person)  # Output: Alice is 30 years old.
In this example, the __str__() method is used to define how an instance of the Person class should be converted to a string when the print() function is called on it. The method returns a string that includes the person's name and age.

Q:In the video “AI Guru makes $238,800 with misleading paid course,” what was the main ethical issue raised concerning the use of developers’ work, and how might this have been avoided?

Does not properly credit people who he takes code from. 

Q: Describe the Python statistics module and give an example of a function within the module that can be used to perform a common statistical operation.

The Python statistics module is a built-in module that provides functions for statistical calculations. It includes functions for calculating measures of central tendency (like mean, median, and mode), measures of dispersion (like variance and standard deviation), and other statistical calculations.

One commonly used function in the statistics module is mean(). This function takes a sequence of numbers as an argument and returns the arithmetic mean (average) of those numbers.

Here is an example of using the mean() function:

python
Copy code
import statistics

data = [1, 2, 3, 4, 5]
mean = statistics.mean(data)
print(mean)  # Output: 3
In this example, we import the statistics module and create a list of numbers called data. We then call the mean() function and pass in data as an argument. The function returns the mean of the numbers in data, which is 3. We store the result in a variable called mean and print it to the console.

Other commonly used functions in the statistics module include:

median(): This function takes a sequence of numbers as an argument and returns the median (middle value) of those numbers.

mode(): This function takes a sequence of numbers as an argument and returns the mode (most common value) of those numbers.

stdev(): This function takes a sequence of numbers as an argument and returns the sample standard deviation of those numbers.

variance(): This function takes a sequence of numbers as an argument and returns the sample variance of those numbers.

## Sources: 

-ChatGPT

-https://docs.python.org/3/library/statistics.html