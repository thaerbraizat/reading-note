#  Data Modeling

![API](https://nordicapis.com/wp-content/uploads/Building-a-RESTful-API-Using-Node.JS-and-MongoDB.png)

1. Name 3 advantages to Test Driven Development?
* You receive fast feedback. 
* TDD creates a detailed specification.
* TDD reduces time spent on rework.

2. In what case would you need to use beforeEach() or afterEach() in a test suite?

beforeEach and afterEach can handle asynchronous code in the same ways that tests can handle asynchronous code - they can either take a done parameter or return a promise.

3. What is one downside of Test Driven Development?

the strongest argument against TDD is that the tests need to be maintained because the code has got to. Whenever requirements change, you would like to vary the code and tests.So, actually, this disadvantage is that the same as before when writing code that apparently takes an extended time.

4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?

ES6 class constructors	
This can be said to be a syntax base for constructor functions and instantiate objects using a new operator.
ES5 function constructors
This also uses a new operator for object creation but focuses on how the objects are being instantiated.

5. Why REST?

**REST** aims to make caching easier. Since the server is stateless and each request can be processed individually, GET requests should usually return the same response regardless of previous ones and the session. This makes the GET requests easily cacheable and browsers usually treat them as such.


### Resource
* [REST](https://www.serviceobjects.com/articles-whitepapers/why-rest-popular/).