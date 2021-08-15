# Authentication

![API](https://nordicapis.com/wp-content/uploads/Building-a-RESTful-API-Using-Node.JS-and-MongoDB.png)

1. Explain what a “Singleton” is (in Computer Science terms)?

A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. ... The singleton pattern is used in programming languages

2. Explain how the Singleton pattern can be used with Node modules, specifically with classes?


 let’s go ahead and modify this file to export a singleton instead of a logger. So on line 17 I’m just going to come in here and add a new class called singleton. So this class is only going to allow us to create one instance of the logger. Anytime we need that instance we’re going to retrieve it through a get instance method.
So let’s go ahead and add a constructor to our singleton class. And what we want to do within this constructor is we want to check and see if an instance has already been created. So I’m going to save the instance directly to the class. So if there’s not a singleton instance then we want to create one. So if we don’t have one then the singleton instance will equal new logger. So that’s our singleton. And it will only allow us to create one instance whenever we instantiate this singleton class.



3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.

Middleware functions can perform the following tasks:

* Execute any code.
* Make changes to the request and the response objects.
* End the request-response cycle.
* Call the next middleware function in the stack.
* If the current middleware function does not end the request-response cycle, it must call next() to pass control to the next middleware function. Otherwise, the request will be left hanging.


### Securing Passwords 
Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.
We all know storing passwords in clear text in your database is ridiculous. Many desktop applications and almost every web service including, blogs, forums eventually need to store a collection of user data and the passwords, that has to be stored using a hashing algorithm.

### Basic access authentication
In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.

### OWASP auth cheatsheet
Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

Session Management is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction. Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests. Sessions should be unique per user and computationally very difficult to predict. The Session Management Cheat Sheet contains further guidance on the best practices in this area.




### Resource
* [Node.js Design Patterns — Singleton pattern ( Series -1)](https://medium.com/@maheshkumawat_83392/node-js-design-patterns-singleton-pattern-series-1-1e0ab71e3edf).
