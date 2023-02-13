## JavaScript Object Basics

1.How would you describe an object to a non-technical friend you grew up with?

`objects` are essentially another data type in JavaScript, they typically consist of, variables and functions, which are referred to as properties and methods when they are inside objects. 


2.What are some advantages to creating object literals?

Object literals are typically used to transfer a series of structured related data items. An expample would be sending a request to a server.This is easier than sending multiple items separately.


3.How do objects differ from arrays?

Properties can be accessed by name whereas arrays values are accessed by their index.





4.Give an example for when you would need to use bracket notation to access an 
object’s property instead of dot notation.

Bracket notation can be used to accessed properties in the object if the property name is stored in a variable. Whereas dot notation cannot be used. Dot notation is still more preferable as it is more succinct. 


>
    const person = {
     name: ["Bob", "Smith"],
     age: 32,
    };

    function logProperty(propertyName) {
    console.log(person[propertyName]);
    }

    logProperty("name");
    // ["Bob", "Smith"]
    logProperty("age");
    // 32
> 
5.Evaluate the code below. What does the term this refer to and what is the advantage to using this? 

`this` keyword referes to the current object the code is being written inside.  `this` enables you to use the same method definition for every object you create.

>
    const dog = {
    name: 'Spot',
    age: 2,
    color: 'white with black spots',
    humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
} 

>
`this` is referring to the name property and age property.  

##Introduction to the DOM 

1.What is the DOM?

**The Document Object Model** is the data repsentation of the objects that comprise structure and content of a document on the web. It is a programming interface for web douments. It represents the web page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects so prgramming languages can interact with the page. 

2.Briefly describe the relationship between the DOM and JavaScript.

The DOM essentially allows web pages to interact with JavaScript. Without the DOM JavaScript would not have a way to access the components of a webpage. Example of DOM

>    
    const paragraphs = document.querySelectorAll("p");
    // paragraphs[0] is the first <p> element
    // paragraphs[1] is the second <p> element, etc.
    alert(paragraphs[0].nodeName)
>
in this example DOM specifies `querySelectorAll` method in this code snippet must return a list of all the `<p>` elements in the document. 

Common APIs in web and XML page scripting using the DOM


* `document.querySelector(selector)`
* `document.querySelectorAll(name)`
* `document.createElement(name)`
* `parentNode.appendChild(node)`
* `element.innerHTML`
* `element.style.left`
* `element.setAttribute()`
* `element.getAttribute()`
* `element.addEventListener()`
* `window.content`
* `Window.onload`
* `window.scrollTo()`


### Things I want to know more about

Using constructor functions

References:

*[JavaScript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)