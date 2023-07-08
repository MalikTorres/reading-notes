# Class 38 notes

### async actions

Why use Redux middleware?

Centralized state management, React Redux provides a centralized store for managing the state of your application. instead of passing down state and callbacks through multiple levels of componenets

Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.

This process starts when an async action is dispatched. The action is typycally triggered by a user interaction or component lifecycle event.

How are we accommodating async in our Redux app?

Being used with Redux Thunk: It extends Redux's capabilities by allowing action creators to return functions instead of plain objects.


### thunk middleware

Why would you need `redux-thunk` middleware?

You need the redux-thunk  middleware in your Redux application to handle asyncronous operations an enable the use of async action creators.

Redux Thunk middleware allows you to write action creators that return a ____ instead of an action.

Redux Thunk middleware allows you to write action creators return a `function` instead of an action.

Describe how any return value from the inner thunk function will be made available.

In Redux, when a thunk a function is dispatched, any return value from the inner thunk function is not automatically made avaliable outside the thunk.


### Reflection

What are your learning goals after reading and reviewing the class README?

Understanding more about redux

### Things I want to know more about

I would like to know more about asyncronous actions.