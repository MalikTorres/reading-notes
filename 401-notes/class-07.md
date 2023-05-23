# Class 7

#### Intro to JWT

What is a JSON Web Token (JWT)?

JWT's define a compact and self-contained way for securely transmitting information between parties as a JSON object. The information an verified and trusted because it is digitally signed

When should we use JSON Web Tokens?

- Authorization
- Infromation Exchange

Claims are expected in which structural component of a JWT?

The payload, calims are statement about the entity.

#### Are JWTs Secure?

If I get a JWT and I can decode the payload, how can we call that secure?

They are as the signatured can be changed

If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.

They need to know both the secret and the key

Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

Essentitally this information is transmitted through an algorithmic function


#### JWTs Explained

Why use JWT?

Enables you to securley transfer information

JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

It can be sent in multiple ways quickly and contains information about the user

What are the three components (the structure) of a JWT signature? 

The header and payload

Reflection

What are your learning goals after reading and reviewing the class README?

How to implement JWR


### Things I want to know more about

Building basic auth