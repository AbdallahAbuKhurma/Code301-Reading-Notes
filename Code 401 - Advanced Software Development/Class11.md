# Event Driven Applications
>
## Event Driven Programming

* Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

* An event-driven programming approach uses events to trigger various functions. An event can be anything, such as typing a key or clicking a mouse button. A call-back function is already registered with the element executes whenever an event is triggered.

* In an event-driven application, there is generally a main loop that listens for events and then triggers a callback function when one of those events is detected. In embedded systems, the same may be achieved using hardware interrupts instead of a constantly running main loop. Event-driven programs can be written in any programming language, although the task is easier in languages that provide high-level abstractions, such as await and closures.

## EventEmitter

Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. Of course, creating our own version of EventEmitter wouldn’t be much of a challenge, and in fact there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.

## Vocabulary Terms

***Authorization*** is the function of specifying access rights/privileges to resources, which is related to general information security and computer security, and to access control in particular.

***Role Based Access Control*** is an approach to restricting system access to authorized users. It is used by the majority of enterprises with more than 500 employees, and can implement mandatory access control (MAC) or discretionary access control (DAC).

***Capabilities*** A capability is a communicable, unforgettable token of authority. It refers to a value that references an object along with an associated set of access rights. A user program on a capability-based operating system must use a capability to access an object.

## Removing Listeners

There will likely come a time when you want to remove an event listener from an event. This could be for performance reasons (the event is no longer needed) or to avoid memory leaks (if an event listener references an object that is no longer needed, it won’t be able to be garbage-collected. This can lead to a build up of unnecessary objects).

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    SQL and Authentication.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    Event Driven Programming

3. What are you most excited about trying to implement or see how it works?

    Events.

## Resources

[Event Driven Programming](https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming)

[Node docs: events](https://nodejs.org/api/events.html)
