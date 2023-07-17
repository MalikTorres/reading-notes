# Class 43 Reading Notes

### getting started with react native

Name three Core Components of React Native and describe what they do.

View: A fundamental component used for creating UI elements, similar to `<div>` in web development.

Text: Used for displaying text content on the screen, similar to `<p>` or `<span>` in web development.

Image: Used for displaying images, allowing you to load and render different types of ima

What problem does React Native solve (why call it native)?

React Native allows developers to build mobile applications using JavaScript and React, while still providing a native-like user experience. 

What are the building blocks of a React Native app? How does that compare to a React app?

The building blocks of a React Native app are components, which are reusable UI elements responsible for rendering a part of the user interface. 

expo

What solution does expo provide?


Expo is a platform that provides a set of tools, services, and libraries to simplify React Native app development. It offers features like an integrated development environment (IDE), device testing, over-the-air updates, and access to device APIs. Expo aims to streamline the development process and make it easier for developers to build and deploy React Native apps.

Expo tries to manage as much of the complexity of building apps as possible,

Expo is often referred to as the "managed" workflow because it handles many aspects of app development, such as building, bundling, and managing dependencies, without requiring developers to deal with lower-level configuration.

which is why we call it the ____ workflow.

Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the managed workflow.

What is the difference between React Native and Expo?
expo snack

Expo Snack is an online tool that allows you to quickly prototype and test React Native code in a web browser without the need for local development setup. It provides a code editor, simulator, and the ability to share the code with others, making it convenient for experimenting with React Native code snippets.

Checkout this tool. What does snack allow you to do?

ejecting

What does “eject” mean within the context of Expo?

"Ejecting" in the context of Expo means transferring the control of your Expo project from the managed workflow to the bare workflow. It allows you to have more control over the project configuration and access to lower-level dependencies and native code.

When should you not eject?

You should avoid ejecting from Expo if you prefer the convenience and ease of use provided by the managed workflow. If your app does not require extensive customization or specific native modules, sticking with the managed workflow can save development time and effort.

Why might you choose to eject?

You might choose to eject from Expo if you need to add custom native code, use specific native modules that are not available in the managed workflow, or require more control over the project configuration. Ejecting allows you to integrate custom native code and libraries, giving you greater flexibility and access to the full power of native development capabilities.

### Things I want to know more about

How to work with react native