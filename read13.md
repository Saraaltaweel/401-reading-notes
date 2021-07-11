
1. What does it mean that web sockets are bidirectional? Why is this useful?
*That's mean reliable two way sending and recieving between two networks in the same time.*

2. Does socket.io use HTTP? Why?
*he initial connection setup it done over HTTP. Also, a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js*

3. What happens when a client emits an event?
*Bind the socket to this server. Then listen to the connection event. When that event is invoked*

4. What happens when a server emits an event?
*The client will be listening to the events to handle it*

5. What happens if a client “misses” an event?
*can't lestining to emmiting*

### Socket:
*protocol to open the network connection for the program, allowing data to be read and written over the network.*

### Web Socket:
* is a computer communications protocol providing full-duplex communication channels over a single TCP connection.*

### Socket.io:
*is a library that enables real-time, bidirectional and event-based communication between the browser and the server.*

### Client:
*it could be a browser (front-end) or a server with an open socket to the original server.*

### Server:
*is a computer that serves information to other computers(clients).*

### OSI Model:
*stands for Open-System Integration model, is a model that characterizes and standardizes the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology.*

### TCP Model:
* is a suite of communication protocols used to interconnect network devices on the internet.*

### TCP:
* is a standard that defines establishing and maintaining a network conversation through which application programs can exchange*

### UDP:
* is part of the TCP/IP suite of protocols used for data transferring.*

### Packets:
*it is a form of data that consists of a small amount of information with a port number, IP addresses to the sender and the caller, and a tail part that contains some protocol information.*


## Message Queues

* A Queues of messages sent between applicatios includes a sequence of work object wating to processe

* A message is the data transported between the sender and the receiver application; it's essentially a byte array with some headers at the top. It is a form of asynchronous service-to-service communication used in serverless and microservices architectures. Messages are stored on the queue until they are processed and deleted. Each message is processed only once, by a single consumer. Message queues can be used to decouple heavyweight processing, to buffer or batch work, and to smooth spiky workloads.*

### Features of Message Queue services
- Asynchronous Messaging. Asynchronous messaging is a foundational concept for message queueing.
- Unlimited Queues.
- Real-Time Message Processing.
- Push and Pull Queues.