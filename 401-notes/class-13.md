## Class 13

### Reading

#### Socket.io Chat Example

1. Explain to a non-technical recruiter what the Chat Example (above) does.

  Essentially each client is connected to one server where each client can send and receive messages.

2. What proof of life are we getting on the backend from the above app?

  the `server.listen` and console log.

3. Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?
Rooms

    `socket.broadcast.emit`

#### Rooms

1. What is a room and how might a room be useful?

    A rooom is arbrary channel that sockets can `join` and leave. It can be used to broadcast events to a subset of clients.

2. How do you join a room?

  An example of joining to a socket is:

    `io.on("connection", (socket) => {
  socket.join("some room");
});`

3. how do you leave a room?

    An example of leaving a room is

    `io.on("connection", socket => {
  socket.on("disconnecting", () => {
    console.log(socket.rooms); // the Set contains at least the socket ID
  });

  socket.on("disconnect", () => {
    // socket.rooms.size === 0
  });
});`

#### Namespaces

What is a Namespace and what does it allow you to do?

A namespace is communication channel that allows you to split the logic of your application over a single shared connection(this is also called "multiplexing")

Each namespace potentially has its own what? (hint: 3 things)

  - Main namespace
  - Custom Namespace
  - Client initialization


Discuss a possible use case for separate namespaces

  A namespace that only has authorized users.

#### Bookmark and Review

Reflection

1. What are your learning goals after reading and reviewing the class README?

A better understanding of sockets

#### Things I want to know more about

How to implement sockets in my programs 