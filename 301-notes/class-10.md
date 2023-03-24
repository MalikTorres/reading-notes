### Class 10 Notes

### Understanding the JavaScript

What is a ‘call’?

A call is the invocation of a function

How many ‘calls’ can happen at once?

`calls` happen one at a time top to bottom

What does LIFO mean?

'Last In First Out' the last function gets pushed into the stack and is the first to be popped out when the funtion returns.

Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

![Callstack](reading-notes/301-notes/CallStack.png)

What causes a Stack Overflow?

This occurs when there is a recursive function(a functiont that calls itself) without an exit point.Browsers have a maximum stack call that it can accomodate before throwing a stack error.

### JavaScript error messages

What is a ‘reference error’?

Using a variable that is not yet declared, best practice is declaring the variable before any declaration is made.

What is a ‘syntax error’?

When the something cannot be parsed because of syntax, and example would be a trailing comma.


What is a ‘range error’?

Trying to manipulate invalid length.

What is a ‘type error’?

when type of numbers,strings, etc are incompatible accessing a property in an undefined type of variable.

What is a breakpoint?

It's the point until you want your code to run when debugging

What does the word ‘debugger’ do in your code

You can create the break point by putting the word 'debugger' in your code.


### Things I want to know more about

How to be better at debugging code.