# Socket.io 

1. What is the benefit of transforming data into packets?

TDM-based networks must transform into packet-based networks to meet the demands of pervasive data-centric applications and services. Packet-based networks not only enable new innovations, services, and business opportunities, they are also the most cost-effective, efficient, and scalable networks for content delivery

2. UDP is often refereed to as a connectionless protocol. Why is this?

UDP is a connectionless protocol. It is known as a datagram protocol because it is analogous to sending a letter where you don't acknowledge receipt. Examples of applications that use connectionless transport services are broadcasting and tftp .

3. Can a socket server application have multiple socket connections?

Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to

4. Can a socket connection application be connected to multiple socket servers?

A connected socket is assigned to a new (dedicated) port, so it means that the number of concurrent connections is limited by the number of ports, unless multiple sockets can share the same port

5. Can an application be both a socket server and a socket connection?

yes ,
* var io        = require('socket.io').listen(server); // this is the socket.io server
* var clientio  = require('socket.io-client');         // this is the socket.io client
* var client    = clientio.connect(...);               // connect to second app

* io.sockets.on('connection',function(socket) {
*  socket.on('eventFiredInClient',function(data) {
*    client.emit('secondNodeAppln', data); // send it to your second app
  });
});