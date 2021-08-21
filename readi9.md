# Event Driven Applications

![api](https://scotch-res.cloudinary.com/image/upload/w_1050,q_auto:good,f_auto/media/1/nrMHOlRR6imGBoKkDZLJ_getting-started-with-node-express-postgres-sequelize.png.jpg).

1. Why is access control important?

Access controls limit access to information and information processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorisation, unlawfully and the risk of a data breach.

2. Describe an application that would need access control.

university application

3. What is a role used for?

the role means what the data the user allows to read or update or delete.

4. Why is role based access control more scalable than discretionary or mandatory access control?

 RBAC is superior to ACL in terms of security and administrative overhead. ACL is better suited for implementing security at the individual user level and for low-level data, while RBAC better serves a company-wide security system with an overseeing administrator.


 * **Event Driven Programming** 

 Event-Driven Programming makes use of the following concepts:

An Event Handler is a callback function that will be called when an event is triggered.
A Main Loop listens for event triggers and calls the associated event handler for that event.

Event-Driven Programming
js uses events heavily and it is also one of the reasons why Node. js is pretty fast compared to other similar technologies. As soon as Node starts its server, it simply initiates its variables, declares functions and then simply waits for the event to occur.


* **Node docs: events** 

uch of the Node.js core API is built around an idiomatic asynchronous event-driven architecture in which certain kinds of objects (called "emitters") emit named events that cause Function objects ("listeners") to be called.

For instance: a net.Server object emits an event each time a peer connects to it; a fs.ReadStream emits an event when the file is opened; a stream emits an event whenever data is available to be read.

All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter.on() function that allows one or more functions to be attached to named events emitted by the object. Typically, event names are camel-cased strings but any valid JavaScript property key can be used.

When the EventEmitter object emits an event, all of the functions attached to that specific event are called synchronously. Any values returned by the called listeners are ignored and discarded.