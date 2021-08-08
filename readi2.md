# Express

1. What’s the difference between PUT and PATCH?

The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.

2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server?

* Nock
* MockServer
* Beeceptor

3. Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

While developing node services, we might need to expose our Api documents based on requirement. In that case we think of picking right documentation tool because there are many 3rd parties tools available for it. I have created sample POC by using 2 popular documentation tools
 1. Swagger and
 2. Apidocjs

Here is my finding regarding both:

* **Popularity**: By comparing stats,  swagger-ui is more popular then apidocjs.
* **Consistency**: If we already using swagger for our Dotnetcore service, then implementing swagger tool will consist more from Info and UI prospective.
* **Implementation complexity**: apidocjs and swagger both required documentation content on implemented method as customize comment data. In addition they allow to write documentation data in separate resource file as .js and .json. If we already have swagger.json created by DotnetCore we can reuse more than 80% specification.
* **Maintenance**: For apidocjs will have to modify documentation for each affected method/endpoints if service changed. In swagger we can limit changes. But by implementing apidocjs we can isolate the layer.
* **Other benefits**: Because swagger use plain .json that could be parsed through programing language, thus we can get advantage of various other 3rd parties in order to create http client and more. 
* **Future**: Due to popularity of swagger, apidocjs provide information about apidoc-swagger converter so we can switch apidoc to swagger anytime.

4. Compare and contrast SOAP and ReST?

![Compare and contrast SOAP and ReST](https://i.stack.imgur.com/DFII3.png)


### Resource
* [SOAP and ReST](https://stackoverflow.com/questions/2131965/main-differences-between-soap-and-restful-web-services-in-java).
* [apidoc vs swagger for node app](https://www.asptricks.net/2019/04/apidoc-vs-swagger-for-node-app.html).