# CRUD
![react](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1. In your own words, describe what each group of status code represents:
* 100’s = The HTTP 100 Continue informational status response code indicates that everything so far is OK and that the client should continue with the request or ignore it if it is already finished.

* 200’s = 200 implies that the response contains a payload that represents the status of the requested resource. An error message usually is not a representation of that resource. If something goes wrong while processing GET.

* 300’s = 300 Multiple Choices redirect status response code indicates that the request has more than one possible responses. The user-agent or the user should choose one of them. As there is no standardized way of choosing one of the responses, this response code is very rarely used.

* 400’s =  Bad Request response status code indicates that the server cannot or will not process the request due to something that is perceived to be a client error.

* 500’s = The 500 Internal Server Error is a very general HTTP status code that means something has gone wrong on the web site's server but the server could not be more specific on what the exact problem is.

2. What is a status code 202?

The 202 response is intentionally non-committal. Its purpose is to allow a server to accept a request for some other process (perhaps a batch-oriented process that is only run once per day) without requiring that the user agent's connection to the server persist until the process is completed.

3. What is a status code 308?

308 Permanent Redirect redirect status response code indicates that the resource requested has been definitively moved to the URL given by the Location headers.
 

4. What is the ‘Forbidden’ status code?

403 Forbidden client error status response code indicates that the server understood the request but refuses to authorize it.The access is permanently forbidden and tied to the application logic, such as insufficient rights to a resource.




## Build A REST API With Node.js, Express, & MongoDB .

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

 for storing sensitive data (not to be pushed)

2. What is middleware?

system with functions that have access to the request object (req), the response object (res), and the next function in the application’s request-response cycle. The next function is a function in the Express router which, when invoked, executes the middleware succeeding the current middleware.

3. What does app.use(express.json()) do? 

allow us to use express methods.

4. What does the /:id mean in a route?

id is the unique instance field (_id) that is given to each Mongoose model instance by default.

5. What is the difference between PUT and PATCH?

PUT = create , PATCH = update

6. How do you make a default value in a schema? 

by creating a new document without that path set, the default will kick in.

7. What does a 500 error status code mean? 

500 Internal Server Error

8. What is the difference between a status 200 and a status 201?

200 =  accessible  resource, 201 = create operations


References:

* [status codes](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

* [Video](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)