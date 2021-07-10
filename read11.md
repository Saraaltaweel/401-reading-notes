1. Why is access control important?
*Access controls limit access to information and information processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorisation, unlawfully and the risk of a data breach.*

2. Describe an application that would need access control.
*Login credentials (such as usernames and passwords). PINs and one-time passwords (OTPs). Virtual private network (VPN) access to internal networks.*

3. What is a role used for?
*to determine what part of the system this client has access to it.*

4. Why is role based access control more scalable than discretionary or mandatory access control?
*user under RBAC may only be assigned a single role in an organization. Additionally, there is no way to provide individual users additional permissions over and above those available for their role.*

### Authorization:
*is a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs, data and application features. This is the process of granting or denying access to a network resource which allows the user access to various resources based on the user's identity.*

### Role Based Access Control:
*Role Based Access Control (RBAC), also known as Non discretionary Access Control, takes more of a real world approach to structuring access control. Access under RBAC is based on a user's job function within the organization to which the computer system belongs.*

### Capabilities:
*list of actions that user can be able to do it.*

## Event-Driven Programming in Node.js:

### Event-Driven Programming:
*logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision*

`const Mailbox = {`
  `sendMail: function(){`
    // code to send mail.
  `},`
  `receiveMail: function(){`
    // check server for new mail.
  `}`
`}`

* events module from node.js.
- npm i events

`const EventEmitter = require('events').EventEmitter;`
`const myEventEmitter = new EventEmitter;`
