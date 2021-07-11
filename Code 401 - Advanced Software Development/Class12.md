# Socket.io
>
## Review, Research, and Discussion

1. What is the benefit of transforming data into packets?

    * meet the demands of pervasive data-centric applications and services.
    * most cost-effective, efficient, and scalable networks for content delivery.
    * redundancies for full visibility

2. UDP is often refereed to as a connectionless protocol. Why is this? -UDP is a connectionless protocol. No connection needs to be established between the source and destination before you transmit data. UDP does not have a mechanism to make sure that the payload is not corrupted. As a result, the application must take care of data integrity all by itself.

3. Can a socket server application have multiple socket connections?

    * A server socket listens on a single port has Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources.

4. Can a socket connection application be connected to multiple socket servers?

    * server socket listens on a single port. All established client connections on that server are associated with that same listening port on the server side of the connection. An established connection is uniquely identified by the combination of client-side and server-side IP/Port pairs. Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.

5. Can an application be both a socket server and a socket connection?

    * You can't have two client sockets connect to each other in TCP, as the low-level connection protocol doesn't work that way.

## Vocabulary Terms

* **Observer Pattern:**

  * The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

* **Listener:**

  * function in a computer program that waits for an event to occur.

* **Event Handler:**

  * is a block of code (usually a JavaScript function that you as a programmer create) that runs when the event fires. When such a block of code is defined to run in response to an event

* **Event Driven Programming:**

  * An event-driven programming approach uses events to trigger various functions. An event can be anything, such as typing a key or clicking a mouse button. A call-back function is already registered with the element executes whenever an event is triggered.

* **Event Loop:**

  * Event loops handle asynchronous callbacks in Node.js. It is the foundation of the non-blocking input/output in Node.js, making it one of the most important environmental features.

* **Event Queue:**

  * An event queue is a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system.

* **Call Stack:**

  * A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

* **Emit/Raise/Trigger:**

  * in event-driven programming, emit sends a message to trigger a response and raise an event

* **Subscribe:**

  * Subscribes an event handler method or procedure to an ABL or .NET class event.

* **database:**

  * A database is an organized collection of structured information, or data, typically stored electronically in a computer system. A database is usually controlled by a database management system (DBMS).

## WebSocket vs Socket.io

**WebSocket** is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

**Socket.IO** is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.

## Resources

[OSI Model Explained](https://www.youtube.com/watch?v=vv4y_uOneC0)

[Socket.io vs Web Sockets](https://www.educba.com/websocket-vs-socket-io/)

[Socket.io Documentation](https://socket.io/docs/v4/index.html)

[Socket.io Server API](https://socket.io/docs/v3/server-api/index.html)
