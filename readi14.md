# Event Driven Architecture

1. What’s the difference between a FIFO and a standard queue?

FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers

2. How can the server be assured a message was properly received?

by a received messages from client-side 

3. What classic design pattern is best represented by event driven programming?

Event-Driven Primitives
All interactions taking place in a distributed system over a network can be categorized into just three primitive types: events, commands and queries.
When talking about Event-Driven Systems, this distinction helps vocalizing the intent behind sending a message.
Events
Whenever a system performs an action, the message containing the observation of that fact is called an event.
You can think of events as plain information saying that “something has happened”, like a log entry. An observable fact. Events may or may not trigger a side-effect.
Events have two primary functions:
They are triggers of side effects somewhere in the system.
They are also carriers of arbitrary data.
Just like pure information, events do not necessarily carry any expectation of future action to be performed or response to be returned, but they can still carry data. We will see later how we exploit this duality to distinguish two very different, yet powerful, Event-Driven patterns.

4. How do you test an event driven system?

we write cases in test.test.js file and we run it by using JEST

* **AWS SNS and SQS**  

SNS is a publisher subscriber network, where subscribers can subscribe to topics and will receive messages whenever a publisher publishes to that topic. AWS SQS is a queue service, which stores messages in a queue.
![SNS VS SQS](https://res.cloudinary.com/practicaldev/image/fetch/s--xU0ynxUd--/c_imagga_scale,f_auto,fl_progressive,h_500,q_auto,w_1000/https://dw71fyauz7yz9.cloudfront.net/video-upload__c8bc44f83cd41222de8ae55b55c63ef2/thumbs-video-upload__c8bc44f83cd41222de8ae55b55c63ef2-00001.png)