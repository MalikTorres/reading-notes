## Class 3 Notes

### Review: ES6 Classes

Classes are a template for creating ____.

Classes are a template for creating objects. They encapsualate(essential features) data with code to work on that data. 

Can a class declaration be hoisted?

Class declarations may be able to be anonymous similar to function expressions but they have restrictions similar to `let` and `const`, therefore they cannot be hoisted.

How would you describe a constructor and contextual “this” to a non-technical friend?

Constructor's essentially allow the developer to save time by creating properties and key values that can be used accessed in the future. They then can use the keyword `this` to access those key values that were stored.

### Using Express Routing

Within Express, what does routing refer to?

How an application's endpoints (URI's) respond to client request. HTTP Methods can be defined as `app.get(),` `app.use()` etc.

What is the difference between a route path and a route method?

Route methods are derived from one of the HTTP methods, and attached to an instance of the express class. Route paths in combination with request methods, defined the endpoints at whcih requests can be made.

When is it appropriate to add next as a parameter to a route handler and what must 
you do if next has been passed to your middleware as a parameter?

When there are multiple callback functions

Express Routing

What is an Express Router?

It provides access to routing APIs like, `.use`,`.get`, `param`, and `route`

By what mean do we initialize express.Router() in an express server?

We assign and store `express.Router()` to a variable.

What do we use route middleware for?

Middleware allows action to be take before the request is processed. Such as user authentification, logging data for analytics, or  anything else.

Reflection

What are your learning goals after reading and reviewing the class README?

I would like to be more patient with my learning and not be so hard on myself throughout this process if I do not understand something right away.


#### Things I want to know more about

How to use `express.router`