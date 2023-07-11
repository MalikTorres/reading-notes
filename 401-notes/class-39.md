# class 39

Redux Toolkit (RTK)

What concerns are addressed by Redux Toolkit?

"Configuring a Redux store is too complicated"
"I have to add a lot of packages to get Redux to do anything useful"
"Redux requires too much boilerplate code

What does configureStore() do?

`configureStore()`: wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes `redux-thunk` by default, and enables use of the Redux DevTools Extension.

How would I use createSlice()?

`createSlice()`: accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.

MobX

What is Mobx?

MobX is a simple, scalable and battle tested state management solution.

How does MobX make it “impossible” to produce an inconsistent state?

Observable State: In MobX, state variables that need to be observed and tracked for changes are marked as observables.

How would we build a reactive user interface?

Define Observables: Identify the state variables in your application that need to be observed for changes. 

Tutorial

What take-away(s) did this tutorial provide?

Some takeaways are 

Redux Toolkit: Redux Toolkit is the recommended approach for writing Redux logic. It simplifies Redux usage patterns and provides a standardized way of using Redux.

Redux Essentials: The Redux Essentials tutorial is a great starting point for beginners. It teaches how to use Redux Toolkit to build a real-world example application and introduces Redux concepts along the way.


### Things I want to know more about

How to use redux toolkit