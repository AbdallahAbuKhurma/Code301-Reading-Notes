# Message Queues
>
1. What does it mean that web sockets are bidirectional? and Why is this useful?

        That’s mean reliable two way sending and recieving between two networks in the same time.

2. Does socket.io use HTTP? Why?

        he initial connection setup it done over HTTP. Also, a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js

3. What happens when a client emits an event?

        Bind the socket to this server. Then listen to the connection event. When that event is invoked

4. What happens when a server emits an event?

        The client will be listening to the events to handle it

5. What happens if a client “misses” an event?

        can’t lestining to emmiting

## Terms

* **Socket vs. Web Socket:**

      WebSockets typically run from browsers connecting to Application Server over a protocol similar to HTTP that runs over TCP/IP. So they are primarily for Web Applications that require a permanent connection to its server. On the other hand, plain sockets are more powerful and generic. They run over TCP/IP but they are not restricted to browsers or HTTP protocol. They could be used to implement any kind of communication.

* **Socket.io:**

      is a library that enables real-time, bidirectional and event-based communication between the browser and the server

* **Client:**

      can be thought of as the browser. It connects to an established server and makes requests.

* **Server:**

      responds to requests from the client.

* **OSI Model (Operations Systems Interconnection Model):**

      Application -> Presentation -> Session -> Transport -> Network -> Data Link -> Physical. Explains how information is passed thru the internet from the browser all the way down to the fiberoptic wires.

* **TCP Model(Transmission Control Protocol):**

      uses less, but in effect more concise, levels as OSI to demonstrate how information is passed over the internet. It requires that all information from the server be present in order to fulfull the clients request.

* **UDP (User Datagram Protocol):**

      is similar to TCP except for that it allows for not all of the data to be present in the servers response to the client. An example of UDP is a streaming platform and when the client has to pause to buffer the streaming content.

* **Packets:**

      refer to the way that data is sent in the TCP model.

## Features of Message Queue services

* Asynchronous Messaging. Asynchronous messaging is a foundational concept for message queueing.

* Unlimited Queues.

* Real-Time Message Processing.

* Push and Pull Queues.

## Resources

[Socket.io Chat Example](https://socket.io/get-started/chat/)

[Rooms and Namespaces](https://socket.io/docs/v3/rooms/index.html)

[Socket.io Emit Cheatsheet](https://socket.io/docs/v3/emit-cheatsheet/index.html)
