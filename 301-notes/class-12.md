#### In your own words, describe what each group of status code represents:

100’s = Informational status codes, informs the client that the header part of the request has been received 

200’s = Success codes. Informt he client that it request was accepted

300’s = These are redirection clodes. Inform the client that resource they are requesting isn't avaliable 

400’s = Client error codes. invalid request a client sent to a server.


500’s = These server error codes. Inidicate problems with overwelmed servers and unreachable servers.


What is a status code 202?

Accepted, if the update is asynchronous, this code can be used. It should include the RL to access the updated resource or an URL to check if update has been succeeded.

What is a status code 308?

Permananent Redirect, this is right code if the resource will now be avaliable at the new URL 



What code would you use if an update didn’t return data to a client?

The code to use iss 307.


What code would you use if a resource used to exist but no longer does? 


a code 308

What is the ‘Forbidden’ status code? 

403 is `forbidden`

#### Build A REST API With Node.js Express & MongoDB


Why do we need to pull our MongoDB database string out of our server and put it into our .env?

To sync our database to our server.



What is middleware?

A request handler with access to the applications request-response cycle.

What does app.use(express.json()) do?

Allows our server to accept JSON

What does the /:id mean in a route?

The path that allows you to get to the function.

What is the difference between PUT and PATCH?

`PUT` alters resources `PATCH` is a technique for transferring the resources

How do you make a default value in a schema?

You can set the value to a function

What does a 500 error status code mean?

This means interal server error

What is the difference between a status 200 and a status 201?

200 means everything is functioning correctly and 201 means the server completed it's browser request


#### Things I want to know more about


How to use MongoDB

