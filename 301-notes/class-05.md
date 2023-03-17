### Class 05


#### Thinking In React


1. What is the `single responsibility principle` and how does it apply to components?

    This is a component that should ideally only do one thing only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

2. What does it mean to build a ‘static’ version of your application?

    The static version of an app renders the data model, these models reuse other components and data using props. State should not be used when using a static version.

3. Once you have a static application, what do you need to add?

    You'll need to add state, as state is the data that will be changing.

4. What are the three questions you can ask to determine if something is state?

      * Does it remain unchanged over time? If so, it isn't state.
      * Is it passed in from a parent via props? If so, it isn't state.
      * Can you compute based on existing state or props in your component? 

5. How can you identify where state needs to live?

      * Identify every component that renders something based on that state.
      * Find their closest common parent component - a component above them all in the hierarchy
      * Decided where the state should live

  **State can live:**
  
  1. directly into parent common parent
  2. You can also put the state into some component
  3. If you can't find a component where it make sense to own the state, create a new component soley for holding the state and add it somewhere in the hierarchy above the common parent component.


#### Higher-Order Functions 


1. What is a “higher-order function”?

  Functions that operate on other functions, either by taking them as arguements or by returning them, are called higher-order-functions. 

2. Explore the greaterThan function as defined in the reading. In your own words,

  Greater than functions essentially allow  abstration over actions not just values. 

3. what is line 2 of this function doing?

  I believe it's creating another function. 

4. Explain how either map or reduce operates, with regards to higher-order functions. 
 
    The way the map method operates is that content is mapped to a new form by the function.

#### Things I want to know more about

How high order functions are used.