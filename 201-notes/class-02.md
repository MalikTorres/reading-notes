### Class 02 Reading Notes

### Introduction to HTML Continued

##### Questions

Why is it important to use semantic elements in our HTML?

Semantic elements help give our content the correct meaning. For example `<h1>` tells the browser that there is a heading.

How many levels of headings are there in HTML?

There are six headings levels in HTML, `<h1>, <h2>,<h3>,<h4>,<h5>,<h6>`. Best practice is to use no more than three headings per page.

What are some uses for the `<sup>` and `<sub>` elements?
Subscript and  Super script are used for marking up items like dates and math questions.

`<p> If x<sup>2</sup> is 9, x must equat 3 or -3.</p>`

When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term?
This provides a hint to user agents on how to announce/display the contentw hile informing all users what the abbreviation means.

>
    <p>
      We use <abbr>HTML</abbr>,Hypertext Markup Language, to structure our web documents.
    </p> 
>

### How CSS is Structured

#### Questions

What are ways we can apply CSS to our HTML?
External stylesheets, Internal, and Inline.

External: `<link>` in header,
Internal: `<style>` in code
Inline: `<style>` in line

Why should we avoid using inline styles?
It is an ineffient way to maintain CSS with multiple edits being required for a single page. It also impacts the readabilty of your HTML

Review the block of code below and answer the following questions:

What is representing the selector?
`<h2>` is the CSS selector

Which components are the CSS declarations?
`color: black;` is the declaration.

Which components are considered properties?
`padding: 5px` is a considered a property.

### JavaScript Basics

#### Questions

What data type is a sequence of text enclosed in single quote marks?
This data type is a string. `""`, `''`

List 4 types of JavaScript operators.
`+`: Adds two numeric operands

`-`: Subtract right operand from left operand

`*`: Multiply two numeric operands

`%`: Modulus operator. Returns remainder of two operands

Describe a real world Problem you could solve with a Function.
A function could be created that would automate tipping so customers knew the percentage they should tip. 


### Making Decisions In Your Code - Conditionals

The ternary operator
`condition ? run this code : run this code instead`


### Questions

An if statement checks a __ and if it evaluates to ___, then the code block will execute.

An if statement checks a `condition` and it evaluates to true, then the code will execute.

What is the use of an else if?
`else if` allows us to add additional choices and outcomes.

List 3 different types of comparison operators.

`>=` The greater than or equal to operator

strict equal operator 
`===` Returns true if the operands are equal and of the same type

Strict not equal
`!==` returns true if the operands are not of the same type but not equal, or are of different type


What is the difference between the logical operator && and ||?

`&&` is AND 
`||` is OR

#### Things I would like to know more about 

What are cases for not using a strict not equal operator?

#### References

[HTML Advanced Text Formatting](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting)
[How CSS is Structured](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured)
[Making Decisions in Your Code](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)
