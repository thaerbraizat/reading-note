# Message Queues

1. What does it mean that web sockets are bidirectional? Why is this useful?

Whereas HTTP relies on a client request to receive a response from the server for every exchange, WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time.

2. Does socket.io use HTTP? Why?

the initial connection setup it done over HTTP. Also, a socket.io server will attach to an HTTP server so it can serve its own client code through .

3. What happens when a client emits an event?

The Socket.IO API is inspired from the Node.js EventEmitter, which means you can emit events on one side and register listeners

4. What happens when a server emits an event?

the client side will receive the handel of changes and got the results

5. What happens if a client “misses” an event?

'disconnect' would fire immediately on websocket close so a client could respond with some useful UI if it chose to, now it may wait 15 seconds or more before it finds out the connection is dead. This is undesirable for something like a chat app.

6. How can we mitigate this?

make sure the client connected befor send or make task queue.

* **Rooms and Namespaces** A room is an arbitrary channel that sockets can join and leave,Each Socket in Socket.IO is identified by a random, unguessable, unique identifier Socket#id. For your convenience, each socket automatically joins a room identified by its own id.Please make sure to use io.to(...).emit(...) (or socket.to(...).emit(...)) in a synchronous manner.

The “room” feature is implemented by what we call an Adapter. This Adapter is a server-side component which is responsible for:

storing the relationships between the Socket instances and the rooms
broadcasting events to all (or a subset of) clients

Room events
Starting with socket.io@3.1.0, the underlying Adapter will emit the following events:

create-room (argument: room)
delete-room (argument: room)
join-room (argument: room, id)
leave-room (argument: room, id)

* Socket.io Emit Cheatsheet 
* server side

io.on("connection", (socket) => {

  // basic emit
  socket.emit(/* ... */);

  // to all clients in the current namespace except the sender
  socket.broadcast.emit(/* ... */);

  // to all clients in room1 except the sender
  socket.to("room1").emit(/* ... */);

  // to all clients in room1 and/or room2 except the sender
  socket.to("room1").to("room2").emit(/* ... */);

  // to all clients in room1
  io.in("room1").emit(/* ... */);

  // to all clients in namespace "myNamespace"
  io.of("myNamespace").emit(/* ... */);

  // to all clients in room1 in namespace "myNamespace"
  io.of("myNamespace").to("room1").emit(/* ... */);

  // to individual socketid (private message)
  io.to(socketId).emit(/* ... */);

  // to all clients on this node (when using multiple nodes)
  io.local.emit(/* ... */);

  // to all connected clients
  io.emit(/* ... */);

  // WARNING: `socket.to(socket.id).emit()` will NOT work, as it will send to everyone in the room
  // named `socket.id` but the sender. Please use the classic `socket.emit()` instead.

  // with acknowledgement
  socket.emit("question", (answer) => {
    // ...
  });

  // without compression
  socket.compress(false).emit(/* ... */);

  // a message that might be dropped if the low-level transport is not writable
  socket.volatile.emit(/* ... */);

});

* client side 


// basic emit
socket.emit(/* ... */);

// with acknowledgement
socket.emit("question", (answer) => {
  // ...
});

// without compression
socket.compress(false).emit(/* ... */);

// a message that might be dropped if the low-level transport is not writable
socket.volatile.emit(/* ... */);