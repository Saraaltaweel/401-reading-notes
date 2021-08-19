1. What are the advantages of storing tokens in “Cookies” vs “Local Storage”?
*Cookies and local storage serve different purposes. Cookies are mainly for reading server-side, whereas local storage can only be read by the client-side . Apart from saving data, a big technical difference is the size of data you can store, and as I mentioned earlier localStorage gives you more to work with*

2. Explain 3rd party cookies.
*A third-party cookie is placed on a website by someone other than the owner (a third party) and collects user data for the third party. As with standard cookies, third-party cookies are placed so that a site can remember something about the user at a later time*

3. How do pixel tags work?
*Pixel tags are typically single pixel, transparent GIF images that are added to a web page. Even though the pixel tag is virtually invisible, it is still served just like any other image you may see online*

### cookies:
*small bit of data stored on a user’s computer by the web browser while browsing a webiste, designed to be reliable mechanism for websites to remember stateful information or to record the user’s browsing activity*

### authorization:
*is a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs, data and application features*

### access control:
*Component of data security that dictates who is allowed to access and use company information and resources. Through authentication and authorization, access control policies make sure users are who they say they are and that they have appropriate access to company data*

### conditional rendering:
*In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application. Conditional rendering in React works the same way conditions work in JavaScript*

## Redux:
*is a state container for JavaScript apps, often called a Redux store. It stores the whole state of the app in an immutable object tree. To create a store the createStore(reducer, initialState], enhancer]) function is used to create a new store*

### What problem does Redux solve?
*Redux provides a solution by ensuring that: Your state is wrapped in a store which handles all updates and notifies all code that subscribes to the store of updates to the state*

### Who to use Redux in react
- *create store as we create context*
- *pass store and context to provider*
- *imported as context exactly*