# Class 9 Reading Notes

### Functional Programing Concepts

What is functional programming?

Functional programming is a programming paradim - style of building the structure and elements of computer programs that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data - wikipedia

What is a pure function and how do we know if something is a pure function?

- It returns tha same result if given the same arugments(it is also referred to as `deterministic`)

- It does not cause any observable side effects

What are the benefits of a pure function?

- The code is easier to test, unit test can be implmented

  - Given a parameter `a` -> expect the function to return value B

  - Given a parameter `c` -> expec the function to return value D

What is immutability?

  Unchanging over time or unable to be changed. Its state cannot change after it's created. For example an object that is immutable cannot be changed a new object with the new value would have to be created.

What is Referential transparency?

If a function yields the same result for the same input, it is referetially transparent

`pure functions + immutable data = referential transparency`

### Modules and require()

What is a module?

Essentially another JavaScript file that will be used to implement logic

What does the word ‘require’ do?

It is a path to the module that is being required in the file. Syntax: `require('')

How do we bring another module into the file the we are working in?

It has to be explicit in the file which part of the file you want exported to another file. `module.exports=counter;`


What do we have to do to make a module available?

We have to export the module and then `require()` it in another file and assign it to a vairable.


#### Things I want to know more about

How to use Modules in my programs