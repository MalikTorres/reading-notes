## Class 9 Readings

### HTML Forms

Why are forms so important in web development?

Forms are one of the main points of interaction between a user and website or application. Forms allow users to enter data. This data is then sent to a webserver for processing. Or used on the client=side to update the interface in some way. Forms are made up of **form controls**


When designing a form, what are some key things to keep in mind when it comes to user experience?

It is important to make sure that you're only gathering the necessary information from the user. As the bigger the form the more it overcomplicates things.

List 5 form elements and explain their importance.

`form` element defines a form, similar to `section` or `footer` elements. 

`button` element allows a user to send or submit their data once they have filled out their form

`label` element reprents a caption for an item in a user interface.

`textarea` element represents a multi-line plain text editing control, which is useful when allowing users to enter a sizeable amount of free form text. 

`input` element is used to create interactive controls for web-based forms in order to accept data from the user. 


### Introduction To Events

How would you describe events to a non-technical friend?

Events are essentialy reactions that occur after performing a certain action. 

When using the addEventListener() method, what 2 arguments will you need to provide?

The name of the event you want to register the handler for, and the code that compromises the function in reseponse to it.


Describe the event object. Why is the target within the event object useful?

The target property of the event object is a reference to teh element the event occured upon.

What is the difference between event bubbling and event capturing?

Event bubbling describes how the browser handles events targetd in nested elements. Event capturing is similar to event bubbling but in revers order. Instead of the event firing first on the innermost targets, and then on the sucessively less nested elements, the event fires first on the least nested element, and then on the successively more nested elements, until the target is reached.

### Things I want to learn more about 

How to apply and use event listeners and event objects


### references:

* [Event listeners](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events#event_objects)