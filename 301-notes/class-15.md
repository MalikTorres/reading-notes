# Class 15 Notes

#### OAuth

What is OAuth?

OAuth allows websites and services to share assests among users. It is widley accepted, but has vulnarbilties.

Give an example of what using OAuth would look like.

An example of OAuth is when you log onto a website an it provides the user more than one opportunity to log into a website.

How does OAuth work? What are the steps that it takes to authenticate the user?

* The first website connects to the second website on behalf of the user

* The second site generates a one-time toke and a one time secrete unique to the transaction o the parties involved.

* The client's software presents the request token and secret to their authroization provider

* If not authencated the client will be asked to reauthenticate themselves.

** These are just some of the steps***

What is OpenID?

OpenID works as a singl sign in 


#### Authorization flows

What is the difference between authorization and authentication?

Auth0 uses the OpenID Connect (OIDC) Protocol and OAuth2.0 framework to authenticate users.

What is Authorization Code Flow?

It is the exhange of an Authorization Code for a token

What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

A migitgation for the challenges faced when using Auth0 on single page applications

What is Implicit Flow with Form Post?

Intended for public clients to store sensitive information

What is Client Credentials Flow?

This sysmte authorizes the app rather than the user.

What is Device Authorization Flow?

This device ask the user to go to a link on their computer or smart phon and authroize the device

What is Resource Owner Password Flow?

Typycally an interactive platform that ask the user to provide a username and password.


#### Things I want know more about

How to apply these flow to applications