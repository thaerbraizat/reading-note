# Express REST API
![API](https://nordicapis.com/wp-content/uploads/Building-a-RESTful-API-Using-Node.JS-and-MongoDB.png)


1. Name 3 real world use cases where you’d want to change the request with custom middleware?
authorization , checking the user input , handle errors 

2. True or false: The route handler is middleware?
**False**

3. In what ways can a middleware function end the process and send data to the browser?

when we pass it into end point and make it check things if true go next else send data with go 
to the next but we need and return after next end the process.

4. At what point in the request lifecycle can you “inject” middleware?
 after the request

5. What can cause express to error with “Request headers sent twice, cannot start a second response?

The error "Error: Can't set headers after they are sent." means that you're already in the Body or Finished state, but some function tried to set a header or statusCode. When you see this error, try to look for anything that tries to send a header after some of the body has already been written. For example, look for callbacks that are accidentally called twice, or any error that happens after the body is sent.


### Resource
* [stackoverflow](https://stackoverflow.com/questions/58925276/what-is-the-difference-between-a-route-handler-and-middleware-function-in-expres).
* [stackoverflow](https://stackoverflow.com/questions/7042340/error-cant-set-headers-after-they-are-sent-to-the-client?rq=1).