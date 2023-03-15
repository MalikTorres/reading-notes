## Class 03 Reading Notes

#### Lists and Keys

1. What does .map() return?

      It returns a new array

2. If I want to loop through an array and display each value in JSX, how do I do that in React?

      You can use the `.map()`  method

3. Each list item needs a unique ____.

  Each key needs a unique string identifies that item.

4. What is the purpose of a key?

#### The Spread Operator

1. What is the spread operator?
    
    Spreads an iterable object into a list of arguments

    `...` 

2. List 4 things that the spread operator can do.

   The spread operator, concatenating or combing arrays, Using Math functions, using an array as arguments, Adding an item to a list, Adding to state in React, Combing objects, and converting NodeList to an array. 

3. Give an example of using the spread operator to combine two arrays.

      >
        const myArray = [`🤪`,`🐻`,`🎌`]
        const yourArray = [`🙂`,`🤗`,`🤩`]
        const ourArray = [...myArray,...yourArray]
        console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩
      >


4. Give an example of using the spread operator to add a new item to an array.

      >
        const myArray = [`🤪`,`🐻`,`🎌`]
        const yourArray = [`🙂`,`🤗`,`🤩`]
        const ourArray = [...myArray,...yourArray]
        console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩
      >



5. Give an example of using the spread operator to combine two objects into one.

      >
          const objectOne = {hello: "🤪"}
          const objectTwo = {world: "🐻"}
          const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
        console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
        onst objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
          objectFour.laugh() // 😂😂😂😂😂
      > 
      
#### How to Pass Functions Between Components

1. In the video, what is the first step that the developer does to pass functions between components?

    The first step would be to create a function which will handle the changed state.

2. In your own words, what does the increment function do?

    The increment function allows the state to be updated so that when the button is clicked it will reflect the update. 

3. How can you pass a method from a parent component into a child component?

    A function that has the parent component the pass this function to child component render. 

4. How does the child component invoke a method that was passed to it from a parent component? 

    You can access it with methods like `onClick`