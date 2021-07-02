## Authentication

### Explain what a “Singleton” is (in Computer Science terms):
*in software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance*

### Explain how the Singleton pattern can be used with Node modules, specifically with classes:
*IT'S restricts the instantiation of a class to one "single" instance ;useful when exactly one object is needed to coordinate actions across the system*

### If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
*use the singleton approch*

### Router Middleware:
*is functions that have access to the request object (req), the response object (Links to an external site.) (res)*

### Dynamic Module Loading:
*is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory.*
 
### Singleton Pattern:
*is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system.*

### CRUD -> REST Method Matches:
*(Create, Read, Update, Delete) is an acronym for ways one can operate on stored data*

### Mock Testing:
*is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules*

## Basic access authentication:
*In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon :.*

### Protocol:
#### Server side:
When the server wants the user agent to authenticate itself towards the server after receiving an unauthenticated request, it must send a response with a HTTP 401 Unauthorized status line[5] and a WWW-Authenticate header field.[6]

The WWW-Authenticate header field for basic authentication is constructed as following:

WWW-Authenticate: Basic realm="User Visible Realm"

The server may choose to include the charset parameter from RFC 7617:[1]

WWW-Authenticate: Basic realm="User Visible Realm", charset="UTF-8"

#### Client side:
When the user agent wants to send authentication credentials to the server, it may use the Authorization header field.

The Authorization header field is constructed as follows:[7]

The username and password are combined with a single colon (:). This means that the username itself cannot contain a colon.
The resulting string is encoded into an octet sequence. The character set to use for this encoding is by default unspecified, as long as it is compatible with US-ASCII, but the server may suggest use of UTF-8 by sending the charset parameter.[7]
The resulting string is encoded using a variant of Base64 (+/ and with padding).
The authorization method and a space (e.g. "Basic ") is then prepended to the encoded string.
For example, if the browser uses Aladdin as the username and open sesame as the password, then the field's value is the Base64 encoding of Aladdin:open sesame, or QWxhZGRpbjpvcGVuIHNlc2FtZQ==. Then the Authorization header field will appear as:

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==

### bcrypt docs
#### node.bcrypt.js:
*A library to help you hash passwords.*
*bcrypt module uses node-gyp to build and install, you'll need a stable version of node to use bcrypt.*

#### Install via NPM
*npm install bcrypt*




 