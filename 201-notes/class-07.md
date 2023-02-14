## Class 7


### Domain Modeling

Explain why we need domain modeling.

Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that is articulated well can verify and valid your understanding of the problem. As problem solving is intergral as a software developer domain modeling is essential for outline what needs to be done to complete the task. 


### HTML Table Basics

Why should tables not be used for page layouts?

* They decreased webpage accessibility for users who are visually impaired.
* They include complex markup structures, leading to harder to write code
* Tables are not automatically reponsive.

List and describe 3 different semantic HTML elements used in an HTML `<table>`.

`<table>` is used to enclose the content in the table.

`<td>` element is the smallest container inside a table and called is a table cell.

`<tr>` is then used to create table rows

### Introducing Constructors

What is a constructor and what are some advantages to using it?

Constructors are functions that are called using the `new` keyword, when a constructor is called it

* creates a new object 

* bind `this` to the new object, so you can refer to `this` in your constructor code

* run the code in the constructor

* return the new object

> 
    function Person(name) {
      this.name = name;
      this.introduceSelf = function () {
        console.log(`Hi I'm ${this.name}. `);
      };
    }

>

to call `Person()` as a constructor, we use `new`
>
    constr salva = new person("Salva");
    salva.name;
    salva.introduceSelf();

    constr frankie = new Person("Frankie");
    frankie.name;
    frankie.introduceSel(); 

>

How does the term this differ when used in an object literal versus when used in a constructor?

Since constructors are used to create multiple objects. `This` is intergral as it is dynamic and can be referred in different objects in our constructor code.

### Object Protoypes Using A Constructor

Explain prototypes and inheritance via an analogy from your previous work experience.

While working at my last job we would take time to develop a workflow for each of our task. This would function as a unified guide for our role and responsibilities, that way when you members joined our team they would be able to simply follow the guide that was passed on to each of my team memebers, and if a team member left another person could inherit their task seemlessly. 

For reference: prototpe is just a property that every function in JavaScript has and allows us to share methods accross all instances of a function. 



NOTE: This is a very common front end developer interview question


### Things I want to know more about

I would like to know more about oop in JavaScript and creating classes

references:

* [Object Prototypes Using A Constructor](https://ui.dev/beginners-guide-to-javascript-prototype)

* [Introducing Constructors](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)

* [HTML Table Basics](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics) 

* [Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)