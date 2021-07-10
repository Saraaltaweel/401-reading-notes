### Name 3 real world use cases where you’d want to change the request with custom middleware
1. Authentication
2. Web server
3. api

### True or false: The route handler is middleware?
*true*

### In what ways can a middleware function end the process and send data to the browser?
 without using next() and it's passing data


### Middleware :
*Middleware is functions that have access to the request object (req), the response object (Links to an external site.) (res)*

### Test-driven development (TDD) :
*is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases. This is opposed to software being developed first and test cases created later.*

### Behavioural Testing :
*is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.*

### Request Object :
*Represents the information in the HTTP request from the client to the server.*

### Response Object :
*Information in the HTTP response from the server to the client.*

### Routing middleware :
*Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router().*

## Express Routing

### Routing Types:
- Route methods: as GET method route POST method route
- Route paths :in combination with a request method, define the endpoints at which requests can be made.
- Route parameters: are named URL segments that are used to capture the values specified at their position in the URL.
- Route handlers: You can provide multiple callback functions that behave like middleware to handle a request.
- Response methods:The methods on the response object (res)
- app.route() :used to create chainable route handlers for a route path Because the path is specified at a single location, creating modular routes is helpful, as is reducing redundancy and typos
- express.Router: class to create modular, mountable route handlers.