1. What’s the difference between a FIFO and a standard queue?
*FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers*

2. How can the server be assured a message was properly received?
*we can use the socket.io’s acknowledgements.*

3. What classic design pattern is best represented by event driven programming?
*Event-driven from end to end*

4. How do you test an event driven system?
- Ensure supporting topics exist
- Start the application under test (“application” here could mean Kafka Streams, Kafka connectors, Samza, etc.)
- Send some input events

### FIFO Queue:
*(First-In-First-Out) queues are designed to enhance messaging between applications when the order of operations and events is critical*

### Pub/Sub:
*is an asynchronous messaging service that decouples services that produce events from services*

## AWS SNS and SQS
* SNS supports several end points such as email, sms, http end point and SQS. If you want unknown number and type of subscribers to receive messages, you need SNS.

### Event Driven Architecture
*(EDA) is a software architecture paradigm promoting the production, detection, consumption of, and reaction to events. ... A car dealer's system architecture may treat this state change as an event whose occurrence can be made known to other applications within the architecture*

### Use Cases
* Choose SNS if:
- You would like to be able to publish and consume batches of messages.
- You would like to allow same message to be processed in multiple ways.
- Multiple subscribers are needed.
* Choose SQS if:
- You need a simple queue with no particular additional requirements.
- Decoupling two applications and allowing parallel asynchronous processing.
- Only one subscriber is needed.