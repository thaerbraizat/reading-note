# APIs
![react](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1. What does REST stand for?

Representational state transfer (REST) is a software architectural style that was created to guide the design and development of the architecture for the World Wide Web. REST defines a set of constraints for how the architecture of an Internet-scale distributed hypermedia system, such as the Web, should behave.

2. REST APIs are designed around a ____.?

REST or RESTful API design (Representational State Transfer) is designed to take advantage of existing protocols. While REST can be used over nearly any protocol, it usually takes advantage of HTTP when used for Web APIs.

3. What is an identifer of a resource? Give an example.

The target of an HTTP request is called a "resource", whose nature isn't defined further; it can be a document, a photo, or anything else. Each resource is identified by a Uniform Resource Identifier (URI) used throughout HTTP for identifying resources.

4. What are the most common HTTP verbs?

The primary or most-commonly-used HTTP verbs (or methods, as they are properly called) are POST, GET, PUT, PATCH, and DELETE.

5. What should the URIs be based on?

A non-empty scheme component followed by a colon ( : ), consisting of a sequence of characters beginning with a letter and followed by any combination of letters, digits, plus ( + ), period ( . ), or hyphen ( - ).

6. Give an example of a good URI.?

example.com/articles/good-uri-design
example.com/a/good-uri-design

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?


Chatty API is one that requires consumer to make tremendous (subjective matter) amount of distinct API calls to get needed information about a resource. George Reese has defined chatty API as any API that requires consumer to do more than a single call to perform a single, common operation., bad because **poor quality**.

8. What status code does a successful GET request return?

This means the request was successful and the server created a new resource. ... This means the server successfully processed the request, but is not returning any content. Unlike a 204 response, this response requires that the requester reset the document view.

9. What status code does an unsuccessful GET request return?

Client POSTS order to server for a user resource. If user does not exist, 404 Not Found is returned. Order format and information is validated. If not valid, 400 Bad Request is returned.

10. What status code does a successful POST request return?

This means the request was successful and the server created a new resource. ... This means the server successfully processed the request, but is not returning any content. Unlike a 204 response, this response requires that the requester reset the document view.

11. What status code does a successful DELETE request return?

"If a DELETE method is successfully applied, the origin server SHOULD send a 202 (Accepted) status code if the action will likely succeed but has not yet been enacted, a 204 (No Content) status code if the action has been enacted and no further information is to be supplied, or a 200 (OK) status code if the action has

## Things I want to know more about


### Resource
* [API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design).
