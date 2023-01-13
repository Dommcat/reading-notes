# 301 Reading Notes

## Class 5 Summary; This class is about Readings: Putting it all togeather

Q: What is the single responsibility principle and how does it apply to components?
A: The component should ideally only do one thing

Q: What does it mean to build a ‘static’ version of your application?
A: version that takes your data model and renders the UI but has no interactivity

Q: Once you have a static application, what do you need to add?
A: Pass data using props. props

Q: What are the three questions you can ask to determine if something is state?
A:
-Is it passed in from a parent via props? If so, it probably isn’t state.
-Does it remain unchanged over time? If so, it probably isn’t state.
-Can you compute it based on any other state or props in your component? If so, it isn’t state.

Q: How can you identify where state needs to live?
A: Identify which component mutates, or owns, this state.

[Source] <https://reactjs.org/docs/thinking-in-react.html>

## Q: What are hire ordered funtions?

A: Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions.

Q: What is a “higher-order function”?
A: Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions.

Q: Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
A: return method greater than or = 11

Q: Explain how either map or reduce operates, with regards to higher-order functions.
A: The map method transforms an array by applying a function to all of its elements and building a new array from the returned values.
A: Another common thing to do with arrays is to compute a single value from them. Our recurring example, summing a collection of numbers, is an instance of this.

[Source] <https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK>

## Things I want to know more about
