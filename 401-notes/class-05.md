## Class 5 Notes

### Securing Passwords

Explain to a non-technical friend how you would safely hash and store a password.

There are general purpose hash functions that can take in and process large amounts of data in a short time frame. This ensures that if there is an attempt to steal passwords, what's taken is the hash.

What is Bcrypt?

It is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor(this is also known as a security factor)

Why might you use something like Bcrypt?

This can slow down brute force attacks on databases as the the time span of the hash values being generated varies.

### Basic Auth

What is Basic Authentication?

It is a method for an HTTP user agent(also known as  web browser) to provide a user name and password when making a request.


What properties are necessary in the header of a Basic Auth request?

`Aithorization: Basic <credentials>`,  

How are username:password in Basic Auth encoded?

In Base64, which represents a group of binary-to-text encoding schemes that represent binary data.

### OWASP auth cheatsheet

Define the authentication process to a non-technical recruiter.

Essentially this is the process of verifying an individual is who they claim to be, such as when you enter your username and password to access a site.

How should your error messaging respond (both HTTP and HTML)? Why?


There should be a generic response for the user, and a more detailed response on the server side. 

Looking ahead at this module’s course schedule, What do you look forward to learning?

I'm interested in learning more about authentification

What are your learning goals after reading and reviewing the class README?

Become a better problem solver

### Things I want to know more about

Implementing authentication into middleware