## Class 4 Reading

#### Forms

What is a ‘Controlled Component’?

In React, mutable state is usually kept in the state property of components, and only updated with `setState()` The two can be comombied by making the React state be the "single source of truth". Then the React component that renders a form also controls what happens in that form on user input. An input form element whose value is controlled by React in this manner is called a "conntrolled component"

Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

We should update the state with user responses as soon as they enter them. This will allow the displayed output to update as the user types. 



How do we target what the user is entering if we have an event handler on an input field? 

we can target the value that is being entered. 


#### Ternary Operator

Why would we use a ternary operator?

It requires less code than a traditional if statement, can efficiently test multiple conditions.

Rewrite the following statement using a ternary statement

`x===y ? console.log(true) : console.log(false)`

### Things I want to know more aboout

How to use state