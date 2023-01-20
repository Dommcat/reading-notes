# 301 Reading Notes

## Class 10 Summary: This class is about memory storage

What is a ‘call’?

How many ‘calls’ can happen at once?

What does LIFO mean?
Last In, First Out (LIFO) means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

image.png

function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();

What causes a Stack Overflow?
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

SOURCE: <https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4>

What is a ‘reference error’?
variable that is not yet declared

What is a ‘syntax error’?
something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

What is a ‘range error’?
manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

What is a ‘type error’?
errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

What is a breakpoint?
 see what has happened before that point and you can try and evaluate the next lines to check if everything is outputting what you are expecting.

What does the word ‘debugger’ do in your code?
debugger statement in your code in the line you want to break.

<https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c>

<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors>

## Things I want to know more about
