## Class 1 Reading Notes


### How the web works


#### Clients and servers

* Clients are the web user's interneted connecte devices(computers connected to wifi)

* Servers are comptuers that store webpages 

**Internet Connection:** Send and receieve data

**TCP/IP:** Transmission and Control Protocol and Internet Protocal:** how data should travel accross the internet 

**DNS:** Domain Name System, like an address book for websites.

**HTTP:** Hypertext Protocol is an application that defines a language for clients and servers to speak to each other

**Component files:** 
   
   * Code Files: JavaScript,HTML, CSS
   
   * Assets: images, music, video, word documents, and PDF's 


Relative steps of the process

* Browser goes to the DNS server, and finds address

* The browser sends an HTTP request message to the server 

* If server approves the client's request, server will send client an "OK" message. 

* Browser then assembles the webpage. 

The Order

* Browser parses HTML first

* Request then sent for CSS

* Brower generates in memory **DOM** tree from parsed HTML 

* Brower build from DOM tree and applies styles from CSSOM tree and then executes JavaScript.  


DNS created to establish readable IP addresses

**Packets:** Format is in which data is sent from the server to the client.  


### Website Planning 

* What is the website about

* What information is being presented on the subject

* What does the website look like 

#### Sketch out your design

* Wireframe

#### Choosing your assets

* Text

* Theme color 

* Images 

* Font 

**Notes:** Complex projects need detailed guidellines that go into all the details of colors, fonts spacing between items on a page, approprite writing style, and so on. This is sometimes called design guide, design system, or brand look.  

### What is JavaScript

**JavaScript adds interactivity to your website**  

#### APIs(Aplication Programming Interfaces)

* Browser Applicatiojn Programming Interfaces(APIs), users webcam, generating 3D grapics, or audio samples

* Third-party APIs allow developers to incorperate functionality in sites from other content providers, such as Twitter or Facebook

* Third-party frameworks and libraries that you can apply to HTML to accelerate work of building sites and applications 



### Variables 

>
    Declaration:

    let myVariable: 

    Assignment: 

    myVariable = "Bob";

    Calling Variable:

    myVariable;

    Changing variable
    
    let myVariable = "Bob";
    myVariable = "Steve"; 
>

#### Data Types

**String**  `let myVariable = "Bob";` Any text wrapped in single or double quotes

**Number**   `myVarible = 4` Any number

**Boolean** `let myVariable = true;`  True or False value

**Array**    `let myVariable = [1,'Bob', 'steve',10]` structure to store multple values

**Object**  `let myVariable = document.querySelector('h1');` anything is object in JavaScript

> 
    const new york = {
        borough: "Manhattan"
        buildings: 10000
        food: [bread, cheese, ham];
    }

#### Comments

>
    /* 
      Everty thing in between is a comment.
    */ 

    // This is a comment
>  
### Questions 

1. HTTP (poem)
    defines
    a language
    to speak
    between
    clients
    and 
    servers
2. The Browser parses HTML then sends a request for CSS

3. Google search and then save as to find images

4. 
    >
        let number = 4
        let string = '4'

    >
5. Variables in JavaScript are used to store data 

>
     let
     const
> 

### Getting Started with HTML

>
    <p>paragraph<p>

    <em>italic</em> 
     
     <stromg>stronger text formatting</strong>

> 


**Nesting:** Placing elements inside of other elements.

>
     <p>My cat is <strong>very</strong>grumpy,</p>



**Block Elements:** Paragraphs, headings, lists, navigation menus

**Inline Elements:** `<em> <strong> <a>` 


**Note:** Inline and Block don't reference CSS block and inline, in CSS the category of the elements do not change nor their containment 

**Void Elements:**

`<img>` 

no requirement to add `/` at the end of void elements  

#### Atributes 

Elements can also have attributes(extra information about the element) 

> 
    <a> anchor can take the following attributes

    <href> Value sepecifies web address for link
    
    <title> information about the link

    <target> specifies browsing cntext to display the link `target="_blank"` will display link in a new tab. 

>


`<p>A link to my <a href="https://www.mozilla.org/" title="the Mozilla homepage" target="_blank">favorite website</a>.<p>` 

#### Boolean attributes

Attributes with out wrriten values 

>
    <!-- using ther disabled attribute prevents the end user from entering text into the input box --> 

    <input type="text" disabled /> 

    <!-- text input is allowed, as it doesn't contain the disabled attribute --> 
    <input type= "text"> 

#### Anatomy of an HTML document

 >
    <!DOCTYPE html>
    <html leng="en-US"> 
    <head>
        <meta charset="utf-8"/>
        <title> My test page</title>
    </head> 
    <body>
         <p>This is my page</p>
    </body>
    <html>
1. `<!DOCTYPE html>` Set of rules the document has to follow
2. `<html></html>` Wraps all of the pages content
3. `<head></head>` Container for everything the page includes
4. `<meta charset="utf-8">` This element represents meta data that cannot be represented by other HTML, `<base>, <link>,<script>,<style>,<title>,` `charset` attribute sets the characer for the document to UTF-8, inlcudes characters from majority of written languages 
5. `<title></title>` `title` element sets the title of the page. 
6. `<body></body>` This contains all the conent that displays on the page.

`<,>,",'`

>
    Literal Character           Character reference equivalent
    <                           &lt;
    >                           &gt;
    "                           &quot;
    '                           &apos;
    &                           &amp; 

> 

Header: Logo or tagline

Navigation Bar: links or tabs

Main content: cetner of the unique content

sidebar: links, info, quotes, ads

footer: strip accross the bottom

* header: `<header>`

* navigation bar: `<nav>`

* main content: `<main>` `<article>` `<section>`

* sidebar: `<aside>`; often placed inside `main`

* footer: `footer` 

* `<main>` is for conent unique to the page. User `<main>` only once per page, and put it directly inside the `<body>`

* `<article>` encloses a block of related content that makes sense on its own without the rest of the page

* `<section>` grouping together parts of a page that represent a single set of funcitonality(typyically have different headings)

* `<aside>` contains content not directly related to the main content

* `<header>` represents a group of introductory content 

* `<nav>` contrains main navigation for the pages funcitonality (links)

* `<footer>` represents a group of end content for a page

**Non semantics**

3.Grouping items together that do not have an ideal semantic elemant 

`<span>` Inline non semantic

`<div>` Block semantic

#### Line Breaks and horizontal rules

`<br>`: the link break element(fixed short lines)

`<hr`>: Denotes thematic change to the text such as a topic or scene

#### metadata 

**Not displayed on the page**

_Can use meta to add author and description_

>
    <meta name="author" content="Chris Mills"/>
>

#### Adding CSS and JavaScript

`<link>` should go inside `<head>`

>
    <link> rel="stylesheet" href="styles.css"/> 
>

`<script>` should also go inside the head

>
    <script src="js-file.js" defer></script>

    `defer`: load JS after html is parsed
>

#### Questions

1. Attributes are additional information about the element
2. The anatomy of an html element begins with opening tags, has content in the middle, then closing tags.
3. `<article>` is tpycally used for information not relative to the page `<section>` typycally based on functionality
4. `<head>``<title>``<header>``<footer>` `<body>` 
5. meta keywords can boost pages SEO
6. typycally for descriptions 

#### What is JavaScript

High level programming language that makes web pages dynamic

**APIS continued**

**Browser APIS**
* DOM(Document object model API) allows you to manipulate HTML and CSS, creating and changing HTML, and dynamically applying new styles to the page

* Geolocation API(retreieves geographical information)

* Canvas and WebGL APIS allow 2D and 3D graphics

* Audio and video APIS allow multipmedia

**Third Party APIs**

* Twitter API

* Google Maps API

**Event Listeners** Initiates event once process has occured

`async` and `defer` both instruct the browser to download the script(s) in a separate thread, while the rest of the page(DOM), is downloading so the page that is loading is not blocked during the fetch process


#### Miscellaneous 

 What is the first step to designing a Website?

* Project Ideation(What is looking to be accomplished 

What is the most important question to answer when designing a Website?

* What/How do I accomplish my goals with a website

Why should you use an `<h1>` element over a `<span>` element to display a top level heading? 

* `<h1>` signifies that the content displayed is an important element that is acting as a header and has benefits such as improved searching capacity.

What are the benefits of using semantic tags in our HTML?

* sementics act as important keywords and can improve SEO. They can also help with page navigation. 

Describe 2 things that require JavaScript in the Browser?
* To implement features that come from an API

* Adhere to `events` that you want to run on your page

How can you add JavaScript to an HTML document?

* Inline using `<script>` or externally with a separate JavaScript file. 

### Things I would like to know more about

What is a good ratio between non semantic elements and semantic elements

