# 401 Class 5 Reading Notes

## Summary: This class is about Ten Thousand Game 1 

Q: How can the random module be utilized in Python to generate random numbers or make selections from a list, and what are some common functions available within the module?

A: The random module provides functions to generate random numbers within a given range or from a specified distribution. For example, to generate a random integer between 0 and 10, you can use the randint() function:

import random

random_number = random.randint(0, 10)
print(random_number)


The random module provides functions to randomly select an element from a list or sequence. For example, to select a random element from a list of fruits, you can use the choice() function:

import random

fruits = ['apple', 'banana', 'orange', 'mango']
random_fruit = random.choice(fruits)
print(random_fruit)

Some other commonly used functions in the random module are:

random() - to generate a random float between 0 and 1
uniform(a, b) - to generate a random float between a and b
randrange(start, stop, step) - to generate a random number from the range(start, stop, step)


Q: In the context of software development, what is risk analysis, and what are the key steps involved in conducting a risk analysis for a software project?

A: Risk analysis is a process of identifying, assessing, and mitigating risks associated with a software project. In software development, risk analysis is an important step that helps project managers and development teams to identify potential problems that may arise during the project and take necessary measures to avoid or mitigate them.

-Identify potential risks that may affect the project
-Assess the likelihood and impact of each risk
-Prioritize the risks based on their likelihood and impact
-Develop a plan to mitigate the identified risks
-Monitor the project for any new risks and make adjustments to the risk management plan as needed


Q: What is test coverage and why is it an important (or potentially misleading) metric in software testing?

A: Test coverage is a metric used in software testing to measure the extent to which the source code of a software application has been tested by a particular test suite. It measures the percentage of code that has been executed by the tests in the test suite. The purpose of test coverage is to ensure that all parts of the code have been tested and to identify any untested or under-tested parts of the code.

Q: What is Big O notation, and how is it used to describe the performance of an algorithm? Give an example of an everyday task (not software related) that demonstrates O(n) time complexity.

A: In software development, Big O notation is used to analyze the performance of algorithms and to compare the efficiency of different algorithms. It is a useful tool for understanding the scalability of software applications and for identifying potential performance bottlenecks. By analyzing the time complexity of an algorithm using Big O notation, developers can optimize their code to improve performance and reduce the time and resources required to execute the algorithm.


## Sources Used: 
https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python
https://www.edureka.co/blog/risk-analysis-in-software-testing
https://martinfowler.com/bliki/TestCoverage.html
ChatGPT
https://www.youtube.com/watch?v=v4cd1O4zkGw

 ## Things I want to know more about
 Dependency Injection
 
 Dependency Injection can make software applications more flexible and easier to maintain, as it allows components to be easily replaced or updated without affecting the rest of the application. It is a powerful technique that can help to improve the modularity and extensibility of software applications.