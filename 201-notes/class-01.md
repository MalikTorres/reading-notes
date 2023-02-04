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