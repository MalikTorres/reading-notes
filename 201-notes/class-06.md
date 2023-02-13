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
