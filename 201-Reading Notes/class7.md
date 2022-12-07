# 201 Reading Notes: Class 07

## Summary: This class reading assignment is about Object-Oriented Programming and HTML Tables

### Domain Modeling

Explain why we need domain modeling.

-A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders.

HTML Table Basics

Why should tables not be used for page layouts?

-Layout tables reduce accessibility for visually impaired users
-Tables produce tag soup
-Tables are not automatically responsive

[List and describe 3 different semantic HTML elements used in an HTML.]

[Source]<https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Advanced>

### Introducing Constructors

What is a constructor and what are some advantages to using it?

**Using object literals is fine when you only need to create one object, but if you have to create more than one, as in the previous section, they're seriously inadequate. We have to write out the same code for every object we create, and if we want to change some properties of the object - like adding a height property - then we have to remember to update every object.**

How does the term this differ when used in an object literal versus when used in a constructor?

 better way is to use a constructor. A constructor is just a function called using the new keyword. When you call a constructor, it will:

create a new object bind this to the new object, so you can refer to this in your constructor code run the code in the constructor return the new object.

### Object Prototypes Using A Constructor

[Source]<https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors>
Explain prototypes and inheritance via an analogy from your previous work experience.

NOTE: This is a very common front end developer interview question

[SOurce] <https://ui.dev/beginners-guide-to-javascript-prototype>

## Things I want to know more about

Better understanding of object oriented language vs other non object oriented programming languages
