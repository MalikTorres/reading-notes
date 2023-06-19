## Class 26 Notes

### React Quick Start 

#### What are the building blocks of a React app?

React apps are made out of components.

#### What is the difference between an HTML element and a React component?

Eact component has it's own piece of logic that applies to the UI

#### What is JSX and why do we use it?

It's mostly used for is conveience 

#### Describe the process of embedding JavaScript expressions in JSX.

They're typically wrapped in `<div></div>` or empty `<></>`

##### Does React or JSX have any special features for iteration or conditional logic?

Certain options for more compact usage of if else are

```
<div>
  {isLoggedIn ? (
    <AdminPanel />
  ) : (
    <LoginForm />
  )}
</div>
```
```
<div>
  {isLoggedIn && <AdminPanel />}
</div>
```

#### How does React know to respond to a user’s inputs?

You pass down the handler in the return

#### What word indicates that a React component manages data with a Hook?

use, for example useState


#### How can two react components share data?

The state needs added to a shared component

### Render and Commit

#### What are the three steps of refreshing a React UI?

Triggering a render (delivering the guest’s order to the kitchen)
Rendering the component (preparing the order in the kitchen)
Committing to the DOM (placing the order on the table)


#### How do you trigger updates to a component after the initial render?

`createRoot` has to be called

#### Does React recreate DOM nodes on every rerender?

It doesn't

#### After React has updated the DOM, what still needs to happen before the user sees the change? 

A rerender 


### Additional Questions

#### Note the naming conventions in the Airbnb React/JSX Style Guide. What pattern(s) do you see?

Double quotes for JSX and single JavaScript.
No padding JSX curly braces with spaces

#### Looking ahead at this module’s course schedule, What do you look forward to learning?

Having a better grasp of React

#### What are your learning goals after reading and reviewing the class README?

Writing functional components

#### Things I want to know more about

How to manage state in React and Hooks