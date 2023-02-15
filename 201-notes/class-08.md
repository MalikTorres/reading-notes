## Class 8 Reading 

### Flexbox

1. Flexbox is designed for one-dimensional content. Explain what this means.

  It takes in a combination of different items of different sizes and returns the best layout for those items.  It allows for flexible boundaries.

2. Explain the difference between the main axis and cross axis.

    main axis is set by the `flex-direction` property. If that is `row` your main axis along the row, if that is `column` your main axis is along the column. Flex items move as a group along the main axis. The cross axis runs in the other direction to the main axis, so if `flex-direction` is `row` the cross axis runs along the column.

3. How can using certain properties of flexbox negatively impact accessibility?

    Using properties that reverse the order of row and column can impact keyboard navigation as it follows DOM not visual display. Important to use to caution when changing properties that reorder the visual display of how things are ordered in the HTML document.  


### Layout

1. What are some advantages of using flexbox over float?

    Flexbox allows for items to be vertically centered, make all of the children of the container take up an equal amount of the avaliable width/height, regardless of how much width/height is avaliable. Lastly, make all the columns in a multple-column layout and adopt the same height even if they contain a different amount of content.


2. How does this topic connect with your long term goals? 

     Flexbox will allow me to structre websites more effiently and build out professional wireframes. 


  ### Things I want to learn more about

  How to effitively use flexbox. 

  Referemces:

  * [Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)