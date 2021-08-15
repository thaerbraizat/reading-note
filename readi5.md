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


### Resource
* [Node.js Design Patterns — Singleton pattern ( Series -1)](https://medium.com/@maheshkumawat_83392/node-js-design-patterns-singleton-pattern-series-1-1e0ab71e3edf).
