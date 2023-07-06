# Class 37

### Multiple Reducers Example

Why create multiple reducers?

Multiple reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

How would you combine multiple reducers?

I would use the `comebineReducer` function from Redux, or a state management library?

How will you manage state as an immutable object? why?

State managed this way can lead to performance improvements.

### Redux Docs: Using Combined Reducers

combineReducers is a utility function to simplify the most common use case when writing ___ _____ .


Redux

Explain how combineReducers assembles the new state tree.

When the root reducer receives an action, it delegates the handling of that action to each individual reducer, and then combines the results into a new state tree.

How would you define initial state in an app using combineReducers?


When using `combineReducers` in Redux to manage state in your application, you define the state for each individual reducer separately. The initial state defines the starting values for each slice of the state managed by the reducers.

### Redux Docs: Combined Reducer Syntax

Why will you want to split your reducing functions as your app becomes more complex?

In order to manage independent parts of the state.


The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____.

The `combineReducers` helper function turns an object whose values are different reducing functions into a single function you can pass to `createStore`.

What is a popular convention when naming reducers?

Descriptive names that indicate the portion of state the reducer is responsible for.


Reflection

What are your learning goals after reading and reviewing the class README?

Have a high level grasp of redux

### Things I want to know more about? 

How to work with the `comebineReducer` hook