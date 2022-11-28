# 201 Class 1 Reading Notes

## Summary: This class is about how the web works and intro to HTML and JS

How the Web Works.
<https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works>

Website Design and Process.
<https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/What_will_your_website_look_like>

What is JavaScript?”
<https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics>

### HTTP Haiku Short Poem

<p> Computers language connect,
clients and servers,
requests responses.</P>

Describe how HTML, CSS, and JS files are “parsed” in the browser.
Parsing; Once the browser receives the first chunk of data, it can begin parsing the information received. Parsing is the step the browser takes to turn the data it receives over the network into the DOM and CSSOM, which is used by the renderer to paint a page to the screen.

Q; How can you find images to add to a Website?
A: Use Google images OR unsplash.com

Q: How do you create a String vs a Number in JavaScript?
A: If you have a numeric variable that you want to convert to a string but not change otherwise, or a string variable that you want to convert to a number but not change otherwise, you can use the following two constructs:

The Number object converts anything passed to it into a number, if it can. Try the following:
const myString = "123";
const myNum = Number(myString);
console.log(typeof myNum);
Copy to Clipboard
Conversely, every number has a method called toString() that converts it to the equivalent string. Try this:
const myNum2 = 123;
const myString2 = myNum2.toString();
console.log(typeof myString2);

Q: What is a Variable and why are they important in JavaScript?
A: A variable is a container for a value, like a number we might use in a sum, or a string that we might use as part of a sentence.

[SOURCE] <https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Strings>

## Introduction to HTML

-What is an HTML attribute?
Attributes contain extra information about the element that won't appear in the content. In this example, the class attribute is an identifying name used to target the element with style information.

-Describe the Anatomy of an HTMl element.
The opening tag
The content
The closing tag

-What is the Difference between <article> and <section> element tags
-What Elements does a “typical” website include?
-How does metadata influence Search Engine Optimization?

-How is the <meta> HTML tag used when specifying metadata?
Metadata is data that describes data, and HTML has an "official" way of adding metadata to a document — the <meta> element.

[Source] https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#adding_a_title

## Things I want to know more about
Meta Data and SEO Search Engine Optimizing