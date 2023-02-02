## Reading 7 

### JavaScript Expressions and Opertors  

***Control Flow is the order in which code executes**

Code is typycally run from the first line in a file to the last. _Coditionals and Loops change control flows_ 

**Control Structures:** Include **conditionals**, **loops**, and **functions**. Part of the script may be set to execute when **events** occur. 

### Example of control flow

> 
    if (else field)) {
        promptUser()
    } else {
        submitForm();

    } 
>   

**Control flow means that when you read a script, you must not only read from start to finish but also look at program structure and how it affects order of execution**

### JavaScript Functions 

A JavaScript function is a block of code designed to perfrm a particular task. A function is exectued when "something" invokes it also knoned as calling the funciton. 

**Function Example Below**


>
    // Function to comput the product of P1 and P2 
    function myFunction(p1, p2) {
        return p1 * p2; 
    } 
> 

**JavaScript Function Syntax** 

A JavaScript function is defined with the `function` keyword, followed by the **name** of the function, followed by parenthesis `()`

Functions can contain letters, digits, underscores, and dollar signs(_same rules as variables_)

The parenthesis can include parameter names separated by commas: `(parameter1, parameter2,...)` 

> 
    function name(parameter1, paramter2, paramter3) {
        // code to be executed
    } 
> 

Function **paramteres** are listed inside the paranthesis `()` in the function definition 

Function **arguements** are the **values** received by the function when it is invoked.

Inside the function, the arguements (the paramters) behave as local variables. 

### Function Invocation 

The code inside the function will execute when "something" **invokes**(calls) the function: 

* When an event occurs(when a user clicks a button)

* When it is invoked (called) from the JavaScript code

* Automatically (self invoked)

### Function Return

When JavaScript reaches a `return` statement, the fucntion will stop executing.

If the function was invoked from a statement, JavaScript will "return" to execute the code after invoking the statement. 

Functions often compute a **return value**. The return value is "returned" back to the "caller": 

>
    let x = myFunction (4,3);  // Function is called, return value will end up in x

    function myFunction(a, b) {
        return a * b;           // Function returns the product of a and b
    }

    return in x will b: 12
>

### Why Functions?

You can reuse code: Define the code once, and use it many times.

You can use the same code many times with different arugements, to produce differen results.

>
    function toCelcius(fahrenheit) {
        return (5/9) * (fahrenheit -32);
    }

    // Calling the function 

    document.getElementbyId("demo").innerHTML = toCElsius;

> 

### The `()` Operator Invokes the Function

Using the example above, `toCelsious` refers to the function object, and `toCelsious()` referes to the function result.

Acessing a function without () will return the function **object** instead of the function **result** 

>
    function toCelsius(fahrenheit) {
        return (5/9)  * (fahrenheit-32);
    } 

    document.getElementById("demo").innerHTML = toCelsius;

> 

### Functions Used as Variable Values

Functions can be used the same way as you use variables, in all types of formulas, assignments, and caluclations. 

_Instead of using a variable to store the return value of a function:_ 

>
    let x = toCelsius(77);
    let text = "The temperature is " + x + 

    let text = "The temperature is " + toCelsius(77) + " Celsius";

> 

### Local Variables 

Variables declared within JavaScript function, become **LOCAL** to the function.

Local variables can only be accessed from within the function

>
    // code here can Not user carName 

    function myFunction() {
        let carName = "Volvo"
        // code her CAN use carName
    }

    // code here can NOT user carName

>  

### Operators

The **Assignment Operator (=)** assigns a value to a variable

> 
    let x = 10;

    // Assign the value 5 to x
    let x = 51
    // Assign the value 2 to y 
    let = 2;
    // Assign the value x + y to z;
>

The **Additional Operator (+) adds numbers:

_Can also be used to concatenate strings_
**Adding two numbers, will return the sum, but adding a number and a string will return a string:**
>
    let x = 5;
    let y = 2;
    let z = x + y;

> 
The Multilication Operator (*) multiplies numbers:

> 

    let x = 5;
    let y = 2;
    let z = x * y; 

> 

Since local variables are only recognized inside their functions, variables with the same name can be used in different functions

Local variables are created when a function starts, and deleted when function is complete. 

* Assignment Operators

* Comparason Operators 

* Arithmic Operators

**Arithmetic Operators are used to perform arithmetic on numbers:**

>
    let a = 3;
    let x = (100 + 50) * a; 

> 

* Bitwise Operators 

* String Operators 

* Comma Operators 

* Relational Operators

* Addition Assignment Operator (+=) adds a value to a variable
_Can also be used to concatenate strings_
>
    let x = 10;
    x += 5;
> 



_These are only some of the JavaScript operators there are many more_ 

**precedence** operators determine the order in which they are applied

operators like `!` and `typeof` are prefix opertors 

### JavaScript Type Operators

`||`: OR

`&&`; AND

`!` ; NOT


> 
    +               Addition
    -               Subtraction
    *               Multiplication
    **              Exponential
    /               Division
    %               Modulus(Division Remainder)
    ++              Increment
    --              Decrement
>  

### JavaScript Comparison Operators

>

    ==              equal to
    ===             equal value and equal type
    !=              not equal
    !==             not equal value or not equal type
    >               greater than
    <               less than
    >=              less than or equal to
    ?           

>  

### JavaScript Type Operators

>

    typeof              Returns the type of a variable
    instanceof          Returns true if an object is an instance of an object

>

JavaScript Bitwise Operators
Bit operators work on 32 bits numbers.

Any numeric operand in the operation is converted into a 32 bit number. The result is converted back to a JavaScript number

Operator  Description  Example   Same as         Result    Decimal
>
    &       AND         5 & 1     0101 & 0001      0001       1 
  