## Class 2 Reading notes

#### React Lifecyle

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

 `render` occurs before `componentDidMount`

2. What is the very first thing to happen in the lifecycle of React?

  The first thing is that occured is that the constructor method is called before anything else occurs.

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

  The order is: Contructor, static, getDerivedStateFromProps,render,componentDidMount, and UNSAFE_componentWillMount.

4. What does componentDidMount do?

  This method is invoked immediate after a component is mounted. An effective method to use if you need upload anything using a network request or initialize the DOM.



#### React State Vs Props

1. What types of things can you pass in the props?
    
    What can be passed are essentially arguements, what you want the component to be initialized to. 

2. What is the big difference between props and state?

   Props are passsed into and a component, and handled outside the component. State is handled inside of the component.

3. When do we re-render our application?

  re-render can be used after the user has changed information. The re-render allows for the page to update after the change is applied

4. What are some examples of things that we could store in state?

  If you want to change something in the application that can be saved in state. State can store what values are being updated in a form. 

### Things I want to learn more about 

What are the full capabilities of React? 