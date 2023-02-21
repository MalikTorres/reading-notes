## Class 12 Reading Notes


### JavaScript Canvas

1. What does the <canvas> allow a developer to acheive?

  Canvas allows you to draw 2D graphics in JavaScript

2. What is the importance of the closing `</canvas> tag?

   The closing tag is required as it will allow fallback content to be displayed if the browser does not support canvas, althought most browsers now do.


3. Explain what the getContext() method does.

  The `getContext()` method returns a rendered context object. The `getContext()` method takes on arguement which is the type of context. For example `"2d"` to get a 2D rendering context object, which is an instance of the `ConvasRenderingContext2D` interface.

  The 2D rendering context allows you to draw shapes,text,images, and other objects.

  **Important to check if the browser supports the `getContext()` method**

### Chart.js Documentation

1. What is Chart.js and how it can be brought into your project?

    Chart.js provides a set of frequently used chart types, plugins, and custimization options. In addition to a set of built in chart types.

2. List 3 different Chart types you can create using Chart.js.  

    * bar-funnel
    * boxplot
    * error-bars


### Easily Create Stunning Animated Charts with Chart.js

1. What are some advantages to displaying data via a chart over a table?

    They convey data quicker than tables and are easier to look at. 


2. How could Chart.js aid your previously created applications visually? 

    The cookie stand lab and odd duck lab could have benefitted from a chart display that reflected all of the total data.

### Things I want to know more about

  How to use the ChartJs library.

### References 

[ChartJs Documentation](https://www.chartjs.org/docs/latest/)